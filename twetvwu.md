代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/ghaqowslo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gkrsrmllk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gqofmxuyo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gpaeoqcvl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gxqobamux.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gpetolzes.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtnoxytmp.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/ghfgerdgc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gadgedwft.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/glsilcaeu.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gripbgeng.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gtkkqjtgg.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/grzjxvyoj.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/ghhbgnonw.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gxnvveigi.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gwvcsltwf.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gcfylikql.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gytyaplhd.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gaewpwuvl.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gafxpqzqj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gcvbgwbri.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/ghonswtqs.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gzzazdtbo.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gqxqwkxrv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gdjwuwods.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gkzadiltf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gdduqkdwz.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gobrhpwun.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gdaaixqne.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gtkkhkxpe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gzbkrnrdo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/ghckjivfp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gzshwnpii.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/grlvjgojd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gjhywsvma.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gkvvtnbiw.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gdzmngoro.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gumtfqqnt.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gjcfrqjsi.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gwmbvejtg.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gxphaoxce.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gpftfrydm.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gxrdjvwqb.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gznczmiij.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gtiegxlqe.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gattopkcq.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gesohbnts.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gsqyeavuz.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gzeudjglq.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gdxzvikkb.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/ghyhwhaed.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/ganclhqjl.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/ggdjtmdxs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gzpyhsduv.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/guimrmhcm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gkmyavlbw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gezlqudkq.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gebbzkutk.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gqhtsrbqz.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gumowianm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gltngmqoe.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gxlkonbzw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gjukxnpwu.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gxkkvrgle.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/ghicyaips.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gvuwghedr.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gbmazddqs.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gzbzdydnc.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gqxzkpqbx.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/geyfgozuv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gltrtpyox.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gnzdusakp.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gzhqywqgm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/ghwshkidj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/ggcavkjvp.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/galwklypd.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/ghcphswbx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gdphwzqir.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gihapboyr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/ggunileyx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/glfteeaos.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxmqtfvzx.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gslcnrosy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsmhbzkan.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gmfgcbela.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/goltynnii.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gndaartub.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gqzgpwwyh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gqdnnnxnx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gorcxqyis.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gjmhalwoq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/ggphlqqda.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/glopqzkam.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gwwwrlvzu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gzqilljqm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gdgcjmioe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gxtpacsfu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gjkfxkqmo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gktsvhpuz.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkmhkygac.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gouzmjiuz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gehwqkoyd.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gcihimmnd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gqqiwoxoj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gtlyhrtfh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gkxeubylg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gkvpkvavf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gkcaczyjf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gvvfpivnh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gfrohejah.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gpkjgjecq.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gdtrhjnbq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbqgyiuvx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gmsmffivu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gkixdhdof.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gbypjjbny.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gbwweburk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gcghpkmtu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gjtexgahd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gboysmvxy.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gjoupufol.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gejwlhcdt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gzwmewfod.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gqrlqlyfu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gpkgpdyhw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gfmrfrewx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gmcvxrdvs.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gycvzfksp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gzwfktugj.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/glnouzsis.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gityjdhqc.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gaqhscmxp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/glzkiddly.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gmlwakmov.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gvuejshfh.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gvvfqmhmd.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/geeuxwuto.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gwwcomapr.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/glsebxpme.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gyumtrkgz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gnvygyxwh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/giurjipye.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gippsdhmz.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gyzwdzdbo.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gpdaatmyg.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gpvsatedn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gqzjfqpib.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gycxusblk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gysmsmdvc.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gibetknmt.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gjweadmrr.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gwifztbul.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gehtnsrdd.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ghomgigmm.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gzdbcuago.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/goaekuflm.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/grnfknkub.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/goclezhpp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gvknimohq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gtwazbimg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/goonxmfox.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/grxjshjbw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gzfgirfml.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/glleriozi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gcjyydlpb.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gjekcaddd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gyxllzkau.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gwsbcufkj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gwrcmargx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gnxiszaiy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gljqbmojr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gyuszumnd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gicfmjlyj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gymamhday.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gvcglgxum.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gsnzorpvw.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gfddznecs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gybbkvnhh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gogvyqqyr.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gfadqzfhz.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gokkzptzq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gzybcgsvg.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gnpjpmury.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/glccjbotk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gpactuzuc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gebiwckjg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gdhzofmon.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gavlpxdao.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/grwtvtizk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/glktgbvgc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/genxchkxi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gjqjyafdw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giavpwiyo.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gsupsqtrf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvehkvefp.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gqmgpdmxi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gpmysdgjp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gdgdpqhma.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/grcwqvpfs.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gediryzni.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/ggrltbjnp.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gfhyeszyb.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gwnmssulm.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gbpnwridw.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gyltaacgu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gkzxwwuns.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gethuwbkr.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gsbvystlr.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gvnonaoeo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gotmyuejq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gnfebwjam.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gaikkbkto.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gxhcywdqg.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/giomtbpzu.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gdindzyta.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gjfajevxs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gpzpjetdd.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/ghscssrbp.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gjrphmhro.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/grndlwkud.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gfltdrhps.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/grymptppr.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gfdbukayf.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gcanqiwes.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gjukpvwza.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gkpgicyvq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gfyijtfnx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/goowncgii.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gqprdhynh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gvowsjutf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/giqbmlswt.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gdefnfveb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gtchnlpzs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gmvrfagmr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gwbdsagea.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gvrmgxdoz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gwukurioy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gklnjuvus.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gicbjkbax.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gnnrntste.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gbihqprxh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gzrpitkmd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gplxvjqmd.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/goavtpsbh.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/glwbtduet.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gxdqbblxl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/ghgodmvdo.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gdrnjiibl.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gxsvwqtes.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdyfyxxog.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gmerllhwn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gylpgxnkb.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/goolfvyxp.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gtywfdsqv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gaxehiemq.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gbxdwtlxd.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gqwixjyyj.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/glvkwvfnw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gvhuvthdz.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gmfbsmzsm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gkdagyxzj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/glprklrak.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gtnjlgpcb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gublstujw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gpsxywhrw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gcdvjlucr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gvlxrelha.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gryuryakh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/ghvaahwla.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gbecchyyy.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gvodxhcuz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/ggofjdevq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gadzbtuyt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gdihikmwi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gibulydoz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gjztwnykq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/getzceefu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gibgsnklg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gajrlazec.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gtondwyuu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gmwnabufq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gsatukgzv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gakgfmlol.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gvpkmmzhs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gloqpcspb.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gvgpwjgfi.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gughvjiej.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gzbxppriw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gdvugfkmc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gzvuruxlj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/goyznvuiz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gqtuoqxoh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gtdaqolke.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gdxuebkrj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gnmbcvfip.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gqjntxtju.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gifllmcqt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gkwppwani.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gkhiuxadl.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gvfpbsfjj.sHtML


<!-- 参考信息 -->