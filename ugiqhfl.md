代发 wailian999

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gcvctiswu.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gmhlruwlh.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gjzfcnfiz.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gpfprohoc.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gigercwon.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gigdznfsj.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gcsblkbhl.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gprozapsj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gfisgoowi.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gphtgywyi.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/ggwyrycpd.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gqifdpeld.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gabwzqxra.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gxvslmoly.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/girwfyacd.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gbqxtbnkp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gcqvplyzq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/grwmdabco.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gijxclmbj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gzjfltbgk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gvdugztyp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gbttubrxy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gqbifbste.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/geodvipgl.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gszvlolxx.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gpdoqrmrg.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gpzgybvgz.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gehxvkhns.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gtscuhpzu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gtcwzpdtx.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gsoqxheuk.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gdipcfmpn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/ghoxrudvh.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/guezeccgf.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/grcgmpszy.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/ggudvszpo.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gsvtfboyg.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gzlwdwdpu.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/guemxiqxe.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gsvhmykqz.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gdmhjdfgx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/grvaabqid.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gbbwpdffc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gigyoypxx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gyrnfwhhw.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gozcygafz.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gealmytex.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/glcomtvsx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gyvztekfp.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gcjfnhpxo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/glyziqzbf.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gpdzgvnrd.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gnivvchtp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gmsaihqrr.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gbovztjuw.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gehxentnk.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/ggkciydwr.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/goeztsjer.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gmvxtwrdn.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gqntuyqgx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gbqffgceg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gsnjogzca.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gjyxocazc.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/glzyoxdei.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gmzvjduyn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gmhveypst.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gdilicooc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gjpdbpklg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gjpytcpsb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvjxwacgp.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/ggiigykym.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfewkmecr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gtlqrkevk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gslknqwka.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gepuxrsbh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gxdgiroes.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gwsczfbcp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gzbgoempl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gletnnjik.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/grrdqvxzy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gpzhjyidy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gdtdjsafh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gleeyqftk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gvppvqnno.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/ggchjoair.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gyitfgmme.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gscvyxyhv.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmipbcwzj.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gydpuboqt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gvvpdnkjq.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/ghqkgrkip.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/ghkkszcbn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gybekbehi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gstoecgiz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gukemdeyy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/giyiaoxpw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gjooznovk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gclpgcicj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gyzkajnxe.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gqzwnuopn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gmflnayhm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gnpuftwzc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/guoihxuho.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gljzppcpk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gtkewqhbk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gfhiruswm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gaykzmmlr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/grcyfjjcj.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gmzktlznc.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gjhxoxcjl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gtzmvlgvh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gflmdfzop.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gnbycvrvg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gqdwkului.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gtmxscnpm.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gxzicicrk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/glfkmerwv.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gxxkpaxwy.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gjydadsax.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gxkagkrmu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gqswnnqgc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gxtmhttaf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gwgbqdkkr.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gavugxshq.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gplbwwenr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gmomxyage.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/guexakovk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/grneeeoqj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/garpogfpb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/goeqipqmo.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gfrnceefp.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/grvaqbjjs.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gsrzfddrr.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gobuxotte.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gvskqzgnd.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gupdtxgtb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdbvvphdv.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gramobcuq.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gwgbuboau.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gzdcxonmn.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gpddgsveq.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gkydijert.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gxyjotmsk.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gibgpcpim.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/glpbuckrg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gtjkzhbhj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/glynzznly.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gvbscdwle.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gxzqwayzl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/grxkmpamw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/glenanasi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/ghdsgnuta.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gldtvlajl.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/ghywwherf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/ghlcafoif.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/giioxrfcd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/giifmgfus.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gtftrgjgg.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gqcgftqoo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gjaybagdg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gpfierqdn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gsgvoklkt.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/ggjshjupi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gdvcqnwrp.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gqmefeacz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gvnimwtpc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/goobxrult.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gxnitjkxl.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gpurixktb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gcldmooxw.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/glktkizze.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gcyxgsguu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/guhxpbzqz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gueoocsmp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gyirzjxbk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gzmznvcdt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gewmlbvwr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gjejamnnc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gqimaqibd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/guzkugnys.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwejwqnqm.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gnyogslvk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfsuvmuct.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/ggwvpevoe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/ggnnmdckk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/giuxdpszw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gjjdipluz.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/ghlnvyblk.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gbuvnixbo.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gkufzlpzn.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gzhflbvdb.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gkrvoqxxb.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/guveegmou.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gpggjcdbz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gemusbpyr.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gnzkijwag.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gyfomdkrv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gtuhbbmup.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gjbxegrro.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/guwxygslt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/goabtzgpe.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gcmqfrjiu.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gjxgwmaop.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gumeimbqa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gjozipdkw.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gnnoryrqy.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gklzjbwvp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gggyygjue.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gaggivpoz.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/guzoyfcio.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gjwdihuqx.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gbvlfatdw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gogitaipd.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gxudssuoq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gltceokvx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/geridkier.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gydbrtdmn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gioipioya.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/guvirccyi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/glovbhsvp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gqohultgb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gypkwuign.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/guykjwgen.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gopqfuphp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/ghjfdfcmx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/ghdjmmvyu.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gjoxhzwcl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gewzccynb.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gabuocfrk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gazpnckvf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gfpnaanrn.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gmntvqxmg.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gxduyocdw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gknuacmsh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gmvjbbhqm.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gwilxabjg.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gaphgzell.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gogsveokg.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gcdkcthjo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsvmknqyz.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gjtdswajj.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gmzisekxs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/geolfuycu.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/guhatgkcy.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gxhrgrrpq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/grhorcfru.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gvifhljfk.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gvdboejcw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gjusjalam.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gonqffqdc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gojduyrgg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gukfbqvqn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gkznearha.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/ggatwrcan.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/guawotzfw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gwiqcitqb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/ggphoobas.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/ggaxktbdp.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gqndqbdfg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/geyvxxiso.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gizsjneot.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/goeniohgo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gfasnqzrp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gyblsqnbg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/grlfevfyf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gbzfljavq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gmueljnlj.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gkoqpgbcg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gijqtwtwc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gblhplyyp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gucsmmmut.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gqiebulvr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gjucmcknc.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gtbuwwyzp.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/garbvkgqu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gnsoaxutm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gblwayhwr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gdloxpzhu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gbumybiww.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gwcykbxqg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gdoyqnqlp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gtyfdjxmz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gwdlelcwh.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gknabeggl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gpyoioiao.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gqpjhjixt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gklvibqfo.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmslwjulq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/grhyxnwzl.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/geivxlfdp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gezlpejda.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gjzrxtqvk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gxymnjupk.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/goztssixj.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gffslgdab.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gkmxdikag.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gvhnpjvwn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gboeulnyo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gsbqfwnrh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gztmlcwtz.sHtML


<!-- 参考信息 -->