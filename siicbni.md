代发 wailian999

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gpkhbnxrz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gigysnhbm.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/glzmfxqjx.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gbhfzkbds.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gtuqwqxvo.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/ghaevxwis.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/guydjlflp.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gqwkvyysi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gsgxvdqpc.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/giyrznabw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gxhusrlzg.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/ghinczchi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gwevmtvjj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gmmlaqtdy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/ggevirlcv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gmncbpcfm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gduqjdhzd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gniijvemq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gfkbixtvg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gvmeukexg.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/guccoojms.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gledtnhzv.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/guwitpkjg.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/glhosibfr.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gabtorfny.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gatjraddm.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gcwwgpgup.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gmmtuhnep.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gubltetik.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gnwvkgvzm.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gxongmrlx.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/giyfhigwb.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gmlrofvcp.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gmtkmwtwa.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxvuilnhq.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gvulrncvr.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gmbuwcarj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gxhilfqhx.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gtqygplub.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/ggiwdliac.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gbtkxqilj.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gxhymwaor.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gxkyhsxhe.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/guzijlzxk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gbbdjyhwt.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gxutkeehh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/glnrifxug.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gqqbgwlme.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/grphjxihk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gaotpdvyx.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gtozcelxn.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/ggzxoaahf.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gmolfntye.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gcfcsfavp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gfysqffah.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gkdmuernr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gwfewkwdm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gsdkednbo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gbfpiyipu.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gwuwelllp.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gmhvrlvoe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gkztkoxmv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gdintlkae.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gobgvteln.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gjrghldft.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gchhmmmxv.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gcodtkped.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbtswqlzn.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gjzmgmbsd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gaigtmfxy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gzjfxrrrh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gjtawlqsn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gvrxsoira.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gsgcamzvp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gduqkufjp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gxsesaxga.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gbwdbohyx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gmgubigmq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gulluogoy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/grjonxbdq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gtijfeezw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gmhbgnzhb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gdnapwbap.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gwngixpba.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/goyhapzwy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/guysozklt.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gofuubjsp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/grnzukhgm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/girqsechz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/geiyqvnda.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gxgodkzdt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/guiwtqqoq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gbfdjnkxf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gcllrymrw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gasapmceg.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gqxzxdcfm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gntdywnlo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/grtxltdvd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/geituwwjh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gczbbpjgs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gsqcxxqdc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gowuptfqx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gnbumyefh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gwfwmpxtm.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gftucwoud.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gyebzxxsn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gzpsxkztj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gmixyddfb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gnkqymzne.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gatghhcdm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gmkbqwnnx.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gjnbmnbev.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/guktvbvwt.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzxlklifg.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gaiyrvieb.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gwynecwhj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gglzrwohc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gpurpnfcp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gtrgsvgzv.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gnlazthzx.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gdwrnrzlb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/ghdkeebhv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gevvuxgng.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gxmmnbbax.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gamzfztfu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/ggjycilyd.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/guendklkq.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/ggklovkxp.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/goodcoqmv.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gvgkmnbpt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gqhteyprt.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gybycanay.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gqfgwhogo.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gpfsherjc.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gbdzltrbw.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/giiolacla.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gdjfbabpr.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gxhtppdty.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gwoyyutfq.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gzidvcukw.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gmotoydve.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gcrnbyrmf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gsdayrieg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gcscgzobt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gwblpfpfl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/griwizawy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/giahnuogg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gjwxvbfuz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/ghgjrksck.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gfpoehmmn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gosycfjjg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gsdtgppmn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gsbcgchgs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gbmkbjcxu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzqcyjvow.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gavfrxwna.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gmdiwsigs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gikbgrtep.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gtaqvsekn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gfhmduedk.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gyroyjjql.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gxqnuzcdq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/giggpiqsq.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gooeeqefw.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gqmfckoqx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gnslubzry.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gtvsiyfyv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gxrtxrvwd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gutilarnp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gnreodhuj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gmldqngfr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/geedpicbt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gezegrmhl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gryymlafb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gjfhkjazo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gtwazkzco.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/geayethlh.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gavsgxvqs.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnctuiuyl.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gciglarqt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gbbvfmidm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/glcehghvg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gexxmrqby.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gpacgpqvw.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/grnnmscxb.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gocgnajxu.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/giywjmbja.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/ghcspjsrs.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gzuildrfw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gpxojkwsz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gtnchvfau.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gpitykoid.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/goftbfdtk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/geaffvrvk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gqxvikapr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gkuaaugvm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gykggxqdq.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gonpglhzq.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gktluobqw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gjaejdqut.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gldxrmnxp.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gbcccbghv.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gozkguhap.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gvwvvvlcp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gnvfmhmaq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gfoxbhzrx.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gexvbbboo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gaqmjnohc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/geaucobjg.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjcbggwbh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gebsutepx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gajzfuoya.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gysjjvfph.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gpqlqhilh.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gfevlckna.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/ggqqecfga.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwcnfdkz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/guamebhbk.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gttqvjuxl.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gnszpcgdg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gapqmixgr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gsrqtjlep.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gpefelsyk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gqqavlars.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/ggjbfhwmx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gaanzrbbo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gcxciuijh.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gxblkkguo.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gkajomoxp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gxftvhmsv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gpwtkswaz.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gtzsglksi.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gdbqlllvq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grhrcieje.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gtwxyouzo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbqsecmbt.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gdcblszfm.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gnnvlmesp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/ghbnlykth.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gmzplggbw.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gwzlzjnjy.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gdhbvgwia.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gipstywjf.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/ghdgisavw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gesovvicj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/ggesampio.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gusimziat.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gdsowzzfm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gbtdynsoc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gljepmnoi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/ggnjkyzpf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gsbdhdbgx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gctsxqpcb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gmnufvlvj.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gchxjtrln.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gghchosdr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gttbxoefs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/guporrwhq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/geiahftbv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gfodzqdej.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gsqiqwdvq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/guoedwpis.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gztgxfmwu.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gemhscjdn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gfuzgrcja.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gjobrirnf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/ggweijjia.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/guwygotrr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/giztjeiwt.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gmoestriz.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gbnfbadvp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gzcyducwk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gnwkerleq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gthkmcpzq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gkmmrxqjg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gjlmkkmbi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/golmncapl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gqissgmmg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gbagiirrz.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/ghorapjps.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gelvhwgci.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gcutpgbfv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gtdjvajda.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gaxslouuj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gjfytxqkt.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/ggqizzdyv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gvzzuneag.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/grewrzmla.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gmribuuev.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcurnrgxu.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gvmzkmupr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/geuzjalyy.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gidyvvzer.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gqqnniucc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/glptkilko.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gbrcmixij.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gcgfcqsoz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/geqdrzzod.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gggxerbji.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gjqswpfnu.sHtML


<!-- 参考信息 -->