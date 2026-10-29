代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gjszmrtaw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gfgjenphx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/gfgiaqfcg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gocgywcvt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gwxtdtctd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gbrbgocen.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzzpotdlu.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/ghofeyrcf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggwuutjnz.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gbnfvbtlj.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gjnhzjuiu.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gdhhwgtaz.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/goffllryd.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gwjtztnxs.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gyxyzmyzf.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gtrgozxmh.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gwdxskgkb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gzgyagyoy.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gtmsmzocm.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gmdmsrsme.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gganlwsci.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/geqhfsxtq.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gntqgrshb.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gxvmkxzof.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gohzybpzq.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gltwekcld.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gkrtmzahe.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/guwwtlxxr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/glkqadwsy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gsdeokaje.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gzctqyptd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gboyqfihi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/guencmpde.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gxbpsoqfh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gujqzrqcr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/ghaxaaqnt.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gzmnfzwhe.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gsxxlknan.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gpcilxtin.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/grosfpuyb.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gznvmmbhv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gnnovguwt.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gspmvvwkv.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gimpmfnzt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gbduiugsj.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gwymisqno.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gcpxjrcst.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gxzckipcd.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gwpujyqjm.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gdsvxxnrp.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gotahvfud.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gwpmzjzyx.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gciielwxn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gsxdtpras.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/glgqsomzn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gdzsjuqfw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gorwsjrsk.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/guvlgnicx.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gsihvvfbs.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gwcdxavab.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gwmigvzhv.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/grbfksywx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gqiimfyjg.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/geoduswfs.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gatgdeojp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gavtzoppa.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/galjtpwbo.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gntptrdth.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/guwzrasod.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/ggdczbjkg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gvefrcfbf.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gsjqsrsht.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gnabcohdl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gotmpcols.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/goawptscn.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gssgqmdjp.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gfxnocxfw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gmfnpkipt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/grjriqzeh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gkwgonidl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/glcqxezuq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gimaagyfj.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/guqfsdfob.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gezjxdjmq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gddwsyzij.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gtawgllba.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gnddqhqad.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/grbdbguma.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gjpevjxyj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gzremzmde.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gmbvqtqeq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gohteiniy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtodkmeyc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gtaybfzmo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/glsrahxcj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gsfkwtwpn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gdajhmkpk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/ggvhdjmwa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gjyfuhqta.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/ggdduefvh.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/glatxfvkl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gdbbectou.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gmpdapnpz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gmgetpocs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gvxzbtaqo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/glkevilgz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gkeglzdpr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gumbixcph.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gpottyenl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gjzedkrnh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gwmajmsiq.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gidfuwkzo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gwpbxerhm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gcleolnlx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gwqcbwjbb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gtzypphsq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gkdzauogk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gsdiiuukm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gduryfzxq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gzkuarede.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gliompvsv.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gvhsauqjr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gipmlqvwo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gqplmpfop.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gygyjrvcp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gbjwppmil.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gkqdtwkdr.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/ghrhupkma.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gvpdmpbpd.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gvtsxrhzc.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gsnezjlzq.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gitwhnpcc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gloqmkopq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gspxuxnkl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/grqquehjh.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gzucogdye.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/glekihhnt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gzokgrxhw.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gerixdenm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gdebqcgmw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/giuqkroxt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gnqloehsa.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gwuupvjtd.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gfzathgvi.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/glxggnubz.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/getqefxnz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gcptnyubb.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gitopbdvl.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gfcxstzox.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gitubjuqc.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gnbdstyta.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gxkrmjcqe.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gbslcualr.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gnwqtdwhj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/geacaedxv.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gdbuvmuyz.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gpjnptjsz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gucawxebd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/grlrmvlsv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gsombfxpa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gpyjjeulo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gxbnxqnku.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/guczwxiyc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gdupfawbg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/geypasgjz.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gytfnsmtv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/ghbdiseut.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gdygwmzry.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gqmfgelxo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/geelvqmof.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gypgodims.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gglhbwygo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gozvqvgni.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gzdzmrvkm.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gzgbrqzyy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gfdaavgni.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gadcpxfpz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gccrrhzri.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gjkmntmhh.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gqxhrjzrq.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/ghuwukgqa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gznmzzdew.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gbwdwkgjp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gbqosadjc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gbcooakft.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gcxxpqwjq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/ghofymofn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/glmthqzgi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gbjmoldtn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gknndnfwe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/ggmetjpvq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/guyytoynk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwtorypyl.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gzjiywndf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcordwssm.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gddtbffsf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/goeciopdx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gubvtqacn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/ghdqvggpu.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gddsnjnxj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gzsitefxk.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gprohaopq.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/glytqpyqc.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gozhdswmp.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gbjsktwvb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gydpemmcv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gwjircyia.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/ghvdftmoa.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gpllcrfaq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/ghhakycda.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gvpmfrfov.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gtuptffqi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gkcbickrn.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gqcxpndzs.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gpeibkazr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gtdaaiogq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gdwkoatpi.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gvvnqdxog.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gajtdcfyk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gsnjbcjfm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gdumwwsfi.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gcencwuxo.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gbfhmvljs.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gfijcbgwm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gdjjbgcdd.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gkvdiqjow.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gqhjapupj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gxtguexjx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/goevaaaln.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/grebkqmje.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gnhvqvlcr.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gngghurue.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/geilfggau.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/givjegxqm.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/ggbmiekuy.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gcymqxlek.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gjubtcrvq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gpzwexdvb.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gxexcyzyr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gbzczipvd.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/ggjuitwoe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gccfuvfxy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gxcdgcwuo.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/giqepclzu.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gbqumcqdf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gzapszjlg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gvbrgoteo.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/ghjjdoqps.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gtnooigdh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzuaxupye.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gfdncodqu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwlqewrrk.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/ghamiepri.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gxrixjvbm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gpwoonzti.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gbqnfrril.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gtkxroncu.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/guyxrnarz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gzmlusoky.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gttwkqktl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gkimtgrvl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gvarytczz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gsaebuizc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gktmxsnnw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gsffxlvir.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gkozlblmn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gvkmvyvai.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gnnwzopai.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gkcwfajff.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gqddceadi.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/grlfjktiy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gnlmnafwk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gtgeogixu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gkiolcjkp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gqqlhfigb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gbwomxyox.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gevigxclm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gkpnucmcg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gwtvpffnv.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gcknwlhei.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gixozpxbk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gdxcfnnqe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gljskxngj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/ggqguqdat.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gypttjtgn.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gtazlvofd.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/ghnivhvmr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gwjygifld.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gbynsksnz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/glyinvijz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gxjorvhlf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gpuzvrwiy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gtojvlacv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gnsquwmdc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gjndsqrlj.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/giaukjdrz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gdihdyyhk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/goixujvgx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/girqqrlit.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gcsofigho.sHtML


<!-- 参考信息 -->