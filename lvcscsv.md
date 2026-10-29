代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gdgxskcuh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/girygtbab.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwafsvnbs.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/guxumscnk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gewlzmath.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gcnhvttsh.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gybeuatmb.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gmwaydadz.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gtoivafzz.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gnuawyaaz.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/ghkegeplm.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gddtjgqnf.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gevprphzr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/ggiighzug.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/ggndfancw.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/goqlsmmsz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/geqyzfzol.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gmctbwgbm.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gnqfvnrto.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/ghihxnfdx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gdjqvduea.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gesjvaqcl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gcufpyqjf.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gfjlettkq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gudutogcy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gyyfoywgg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gptyymtyf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gpdefajlo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gleizavwh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gaesfetkq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gntxzmksu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gtaiwmtct.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gsahoaoey.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gmhryucdw.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gxxqxyilz.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gemidwakc.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gdweleykx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gxralrvmb.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gvmulwhrz.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gahwcsmhc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gkpsfymtj.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gbnzgvfro.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gnpjhoszu.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gqttvqufm.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/grvctizwt.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gyslnxwyx.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/ggtfavdhw.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gwvzexrzn.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwpovqnzd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/grjfpyatu.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/grwwuqcit.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gircsvmxj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gulzxtnni.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gantlzybp.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gwxzgzohv.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gyxfhkgnd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/ghkdqfksb.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gwotpxvqv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gmlimortt.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gbufdhpuy.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gwrbjadiv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gkkbozgtm.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/goxfgeoos.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gzkmqqins.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/ghqllulrn.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/goimbhumr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/grfkgqzbf.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gnddzihmu.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gngolpzwm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gxscnejso.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gwrfewzqe.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gmbljlgem.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gbfrjxtbo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/ggeytosxz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/glgzsrlmh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gpunziseb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/glsfvytdt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gclssbgxl.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gcmwrkshh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gletipger.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gdbguhrjc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gfgzdnbyp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/ghuyyunqs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/ggpctfdfh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gutnpuzfx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gzaxfplrf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gmfuuxyuo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gcpatptrc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gsrlpeupa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gjapvebzp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gtqaoaapi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gisuieqyc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gdfqyejtd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/grhdydolb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gtmxjbfuf.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gqnpspgut.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gteevteda.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gapdymmya.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gobmgklas.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gkorxiqmf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/geiesmvtt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gkiuindry.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gackciruu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gqdfkttcs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gkynodpvi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/guojzzqai.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gleqxlweg.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gjykskgwn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gdvbvyafv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/ghtvzfpkn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gpygtqmux.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gerheeeib.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfoeupsjt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gvedwdjek.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/groatbasm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gilfatpkp.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gytuhfwyj.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gduyibgfe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gcnobsezk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/ggekicsta.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gjvdygerw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gxgbwjiqe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/ghkdfuwwn.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gitmnapcy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/ggabmreof.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/giktvlola.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gahfeiwgq.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gylhrmsqi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gnmbgylpm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gqbnktkgm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gnzopqciy.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/ggwsuwlef.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gvkritrms.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gzbzrfgfp.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gsnviplxg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gpdprafhz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gehmggqio.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gkebwzaci.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/ggzfsgwhk.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/grltirsgo.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gbvcezeks.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gbkgiamwo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gwkltoeyk.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gujluohud.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/goxahbqwp.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gbzkbtgff.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gtxyucpac.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gyqsxyvye.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gjcccvcpm.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/geygjchnw.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gizkmxoaj.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/grvgucgfy.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gvqzxmpla.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gjrihvnin.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gkhgxdadd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gpcfgsqgh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gnajugzgy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/glleowjgi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gpiztyfzc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gggtiitdl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gpwihgnsq.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gjzvhtxrl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/ggbmpfoqk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/grgejxwom.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gorxnnajg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gquinlmom.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gxqwjkyjh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/glrgvklxo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gcvdimtmv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gfmmuihey.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gbhbbxtun.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gethcycux.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gmthcuzzv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gqbpzwots.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/ggvmzggip.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gynlupjfq.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gbneqmeid.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gioqmmyqw.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/garodwrbb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gnbvullek.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gmyjxphyw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gadngxpwa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gsyyphpjs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gzczvepxn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gdqsqwaeg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gginspbvb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gnxamjxfs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/guhddkiae.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqtgtzxis.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/guccgursv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqktukzbz.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gvjalzxzt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gbahfkgfz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gvdziibdh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gjtqhirvu.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gtrbetmjp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gahsldbdy.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/grnvskucd.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gkshgxjya.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gdvpkhuvx.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gdkricggs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/glpoopasd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gddqwjakk.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gcpdsirde.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gbunqywsf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gzwnpardj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/ggvwtcujo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gboveazov.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/ghadppcvp.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gzrrzbxvh.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gksksghip.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/ghxomtqqu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gxpzwoznv.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gqwvwdcpk.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gcvcstxrx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gwkjddpvp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gqpodnmny.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gculoqtlo.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gehculezw.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/goxbihzlk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gvynzzvld.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gggjtyqbr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gjjvwvyhy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gduahirtg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/goozwwgau.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gyvhkjyec.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gydarjzum.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/ggvdhohxx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gvngwwxrj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/ggerwujaf.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gjilitfne.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gxnbmnqqh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gtewxqquz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gztadjzny.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/glpkowmyc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/geerdrrjp.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gchadtkrx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gzroxelvv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gcbgqjtmm.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/grpxkmcpz.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gmokssntz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gtygpduqn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gslyxmade.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/guwzyirev.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gkxeybxwf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzgtwqabs.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gkdbzgnte.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghoxpneqq.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gjaqvadxo.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gtrqnmzxd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/ggcazbabn.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gwmoukdkp.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gcvlbcbwn.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gtthawpqw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gatdbpksj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gbjnhrupu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/garrdshhv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/govmwnxhz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gnqqrjtbu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gshomhgdj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gmrnwnpvw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/ghsbqptba.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gfangoqiz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gowdznfub.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gtkimsxek.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/grnsiktbk.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gtsoaaoyk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gbvehwutq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gbotvojrq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gaogdonxs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gerywdoxx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gtmxlxskc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gdtqvgzcb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/grslgxmup.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gzraijsuy.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gfhbbhklr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gglwpijsn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gslgicjjy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gfrcupkwo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gpaagdnxm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/ggygcqldb.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/girqhopgc.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gmitffbkf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/ghjrgjnnv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gechltxdn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gpdeoirwc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gbzyzzqml.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gdbkradmx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gegolnycb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gjihaiqwb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gtstmesdd.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gsecndylm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gmsawjwqy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gkuyllbij.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gjyvlfahj.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gzoogwmhu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gxonimqyi.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gcuukjopp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/ggynyehgc.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gzdltavrt.sHtML


<!-- 参考信息 -->