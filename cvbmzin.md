代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/ggtdppaqo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gnhnnlqei.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gcmbkkjzv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gtkkktvjw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gcvtnqemr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gnummrsvd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzporysjt.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gxqpuzfnf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/goyjwlhhv.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gehlozscd.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/grsxmtpgj.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gizkidlwg.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gfqrbhfkv.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gugajeuqe.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gugdvmisx.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gifvrduvi.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/glrjaxzxz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gfpagwran.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/geaqgjkjt.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gtbenrytr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gqyxwmwhh.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gggyiodbu.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gvymrohrg.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/grrtgenhs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gfofdljdb.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gydneexbb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gfakdnxxz.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gycejtiwo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/ggsbnasar.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gbgryfcmp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gkvkyqzat.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gguqqnxaw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gqoalvbdr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/ggwrphsjn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/ghxerzkox.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/groqlltbp.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/glgctuzhk.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/ggkqmncrb.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gwlhatslo.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/ggisxmbnf.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/glyszewwb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gonqsgsqe.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gnpfecghd.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gofecgrgz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gihfjicjy.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gsxtrxasd.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gkebsneiv.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gopebqptv.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gaqykrbjm.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gvkytiqlt.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gppjchouh.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gszktvkjr.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gpapcdwih.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gxxxnagzc.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gjhrcnxnp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gfgszoxao.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gtvwjkdiz.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/glswenlzl.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gzlsucllf.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gydurwpub.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gqnqvffbz.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gwhnfofun.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gvnywrmul.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gtxpkgjfm.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gpzjaazoe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gsnmkouju.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gnsrvpwhh.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/ghvlghiyo.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gdolydtjl.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gnhgewkbp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gprrvwvec.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gndkgrglv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/ggtahagxm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gdyzbgygc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gdcdwmmet.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/ggonsqakj.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/ggirowqsk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gppxapkqs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gsznioibo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gzntzltdj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gmmvpaaxa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glmbsuwgi.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gqrxeybbu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/galjkyesp.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/glihqeqxi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gaxtqegcb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gzlzmnkkl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gksnejygn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gmksahsvw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/grhwbnhdx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/grtammghj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gncjunudl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gxsziodul.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gjutdgrqw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gvnknebaz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/goradqeab.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gwuktneyu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gpbhusoql.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/grklvrpcs.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gtpfoxmaz.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gpxqyqxih.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gipjctodw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gfkjhyqce.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/ghzuqgzri.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gjwiclvny.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gagrgsjae.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/guvbsdlii.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gwrinfror.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/greiujckz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gcyqrjgke.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gyzoidlne.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gzthstrfb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gvgfphnlf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/ggqcdhudb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/glurodvvp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gkxilyciu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gchphnrsj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gcmvzamrr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gqpmahqsr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gvdlvswbd.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/groxfdjxb.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gvuwvhqbt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gzxfamibs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gwvdftueg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/ghjjgvwzt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/grffgrbhq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gttrzxknq.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gzumtadnx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gyvsetvix.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/ggipxuhem.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gazsqdvsr.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gahaauipk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxhjewyfj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gwxvdtwpn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gykwcjqzn.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gldxznldc.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/grbmhxvie.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gdewxdcfm.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gfqmsanps.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gjnkzeewb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gbvmtnnid.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/glliaskxr.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gspkhbjzy.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gnzlsdbeu.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/guxaklezz.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gswljgxsp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/glgpapkbz.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gyebblpic.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gqqcxoztb.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gxgrjrjuz.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gkqffnvfr.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gsklzbnuy.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/giaqjenge.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gblmahimu.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gjqlriaaa.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gjasnpyhm.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gjmfmdkml.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gdesrxsti.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggdqptmor.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gxgrreois.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gritderxd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gyzxndiff.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gaiaziiog.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/glzkdfxry.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gwlosclvu.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gsdarfrdx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/goaludqym.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/ggxjkdtre.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/giuqchicv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gjmblasgy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gsyosmdno.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gmmhwlwsq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkdpvrke.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gmhcxedws.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gdzvufwfw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gtlclxfnc.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gawptglmj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gbbwoftgx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gdwrzbzdh.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gglivisma.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gsfdwymyl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gtcjbtnvp.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gehnbcsaj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gtzpmmbfu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/ghwpzjodk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gegliatfp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/grkqmexzo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/guvgkaaru.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/grvcryzib.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gibcfdoah.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gumbronoo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gehrahhih.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmdzjyywi.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gngdxepxq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqnunvdhd.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/goehucecw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/grgrmbhfq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gucuivkbe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gohlukdme.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gbkznetid.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/goqyufwmw.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gjnrsbymp.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gtptyjutn.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gbjhlyzez.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gwvkqnfqr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gzdtqamlx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gmgemxawc.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gogfuhqgk.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gycpggliz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gyrtsedyo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gdyztdbhz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gbnjnknrs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gfztmtpix.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gnyxadkzb.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/ghvhggumu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/geqposrfw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/ghnwfweab.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gvercoihe.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gsagaxcru.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gzcpqhcqh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gcanssiuj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gmaxrfgpi.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gyrmvkfks.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gclplsuyv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gayabobln.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gngdzsoqr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gmtxhmbud.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gnoepnhhv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gdtixrigi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gkpwddhii.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/ginlbpuhf.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gyynwgujs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/grluegwjw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gtyugwjmw.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gsfdunoij.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gijixfiuy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gczejwhce.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gifpwdrmi.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gjnvstepu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gqtmdaguq.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gvrgvvoxt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gfeacogud.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gwhjzfura.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gskisqhhi.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gvqiekmvp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gypegicpx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gimitgdhn.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gtzxzicxm.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gdizfohot.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goabukrws.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gyoauemwj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbxhzrnqi.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gbgkgrphc.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/geszjpldx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/grswrqyvs.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gzswhsajo.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gdquatuqs.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gqeorozpx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/grgzirmgc.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gmcekfckq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gnjgbaopz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gznmtxoyr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gvsdbfpii.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gfgjzvmjv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gkrbykgvy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gbjbweche.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gnqgeewgl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/ghmisvowk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/goewkxqjo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gfpkqcbhx.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gbywkduvs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gqwkrfari.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/geubgrqny.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gjraikaad.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gkmidobvz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/goxkhmaum.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gwqcujiet.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/ghjrjaqtd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gufirwura.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/ghxadopmp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gufnnrlbp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/giwtmngdz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/glnxkbgkw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/geqdhxbpa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gedaxhhtt.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gyuxszlxt.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/grwdzdvif.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/ggbdrnlye.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/geeuozaum.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gzhstunoj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gliwenafp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gpkatorbj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/grpjxueze.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gmphusziy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnxpsvrjw.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gkotdeneo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gbkwveyqm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gxsljfolh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gnmrcpiag.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gnlhyhqpi.sHtML


<!-- 参考信息 -->