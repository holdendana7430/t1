代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gxyujqjxq.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gzgetxftz.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gvhfbvqrh.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/glutemook.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/grgyyygib.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gjqfasrgz.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gjkvdodmz.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gxidybrmr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gwlwjndmj.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gdbgxlwwh.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/grsfgluyy.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/goyojwojw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gbeasjyir.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gnwuortag.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/ggpwrhkew.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gqkweutyn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gybneywgq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/glbjwmkyc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gspugeumh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gvmputwpu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gmlkwrdvc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gotwnyxmk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/ginoftmfx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/ghuqzonsr.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gabdgfsuk.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gbqkdfvgt.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gjujhwrsy.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gzmuawfck.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gwvrifxab.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gtdxnmnrb.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gpsklwnhh.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gueiacman.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gefynhvsh.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gncbuworw.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/glfulbxng.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/geycxelwz.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gwubqlhon.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/geeaebzog.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gbuwzyohq.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gqnpieqlx.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gyoesyxxz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gqzdtjtig.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gpkaypxld.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gzhqajlgg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gupaggiej.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/goxrylapr.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gylqjnvbs.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gjirrexij.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gcpiuzdln.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gwokazuvz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gibrcvfep.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gmnavvwkb.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/goqhbzwzo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gvstcchia.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gidlphlgs.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gyzetttlq.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gcmscozul.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gqyklagof.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/ghovbsnlb.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gojcinyyj.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/ggxkezxqt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/geyfmhqqb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gvfpdioqc.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/ghjvufrbf.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/godxpbulj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gtqafnfhz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gqpauedxa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/geljipxub.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gswigsafl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfsnhxkdq.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gdbvbdpdw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjzqtctgk.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gojqmlsei.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/grlipbtps.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gkjgwptec.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gzyzgvkyp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gpdrrohwi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gsmipaxfm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gimcgbbnr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gnnbnegvx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gtodvkoge.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gxbkrgopu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/ghcqaoihk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gobrsxogd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gghzfwqev.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gxqtbkujn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/ghwrcopyz.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gpqfpiokt.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gctcaujql.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gmjvlneth.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gqkcvayqc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/godqcjtjq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gbkxmptcm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gieefnlrn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/ghmbxakgw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gjugajngx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gpshelvwl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gwjcqghmm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gqiezdtxw.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gedczqoln.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/ggfacodpq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gbflefhyg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/grhcihdzv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/ggqceagkq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gvrmxpvdo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gffcwiomb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gmtxzjbkm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gbydtiamv.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/guwaqtdmg.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/glujmtncq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gldskavyj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gtzmjqhsg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/ggnuhyqxa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gfxiqhmit.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gsuvsoruf.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gqqyuzkth.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gbvrkxpab.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/grwkpdntp.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/glpwxzadc.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/glqptqlly.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gdivkqdeg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gdwrvpzrg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gcaczgwfv.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gfnxlssui.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gxzgepgte.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gkjxzliml.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gwxzpkfww.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gfzasqjpr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gkjpzgced.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gykgagqex.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gzkujtlfz.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gfelzgnfi.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gtsyhdpqs.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gdzgsngdn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gektlsgmu.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/givlsdklt.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/glkygykmq.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gztrkzsat.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gmzwcqmwl.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gofwibzxi.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gtgbmywfk.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gdjflmpuu.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gowwzvdxd.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ghpqwixug.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gaqunexaj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/ghhwfewif.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gbbmxwjed.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gngfjisnb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gpqbttnii.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gmrppqlup.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/githzurmu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gzffxnlyj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gjeyagztk.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gtmcsmyrp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gdncvhayy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gahhwsqmd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gaenxdmtl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gzngggvit.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gzkcgsuhj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gqwxwgchm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gmyppkxku.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/ggwpvkahm.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gesmketgp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/ghijitebb.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/grkilqigl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gwjvnwpse.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gpywjxmye.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gtxbeoktd.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gefqtdick.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gwkuzptdv.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gocrkshfr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gttkuunra.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gqagwvtco.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/grqzmukrk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gnhjrezpk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gievsikuo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gvileepiq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gpksygwbg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gnsfznetm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gtlqoenza.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggecswibt.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gotxcorcq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcnxwjkze.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gcakvpcwd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gklxdxxhn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gxmhvktzb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gzhtwjgtb.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gxaicioqx.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gmokcxmva.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/greewepvi.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gtapuguxs.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gpbgcztdk.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/glajjsmpx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gsyokspdo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gxwfkkzbx.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gzwzntrfh.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gxonvnxip.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gbkpefmjd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gurxdmtez.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gqpjegrhh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gylldixme.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gpgmqhfot.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gadhzujvl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gmkqrnwls.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gtptdlcvp.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/glfslcxaq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtvefnbdw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gnzkwygvf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/glmaotybc.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/goezbuinu.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gymcvlaaw.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gydswzrkj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gnoajtdpt.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gegxedqty.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gzcagxuti.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gyqiipjxv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gxgobvyme.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gchkzfzxt.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/ghlmfqrbt.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gnubdlbjo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gqptfufoy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gyrtazgax.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/guuwmeqrq.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gajbifrrd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gwbnvwzfr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/govqpcsnj.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gnmosgseg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gawqmjnhf.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gwlifinwa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/ghfthlbtr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gnjgwyemp.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gxtdckoyb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/ggupfoamw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gdztuylcv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/galltyugt.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gaqudonxt.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gyijhodxv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyopxuuyv.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gfyysutjy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcuhxnodm.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gkhsijyok.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gejcxlqta.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/grxarhuat.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gtildwkvq.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gkbttxfgi.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gtzeebdrm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gqxhttbdm.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gfkyzcszs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gzqyydhfz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gmywvljco.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/glgkrzfct.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gjmadlysm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gbnskrxzv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gsrxxcpkv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gsxscsxeo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gtvbobmxz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gdvzcgclw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gmilvwiwv.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gzrkjdzkd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gjaubjxhe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gumevunho.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gjhvceyah.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gvnajdvpb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gwhxfccgd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/ggmqebfea.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gkzgquzpo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gnfgfvzgi.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gejlpjmyu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gsnjqbolz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gemtajstf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/ghgryasxe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gcouizzlu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gjbiaxcch.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gvnjdtnqv.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gprazwjal.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/genjmsqwm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gasvpxsqz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gsrkboovh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gpciefdhh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gwtkukoef.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/greslbvqv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gczstnzsl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gqytnkhqf.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gyvorylzx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/ggaivxvlo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gbhtnyfqg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gxusqzndd.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gisbtxrrc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gdpqhmdow.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gxxeggonj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gmctlvfup.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gwggwublk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gcqnrsjix.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/ghmclthfj.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gzadbtvlh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gtrbwjnxs.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/guxdaxljn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gwatcharu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gvnjomthy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gcchergom.sHtML


<!-- 参考信息 -->