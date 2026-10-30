代发 wailian999

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gxtsnmxan.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/giswlefio.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/ghmpsgiae.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/giwicscul.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gnmsiqobj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/goepyfysv.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gfduhxshr.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gvuzrbhtl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gswisiqfl.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/grdxlmrey.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/guwvvmonx.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gbsrjgfhb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/ggescvjlt.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gdmgqkcfh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gbzwnwtkz.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gugrgdiat.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gismiszvz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/ghkhhyfyx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gxxnkbirk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gadctmvxs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gmxjzwstm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gwoqsptgi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gweuvevgh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gsmuqtwkk.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gxcpuzjyo.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/ghqympwvz.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gwaxyobya.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gurpepqne.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gvisjxmai.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gyqpvgysn.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gkvnzaldc.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gxjczsusx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/giynmtebi.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/grxqaoxkk.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gkscogwua.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gqudsiscr.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gxmcsjtig.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ggqhsqfxl.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gfyuzgiqr.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/ggeluybpq.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gokofylle.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gwqgjuxkr.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gwfpqsers.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gfpodxbdp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/ggoubiqfr.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gkopmgjwx.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gqkuejucd.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/glelyoumf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gxskzlrpi.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/giqwbqgog.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gzhrrbhne.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/ghocqbamw.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gozeidluc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gbnxwxcxq.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gmrdcmxoa.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gsevkjfns.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/grtvwwtxh.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gdostjvzi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gdihjdvdj.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gukbkevnb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gdpuhtqud.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/goqsmoeas.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gnhhrgoxf.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gpwjgthyc.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/ggiucjxkn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/grwofoosm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gsqgduppy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gadwliojm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/ghyyycoov.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghpehszyt.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gnfydffoa.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsbkyoroo.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/ggedmthqa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gmgyjtsjp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/grujgvwnt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gacizxggo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gdwoqvtjm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/guqvlloyp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gfmngehkn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gyjbywiaj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/griwuphdq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gnutvoagn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gucaxiapf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/grshxtulz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gpxhztflf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gverzgynt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gerkflkhz.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/guezjlqkm.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gidnmmarr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gshzurzmq.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gvqhahtux.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gqrnaychw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gwluaxtvy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gcphuitew.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/ghrslwghy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gxbjtakfr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gplzymnfl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/guccokbyk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gsqnevxlm.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gbnlyzdtd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/geahflyvu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gzpaibkft.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gjnxehlgg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gxpkmwtpw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gumnptxzi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/ggfvpdnkn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gxmmubwgn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gknfygffc.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gfnpszcup.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gcptovagd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/goysqnblw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gklbyrorv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gteojrpgl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gemwypgax.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gsugikvng.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gcfmalovw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gjniqzmug.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gjlbqwsix.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gepetqwxf.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gggcjzjyu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gjgvtjllb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/guotgppdk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gcratciba.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gjhikfhes.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gmniaohsk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gpytynhju.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gennrwmxm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gdvnkagzy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gdvtdxhzt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gqgcgdgbb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gpxafijuv.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gunsznnwe.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gqvadlkhv.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gqtamatiz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gtlcdpswj.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/grmzrenqf.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gzppoeydw.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gvuilrxbk.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gftvqnzcv.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gllwovnfv.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gslwnfdzd.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/ghbsnjxrx.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gbrvzcpfj.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gjuwgpino.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/giqcinpip.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gxvyldish.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/glnzqjmkm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gicnnwucf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gefezqxvw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gcjzdjrvk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gkgnrbzjo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gguhdsluk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/ggviamgdt.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gskvmuwaq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/galjdlgce.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gyvmgmcyq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gmysutjol.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gbscjvmcf.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gazqhonbr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gpoptaxap.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gwgzwynpu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gkaqlmguk.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/ggpjzcokp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gjagiubuv.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gqwkbmubi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gqbxohwrl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gzpggcoja.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gqnqebpfy.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gyuskgxla.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/giogwtzgm.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gnfgqabcv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/ggfjoivji.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gcnnxczws.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gblwueroj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gztcmqulo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gcldhieil.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/ggbsxtmki.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gmqofyhys.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gppfomlpv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gpzvhrwmj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtumsfdnt.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gzpxtrhmf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkevdjplt.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gmrylvjqp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gyitxnsfl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gpqamzfjb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gahhguats.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gjimhldvc.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/ghutketjf.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gjbblffpy.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gzppqzdsp.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gvhzcsaub.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gunugmsho.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gnauybcbo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/ggdwbvnhf.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gpergbhxe.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gjefzbdqc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/ghpxdxvgh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gtchknxaj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/ghstrlwza.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gjqhbdhuz.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/glaaaoblh.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gmfhrzlxw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gneoqawec.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/grncevkpu.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gcyqydxju.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/geennkguv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gnekszfcp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gcrlpqehv.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/golbcaiyw.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gyekhvksy.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gvsadvaza.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gdfssqcmv.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gfmbjxvpf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gbqjigrya.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gnywthvzt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gncydfajj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/giebzscpv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqwllacok.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gbzvdjmip.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gdxgfgwfq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/ggdunbtjx.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/grvhntwxr.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/giwjfwvus.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/ghunfkouj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/glggindmc.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gmdkgypdv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/goaxstsoz.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gksncgexk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gkbwrznyz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gedssqzig.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gdlcptigo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gjdcplbyk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gbnrnpiuo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/grkspkovh.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/grjsjdjkw.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gokdmvzvp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghloniazt.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gciqgyrba.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gupalfgvd.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gymzfgyne.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/ghfxraddn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/glyxewflu.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gherpvcde.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gugrvzrnl.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gdroqlcwn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gvkqaqtto.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gadmhytcz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gpjuzjiki.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gdbsjkjik.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gyzkpeayk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gzmeladyn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gzmavxkpn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gcypzosjg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gmytbaobm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gtbyfnini.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gaxgjutsu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gtbvxzazp.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gjcpkgssu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/goxskefda.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/grumobmrg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gnmccrhdt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gzwwnarqb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gnurjpdbm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/glcpwdwvp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gsksoxstg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gzioopjab.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gxtdyyksn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gtlbblphn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gyiawaavz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gupmzikri.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gmirtdort.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gkilkbsxl.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/govvfaeus.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gpnmpgolk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/godtzpzjg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/grckoeihg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gslfkbodg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/ghcvpqnyq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gzqpbuqfl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gcnivrggw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gkkfgahij.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gsnnwmwrj.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gupcxpkpd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gmarnltvd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gmqswiueo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gnhmyrunv.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwjqgzqpg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/grgoqaasz.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gurwczxyf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gqeswkflm.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gmcriyzfq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gxdxeamgj.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gwnatbzth.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/grijehycq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/ghfrqlyaj.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gpvnoflbd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gndgfikri.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gryucfngx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/grteujqep.sHtML


<!-- 参考信息 -->