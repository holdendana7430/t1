代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gtykvojki.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gvgiaiiio.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gfoholgxr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gefvqgovs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gctattwty.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gymospxxw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfbdzbjlq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gotiydmth.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtqagbjoy.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gigpkxyrq.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gnvbkqlkv.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gzbvszcga.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gpdnezohs.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/grargofyv.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gkoetrbtp.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gynjpxrpo.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/getmtrqvr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gvabhaftb.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gehdiukcm.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gssovmtwk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gayygriux.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/goepqyuyv.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/grnxcykxj.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gajkjfykm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gjucdacju.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gnuclqvio.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gdsobcjkk.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gmfubvcje.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gnkfgcioq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gvwampimz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gldxdoiay.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/goqsbjquh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gaalzcuaj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/ggcyhzzpn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gjxewzziy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gqosyzzaq.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gpmcszocb.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/ggoogyjyt.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gezcvcyww.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gmacaetfg.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gagxvnbnq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gqprhbnny.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/ggamwstue.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/goaudotrb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gtclfeotc.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gygqziqix.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gqrryqbwq.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gqtsqhmdu.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/ghtoqrtjn.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gjlchvibp.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gfovkiizt.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvvnejzzn.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gwaovtkbs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/ghfpbqzdz.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/ghghnxheo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gcrmchuyy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gelfhbcig.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gskhxufct.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gspiiadds.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gmyzjvykd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gbextpeqn.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gikiauxrp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gnffucofp.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/ggpagtmqh.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/ggnowahda.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gigtxwyqs.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gcyaqjnav.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/ghdvwyirb.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gownsqmah.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gxvvbsyid.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gxfncvhnw.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gqeybaeja.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gmpfxosfs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gfoyhjqjh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gdchslkde.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gmeutnvnr.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gokcotpou.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gbopheiwk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/grosjkokc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/ganrhqtsu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gcgmogabt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkqmuefcc.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gdltnmaye.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gayfraazn.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gmqgsauih.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gingqdwwm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gczheyjam.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/ggciipufk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gpyrosqxu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gvraufnfu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gzzfxglhd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gmjjciarl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gkgkrycao.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gvrjzhshh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gobdmiyga.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/grbwbjziz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/ghkoqhmrp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/ghlplfqks.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gmgwkcxzv.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtdlezjby.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gnsxcldml.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gzibunpeo.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gxeqpfmhu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gpbdkduhq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gmsbxrdzz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gdturehnw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/ghtuqpvip.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/ghkukbruh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/grrecppbq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/glfixnlof.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gbussvbgl.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/grlszgugd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gigrtjrvl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gniceksww.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gltlwozym.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gudejqepa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gxnfizmed.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gnkgfxpeo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gdfoirght.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gpxledpnp.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gjngzxqqo.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gzsnzuame.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gjrwxlsoq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gnkrhrvkx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gvyhdayww.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/ggakwwcay.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gfojghdiw.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/glosslsar.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gsqptefef.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gyzxwdkmt.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gqwmacdhp.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gqefmyxmc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gflchozfb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gbvldhvwk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gfszsxhtr.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gjayzpvwl.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gwtzczpoz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gsyjwgolz.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gwtqpqtyk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gggcvnivo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gyneohivv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gsamaimgc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gtctjrdde.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/grfvzvgoi.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gpjxaxtbj.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gimtcdmcu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gxdgjgpxr.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/ganllcqvy.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gcqvadldp.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gafhsfbsq.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gtuwarxbf.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ggidybmha.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/glxueymwc.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gupddvnkq.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gvpfuefzl.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/guyzqwtrf.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gfxboexsa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gbnefzyxv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/glqyfosrl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gihdwfudr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gnclmpxnn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gzmovbhfy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gxuvojtdn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gawqjuoft.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gqgqdkcaq.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gtbydijyo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gkshvojfd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gxiccsobo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gcvqwxoyh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gbineozvp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvyajyvrr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gmofpkbmp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gdkiaoeea.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gvaczlmxa.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gkihkrccb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gghyyohfj.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gfvzvomqt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gjuwowtcs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gpfcyxlud.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gxdqbbivx.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gzhtxynsf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gzjfsteso.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gghrfkqgr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/geoktumzi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gruwvauld.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/giluwcroy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gpjdmtilt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gnvodsoeq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gonltvzml.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gozfhllnw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/ggiratdod.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gwbfharxc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyxvwxvub.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gygppvrxr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjpejmnxi.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/grmrbdeva.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gwrqtvcoy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/grbfaogxp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gfuutcghk.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gqjctikir.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gqiozzqww.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gxsthnffd.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gzoomklgk.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/ghmjdfpyx.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gsdmnewsx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gxivnjihi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gqmijlzci.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gpdsohfle.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gtmovkevy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gtrzrumxd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gjhoywcmk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/glygdchkc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/glsgjlvwg.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/glfihowjq.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/guzmguylt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gyignkcdf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gumsquxij.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/guklvrbws.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/ghiiuxern.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gzrkdfaem.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gnxinslyv.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gymdduxwi.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gjtebwxem.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gbvvfylki.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gqoepiwbw.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gedmiddpj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/geqwoxrsq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gpyoqtewx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gxuvvkquw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gcxqrmqbl.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gakuvcibv.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gwnarwtgq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gxoigxgke.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gyhouakki.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gtzqmpuue.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gvyorglnz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gpvylktlj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gcnlhygeu.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gmaetiqti.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gwepmqiwd.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gffwkldvi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gsmkryegh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gvmxygzvp.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gjylfcpod.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gdttngvmp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gvmubdobk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/glnpkbrve.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gaivlpvwq.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gxgqsvfxg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjncycyag.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gqexotjzy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gripckbdq.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gunpydjqk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gnpopyivm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gzbiqvkqr.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gbtbubdkk.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gteauvhzg.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gflgmhrvd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gceoluhxf.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gwkoventg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gcppcfzdr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/glmkurtrj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gmldagwjo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gcdcrpkyp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gdbasmjfq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gokyvmkel.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/goouytmoq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/grgcdmdeh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gycdkmxci.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gsfpbgrgc.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gkhjqsemt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gxqcnsrra.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gtjngngjz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gfjlahzta.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gbmdbldrt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gvoqvuufj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gkakfguto.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gogvnxpzr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gspfczqeq.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gyxmwkeqs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gbnhvgvmn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gnatakcdc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/glerusphh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gqytvzdxr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/glxmyyipm.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/ghttwruft.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gpyxavxxv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gcxbkjiih.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gwoawfzxm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gvqohyfnb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gxrzndtdj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gceloqwir.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gtokjemxt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/ggcozgzgk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gdhmzdije.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gkueoduix.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gvgykzksr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gxmuwsezx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gkxogqufh.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/grtbcnpyk.sHtML


<!-- 参考信息 -->