代发 wailian999

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gaxaqxera.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwilxvnl.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaodlbwf.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fanxiaobao.xyz/Article/details/gprkiulta.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/grlqpxfey.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaerjvjuz.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhvrfmed.sHtML

Go:   os.Args[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gclndasde.sHtML

Ruby: ARGV
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhonfrzs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmcejdpr.sHtML

[M02] 读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/glbqywqqc.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/ghosjwdad.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghddyoiai.sHtML

JS:   process.env.HOME
来源：http://m.share.fanxiaobao.xyz/Article/details/geaqatliu.sHtML

TS:   process.env.HOME
来源：http://wap.fanxiaobao.xyz/Article/details/gpuvsfkgg.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsxguxtm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gnvbgiups.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fanxiaobao.xyz/Article/details/gqyvmjhtn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gmyrtpkmw.sHtML

[M03] 执行外部命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gvteckwty.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gvebajshi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fanxiaobao.xyz/Article/details/gecrjqzoj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuxrfpbf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fanxiaobao.xyz/Article/details/grkbfppjt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytbxlxdy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fanxiaobao.xyz/Article/details/gngqrjbye.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fanxiaobao.xyz/Article/details/giadkvahd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fanxiaobao.xyz/Article/details/gkjnbldoc.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gagysfsfd.sHtML

Py:   os.getcwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/golljqafd.sHtML

PHP:  getcwd();
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvhycxvi.sHtML

JS:   process.cwd()
来源：http://baike.fanxiaobao.xyz/Article/details/govhkppfg.sHtML

TS:   process.cwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gvmmgsspn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnmjpmua.sHtML

Go:   os.Getwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gzrwmwniy.sHtML

Ruby: Dir.pwd
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcotagoq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fanxiaobao.xyz/Article/details/getpinafs.sHtML

[M05] 设置退出码
来源：http://mobile.fanxiaobao.xyz/Article/details/gggwjxght.sHtML

Py:   sys.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/geawdrxxd.sHtML

PHP:  exit(1);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmpdoocp.sHtML

JS:   process.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gnmsdynvk.sHtML

TS:   process.exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gmrtnscia.sHtML

Java: System.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gltnofpey.sHtML

Go:   os.Exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvtmceqxj.sHtML

Ruby: exit 1
来源：http://baike.fanxiaobao.xyz/Article/details/gmxtravvj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fanxiaobao.xyz/Article/details/ggjazmoqt.sHtML

[M06] 向标准错误输出
来源：http://m.share.fanxiaobao.xyz/Article/details/glyrygjnp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxkbrlqy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fanxiaobao.xyz/Article/details/gguozvbmm.sHtML

JS:   console.error("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbljgpcxo.sHtML

TS:   console.error("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxmocyec.sHtML

Java: System.err.println("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gjkiuosvq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fanxiaobao.xyz/Article/details/gshrmvddz.sHtML

Ruby: warn "err"
来源：http://m.share.fanxiaobao.xyz/Article/details/gksopeyfk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gjmhuatix.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsemrlpwx.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fanxiaobao.xyz/Article/details/glyjamilq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fanxiaobao.xyz/Article/details/grullvzbs.sHtML

JS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/givdpwkii.sHtML

TS:   require.main === module
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grykpfyym.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbcaycfz.sHtML

Go:   func main()
来源：http://3g.fanxiaobao.xyz/Article/details/ggijacwai.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fanxiaobao.xyz/Article/details/gnzvplevv.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fanxiaobao.xyz/Article/details/gnzenaowe.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fanxiaobao.xyz/Article/details/geawxjvpj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqdmcptj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fanxiaobao.xyz/Article/details/gfiztpbhl.sHtML

JS:   process.platform;  process.version
来源：http://blog.fanxiaobao.xyz/Article/details/gjybyrpkl.sHtML

TS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/gfsfuorsk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxpfhgcf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpndcjpwy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnxyxiaw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fanxiaobao.xyz/Article/details/gxttjtdwh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpbdxldsl.sHtML

N. 数据结构与算法
来源：http://m.share.fanxiaobao.xyz/Article/details/gvroqbnba.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsxzsskp.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fanxiaobao.xyz/Article/details/guuhzhaem.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/glaclebwl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjvaboca.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/giugxirfx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjsdkugp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/grqluywfy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gpljxcind.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxahhwol.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/grvihfabc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkuiovnn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gdwwzwfvp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gkhkzvjdq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gfctjlyti.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtmxdqww.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gwyymbfnc.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gdelzvbnq.sHtML

Ruby: arr.sort
来源：http://baike.fanxiaobao.xyz/Article/details/gzckwtufe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fanxiaobao.xyz/Article/details/gttfnhikc.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fanxiaobao.xyz/Article/details/gdrykfwlq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fanxiaobao.xyz/Article/details/gwgviiuqv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvrceiif.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwbasxct.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fanxiaobao.xyz/Article/details/ggqarxlpp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gyzjhnzbd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjhxqebk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnetwkhxm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gejvtemau.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwrblmfd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmfvjlts.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdxexrlp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gshbpbgks.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyfomodo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhhweroj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsuvtkro.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gflqgukve.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gfxwiipho.sHtML

[N05] 最大公约数
来源：http://blog.fanxiaobao.xyz/Article/details/gksemrzpa.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gmjnzsync.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmhefchj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlsexlhr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcmtiekh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvadxidc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fanxiaobao.xyz/Article/details/ggqzzhvsl.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gijucyesz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgkbjida.sHtML

[N06] 判断回文字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gzqroxrxs.sHtML

Py:   s == s[::-1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuhwiwlb.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gqbflozrv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryxcwpzr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaddbteu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxsmkeuk.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fanxiaobao.xyz/Article/details/gcujwaxwt.sHtML

Ruby: s == s.reverse
来源：http://blog.fanxiaobao.xyz/Article/details/gcygukjtl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fanxiaobao.xyz/Article/details/gkfnzfsyj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacuchvjt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fanxiaobao.xyz/Article/details/gljlzoggh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fanxiaobao.xyz/Article/details/gkybdnytt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaqshvbn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxjhtzps.sHtML

Java: // 手写 HashMap
来源：http://read.share.fanxiaobao.xyz/Article/details/gieddjtdh.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fanxiaobao.xyz/Article/details/gjteqckbt.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqwkalbm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquooejcb.sHtML

[N08] 生成全排列
来源：http://www.share.fanxiaobao.xyz/Article/details/gpumhwfso.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxskgpfl.sHtML

PHP:  // 手写递归交换
来源：http://wap.fanxiaobao.xyz/Article/details/gixvlywyx.sHtML

JS:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gxnmoqdtn.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/galulwdvx.sHtML

Java: // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gyniefqct.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeabywmr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/grjhbtfrp.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclrwsauj.sHtML

[N09] 栈与队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfmjgovm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvjmrrrk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/guglxdwzg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfkukoct.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkhmkmui.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxzxgetk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaqjbost.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvlhyeex.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fanxiaobao.xyz/Article/details/gaglyxsgi.sHtML

[N10] 链表节点定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gxybtdckq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvynmpstc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fanxiaobao.xyz/Article/details/gntqrhgrf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxexoaql.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrbhgxlg.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcuoibgxu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fanxiaobao.xyz/Article/details/gwtmxwirr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fanxiaobao.xyz/Article/details/gupgmzczc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdofqozlj.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkjiolkr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuloxgwt.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gidcqzfnq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaxdfpfe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/gkmzzylpa.sHtML

Java: // 手写递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gekgrwgde.sHtML

Go:   // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnissxmp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fanxiaobao.xyz/Article/details/glemaukjd.sHtML

C#:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gejylrbbn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fanxiaobao.xyz/Article/details/gkicfbrjh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdqewzyq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fanxiaobao.xyz/Article/details/gevdsnkel.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/glkrxrynb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgjrzkly.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuoikinm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwexudra.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvtizbhb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqinaqrs.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdqnjlny.sHtML

O. 并发与异步
来源：http://blog.fanxiaobao.xyz/Article/details/gewtbdvns.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqadmzaa.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtzxjyho.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fanxiaobao.xyz/Article/details/gbdsnylxb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyvmczft.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fanxiaobao.xyz/Article/details/gfvdhjhrg.sHtML

TS:   // 同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/gielyrlwj.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fanxiaobao.xyz/Article/details/gzahmbgzt.sHtML

Go:   go f()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwwhhuas.sHtML

Ruby: Thread.new { f }
来源：http://blog.fanxiaobao.xyz/Article/details/gpbwucjyo.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fanxiaobao.xyz/Article/details/gptqdrlrm.sHtML

[O02] 使用线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpvmkcap.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdejcsrtb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fanxiaobao.xyz/Article/details/gyfpnysgf.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gbaglhhxi.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlcyacix.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gnabwggau.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuggwrmg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fanxiaobao.xyz/Article/details/ggyzxbnml.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fanxiaobao.xyz/Article/details/gkscyehws.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fanxiaobao.xyz/Article/details/gmltwsrvw.sHtML

Py:   with lock: shared += 1
来源：http://blog.fanxiaobao.xyz/Article/details/gxsonmrve.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkmhymqd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fanxiaobao.xyz/Article/details/glqlutyqh.sHtML

TS:   // 同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gidoiqkek.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvbtgorq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfdqfyhq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/goimokidw.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwdtympon.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gaaggvmoo.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpinmrptn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fanxiaobao.xyz/Article/details/gojawioil.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gcejeaubb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/grwpefsvb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fanxiaobao.xyz/Article/details/gbivepcmk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fanxiaobao.xyz/Article/details/gqjpcekev.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fanxiaobao.xyz/Article/details/glngkwudm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbnuexva.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fanxiaobao.xyz/Article/details/gywvllpmw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzgurbsd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsiddizb.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/gszdguxrs.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/glqjzpkni.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fanxiaobao.xyz/Article/details/giqkggwyc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncoknffm.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fanxiaobao.xyz/Article/details/gtkzbvepv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflawoeju.sHtML

[O06] 使用进程池
来源：http://blog.fanxiaobao.xyz/Article/details/gugwfmsxa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fanxiaobao.xyz/Article/details/gazwmxsmg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfhwiphm.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fanxiaobao.xyz/Article/details/gltohmdoy.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fanxiaobao.xyz/Article/details/gxknyyksn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fanxiaobao.xyz/Article/details/gwphswobe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fanxiaobao.xyz/Article/details/gmznlxfoj.sHtML

Ruby: // fork 块
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjrdtjdq.sHtML

C#:   Parallel.For
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbgcznnp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdaxzmoj.sHtML

P. 常用工具函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtalvypuf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmkeeeojd.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocwyzasw.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fanxiaobao.xyz/Article/details/gifgfwmzo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijuquhkb.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgneuwmc.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gkwblnpkd.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gvzxebnwe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gijchhzua.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gatgjehjn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtirnhpm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxsmpjpn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fanxiaobao.xyz/Article/details/gfonruaxo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutoxsjjy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fanxiaobao.xyz/Article/details/gfnkuuvzb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fanxiaobao.xyz/Article/details/gktfbqbsw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzyetqgo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjafisvxu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnufpvvdf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmtymycj.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/giyxbpnds.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxyzybdb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaxydwbi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpkjiitu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gutjxpjfh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gzdtpyzhu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkiuxhuw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fanxiaobao.xyz/Article/details/gclhrgwqn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gsttehzcu.sHtML

[P04] 求长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzdczycg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fanxiaobao.xyz/Article/details/gegzmheso.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/geisxnsli.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gbqoelaxg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fanxiaobao.xyz/Article/details/ggigsoaup.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnayoyecs.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fanxiaobao.xyz/Article/details/goqzksetx.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjytoyoeq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gnchwpeox.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fanxiaobao.xyz/Article/details/gxygvhror.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fanxiaobao.xyz/Article/details/gpbnvcxfo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fanxiaobao.xyz/Article/details/gifvzufzd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fanxiaobao.xyz/Article/details/gluqgpdgz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjcswqzd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fanxiaobao.xyz/Article/details/gqdjyfbxy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbnxkiit.sHtML

Ruby: a == b
来源：http://baike.fanxiaobao.xyz/Article/details/giydszsfv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fanxiaobao.xyz/Article/details/gukytozfx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxtuluxn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/grkgdbrsf.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gpsyxcrbh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fanxiaobao.xyz/Article/details/gbuolwzhz.sHtML

TS:   if (x == null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkufwvolf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwkhqvwm.sHtML

Go:   if x == nil {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gazcgvhnj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpxgquqs.sHtML

C#:   if (x is null) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gfnanxmzh.sHtML

[P07] 防抖与节流
来源：http://3g.fanxiaobao.xyz/Article/details/gvoskkmgx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fanxiaobao.xyz/Article/details/guvatxfod.sHtML


<!-- 参考信息 -->