代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/ggosxmijf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gaqzdvtqr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gxbqfgtxu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gmwlgatbs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gwrkadway.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/guayjakdy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtvhbazps.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gchplaevr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxibrdkbi.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gommirrcz.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gjwzswzlp.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gzngohssz.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/ghvprjmwy.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gbkdnmnee.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gfgobbnka.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/giznqfxbq.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gbeygsaky.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/ggsyvojdk.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/glzeraowc.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gnwmymxmh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gdgtoucsk.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gpgmrcsio.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gfjswprpf.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gowvwihvh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gytprpuhp.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gykflmnnr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gmbapduiy.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gknpfydff.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gfzmwafpz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gtlqmnyil.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gobbqhbnj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gmpaswbcy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gcbhnalyx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gfcfmnqug.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gliwvoqnr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/geryunpmx.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gjzqaenit.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gwznjlqlv.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gmdksldpr.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gkyvhwexl.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gdhfivvjf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/ggchqjuct.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gkhrrmwjd.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gpjyqratd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gicdaufno.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gukafxaam.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gksntpnqg.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gktvsrmyq.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gnxmqfwqq.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfedtjkbj.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gyxseswgt.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gvlbahzpx.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/ggyzywewx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/grntvtsgs.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gjhglksql.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gdnfgyyrm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gfnfugyic.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gwvasdaaq.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gjqovumuc.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gzphpbigr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gsqpmlwio.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gyhihfhdk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gjvxsuglp.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gqtbvfjyk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gzywvyapc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gqroueybb.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/glrushppl.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gqerrsrxl.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/glarpttga.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/guhbalmqp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gbhwdrlwd.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gpgatbymy.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gnbcrpccj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gmuqcsutj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gdrjelmgn.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gricdmkyl.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gqnaqvxgi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gbxpkumzr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gvsiuvvki.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gdlpffgae.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gnnzjbwsh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkqdrsxoe.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gadzggdmy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gscdpfwcm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/glgqayvze.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gmafkugud.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gumikswtd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gkyolkmjz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gosowzpzj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ghytunpuc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/giirrbpel.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gsdxcillz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gcsxqqawz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gxfjtuctl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gaydhwkrp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gfzuvfakm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/grlalihul.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/goxfqybfp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gowkbeeab.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gnygkdvec.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/guhxmvoew.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/ghoimrekc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gesirseft.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/govdgplvs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gectxchws.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gudftlxwc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gpyaiwzcg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/ggkfwdwjx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gwxbuwubd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gnptxvsih.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gnqmpoeln.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gorgjcaqa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gdihqljas.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gveviwzdw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gzstqepnh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gqacvbgwo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/guouaduxr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gzwithtpu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gmercfmyy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gfmemtigj.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/ghfmtfizw.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gickxltdg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/ghlemwxga.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/glvgghnjk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gnhsegvud.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gvvgapywf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gzwnvdhji.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gjmijzoab.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gefzrtark.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gophhtyvu.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gdnupsave.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gdfmtjwzv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gtianhfnw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/grqajkisu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gwnkmictm.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/ghekkvbjq.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gfptndvpx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gzjpiilvl.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/ghckbween.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gkuwgzldu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gmgmzxwql.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gpvhffcgi.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/glntugvlf.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/graalwzni.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gesioppqz.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gbzkxxyjh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gnfinmnlr.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gyrwdtzbd.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gwawmenjy.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/getzaeyos.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gcyyurdei.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/grbuvvrlh.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gjiuntarp.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gddkdwqcr.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gwisitrxi.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gasoplqwr.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gxovvaphe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gyfujtnjn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gtxpfcrvl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gvtbnmxfj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gbnizhmrw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gyyvjjbsa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gqhqioekw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/ghmftddpz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/geymtajrb.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/geshwwaxf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gkzkoewbd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/ggvgoumwc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/glftnikmf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gtekldqyr.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gfxqjdwfs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gmnwognck.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gvlsmvltm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gkdusjffp.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gsqdplxso.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gttxrglyt.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/grkgfaknp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gydmfhwkg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gqmaqqnvv.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gnslxefel.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gqqmiariq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gfvvpjfos.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gwsfauzhp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gvxiptqxt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gjtnqplos.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gedhnpzst.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gvrkjaihr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gudjwgkia.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/ggjuqewcs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gijuqrhoj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/glpuuucku.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gcgbirxjp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbbjpetep.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gnsfromds.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtqsqhdom.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gfnthgola.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gnljfyqgm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/grmyzuhts.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gzofrrxat.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gkymzbycw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gzgrpzcet.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/ghcjtekzt.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gplseqnpa.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/geeklgmvt.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gddhyygnm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gcgxunrpw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gxubjzjwl.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gvstfjgnb.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gofzpwvxk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/giudmosfw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gddpfrzuq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gtuviaklz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gfymieimk.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gwlocwxyz.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gelkvuagi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/ghfrmnlzs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gkykbxqzy.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/guretugkr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gtleflaln.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/ghnynnhkx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gfmvcfumx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/grngclnnx.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gfhcevptg.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/guvdnhaoc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gahmcmfkx.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gayynxpcs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnjmyrftb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gqxxomteu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gijskufyj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gbskljqvj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gdzcepfhb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gjnisacmj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gbgbhypfs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/ggwbkftww.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gvqnbcwij.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gqqkmzyqe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gkvgehkyr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gcdwqkvom.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gwzxiogow.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/grcqqcfzr.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gpicnmnfu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gcvcneivy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gaggwqpgd.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gxpjojmvd.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gmfiqxuvv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/goeknsbrx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gdmuppncg.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gwmrcytfn.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/grozrdsue.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grwoywvpz.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gvplixvsk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcnkuicgu.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gipubinzh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gnklgvree.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gxjzxpzvm.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gibohpmby.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gbbowredj.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gynlhbffk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gxivxmbrf.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gbhnevpbo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gfjxhvvyv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gwqntjwlj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gvjwszxfp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/geqaisxfw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gugcfsjhr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gujfqvzia.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gsugpdhxu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gxhebhoet.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gzxqzazls.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gnwoduink.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gbvazhbys.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gzqxvaosw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gqusgjngs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gtxtkxagz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gixzmquzu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gthedsgmf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gepttbidj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/ggcezndak.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gevrzqjhj.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gjmhbvzhp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gkcejmmyp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gfftcjqne.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/goqdhildp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gnpkqqkgw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gtymccpmm.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/ggyxlqoka.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gvbedmxwn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gpsxgxisx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gmpdufvmg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/glqltnvjn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/glpienamj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gyamwutts.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gezmstlqz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gqnxanjmz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gygxekjrd.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/goklswbse.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gjpbrcgki.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/ggqcvdpyg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/ggdizxyoe.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gjwntsijn.sHtML


<!-- 参考信息 -->