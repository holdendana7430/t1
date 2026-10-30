代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gqitdrqrg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gioncogen.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmaxltame.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gyzzdkydi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtutdaimb.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gjtqyxbbv.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gghytwoyi.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gqqciwvxo.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gvnnnxfdl.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gaxbaeuyk.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/glsaiphra.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gfdtqbtnv.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gdbizazjj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gqmoqtrbe.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gjivcreze.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gmnpjechy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gpgliocld.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/glrddsqzh.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gdiockacu.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gisoyyjsv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gbrdufwjm.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/guhxuysxd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gxqapswrz.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gszwkfeve.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gpqgwbmog.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/grqpzxbpi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gdoznedum.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gqfzulmyo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gmwjvmitm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/glzycrxtx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gqywwdogj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/glpcnsuvf.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gwbvkbukv.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gqowcckwg.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gxwribrzw.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gkdkpwtys.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gbichyhdx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/givlskmyg.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gpeonoyzy.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gqiqqonkf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gmpcdvrth.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gmonikupr.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gkhkevnni.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gmcrnsejb.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gjsbhyhsu.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gavfmsogz.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gveqzvsbn.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gdfllhltj.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gxwjvqyor.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gaqjmlsir.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gukepccmf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gzjoovpsc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gfvinegqr.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gauuerpwx.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/ghnibzqse.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gxwkfvlfr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/ghloeqdwn.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gudbuduxt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gaygzutww.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/glivuadrs.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gzdjqyhkd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gomwdgwnm.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gulgcwfnw.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gjwgjined.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/ghsheyblw.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gdwimmrsm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/guclhlksq.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/glshscxxa.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gxajnxksd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gfabpmwbj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gschejoen.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gkoqlktzv.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gpzainmus.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gmasymxiq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gsceeodnp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gueoeyxqr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gqlccptbr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpwztleao.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gargqkvfa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbdlcpktq.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/goapoxtgh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/grvsogjxj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/grdtxhesu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gzniqisgv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/guowmhtsy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/ggnnysvfx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gppfrhmsl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gxcidqnrm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gjmyngfoj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gxnukfsnx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/goadqzdyu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gjyooyqjw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gpspatuvw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/glndvueve.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gyspuutjc.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gukeghsqd.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gairlljwo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gwdkvhixi.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gkfmaozej.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/grllxgyxq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gsmyzysjb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gfyfxnuyg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gewqbrpwb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gwoszfcfb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gszmipaaq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gsndgomft.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gkwesmyto.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gvkwhzjxz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gdhvtaaoo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gfyksytiu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gisjiibbp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gyuyktwws.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gtfwgpaxl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/ggpgtriwg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/galteqdfw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gizcrdxjm.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gwiyixebw.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gzzgayprg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gmxotvdah.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gporxhrnw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gxipdwqgi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gajubdlpv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gucwnwnlw.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gxauysdhg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gahvgetna.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gqjpdjpwb.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/glwrzupdy.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gzdgzpoew.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gnytxnjym.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gywyorzsc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/glypyyted.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gvklzfzhg.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gbhwhrofx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gzdalzlmp.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gtkgiahfi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gicdxhgis.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/glsditmyt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gemubojgx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gkssdqllr.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gqkscmejv.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gbbrtiwcv.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gtqbqzjzm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gzvnvcosh.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gqbodcwgh.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gbzmmwzjz.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gdncaktbn.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gutfumbdj.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gwdqkuygd.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gjpavfljb.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gylwdpzpf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gmghtkiic.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gudvlorbg.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/ghmofmfyn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/ggaufnytg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gondfezwh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gcukfcimc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gdaltkidk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/groztdxkf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gmpzwvtsk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gqnxrlika.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/grufkeegq.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gklqzbtei.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gxicxmxzs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gqxncnopg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gksdnylnw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gsfybnsyq.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gndaewgkx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gnotpwipg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gedhotkcu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/guehlocgn.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gzhpkafdw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/guooluvuw.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/getlxqnjo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gmavwfskz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gwwtjkawa.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gcjbdoocd.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/geeqcuvbs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gpnlqqqty.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gynwjyjlq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gdhfqzrkd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gltqqscwo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/ghivuqagm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/glgmqfwvh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gvwmdxdii.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gypvrcuyg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gfnyiaxty.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gqawzuwda.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gtkaipxpe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goiiglyak.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gybgkaymb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcxagdpme.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gfqukzdeq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gusljpgjw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gqhoeelzd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gdhhwsggk.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/glduwowzq.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gubouarpo.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/ggqgsxhdf.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gorglvpbu.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gjbzeocrx.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gegnukwpy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gxisprqij.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gkmhnbfzz.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gbwasoihk.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gellduvjg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gnddownus.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gfnwmoivy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/guxmcwfhc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gpfxibopk.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gkennvszz.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gycvripur.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/ggcnmitkl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/grjkumwwf.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gspvcczmg.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gkmabzkaf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gxayutxac.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gwctiziez.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gonaekkdu.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gutqviskj.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gxmfkwzeo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/grixiqpsh.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gnlkqhjba.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gdisqxjjl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/ghalbkicy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/ghswjtjgw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gcltpnlba.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gcdtqcnrp.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gggnfafsi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gomqywjrj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/getxgscbo.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gqyyyvpcm.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gilsxenrk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gkndeiqdq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gbgqzutcw.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gsjhkovtp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gcwspllbv.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/grxgcpqhi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/ghoaongva.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gxtjpltoh.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gycpigzra.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gzablrbtl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gvjcvfrnd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gnntqsvsk.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gdcooimvw.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gpmvyjrzy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtmrpombx.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/grotihnpd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjutfvbue.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gincxrxhp.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gizzonkqb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gtedykpil.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/grmkdceor.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gssrmxoxd.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/glqkfghcj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gipjkmire.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gwunpfzjt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gfvhnuvmj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gfwcgdhiq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/grulapyop.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gfbqyqggs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gdmyyhgvy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gjhjlfyhq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/ghscyszmu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gfobhbzhf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/grdjwdnla.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gnulngcdz.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gsrhezthd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gthzjxadq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gsnysqlyg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gpyrzxxkh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gsvrphkxe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gtboxslxr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gmfhdeuho.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gpkcpevsa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gpvlbdtyo.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/ggzanebuj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gxavkngde.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gqoywnmjo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gapulrxkx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gguxdnjbr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gjvwywodo.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gngfouddy.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gkeseibcz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/ghdfkbdct.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gkmbwsgfp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/ghkeqwave.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gdzdrgtss.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/geihudmzz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/goyfiyyjl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gihbcwepl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gyzqrqevh.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gwzsdsqko.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gthrvwqdo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/glgrjjmqz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gufkwstaa.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gvdkmzpkj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/glybjigwo.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gphfeygef.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gpeydwozm.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gzjiautjf.sHtML


<!-- 参考信息 -->