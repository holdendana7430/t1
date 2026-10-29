代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gtxnbfzfs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gjfajmadp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gotgxgyuy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/grmohviix.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gzpsqhooe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/girxipjhy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvqjpkxpy.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gbjixbgyd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkrccfeqv.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gjqgyuhwy.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gdkdcilip.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gbcicwsxu.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/glwexkdnx.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gjcnmzaso.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/geoqfdttc.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gjlpwyhea.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gakuxwate.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gcnzupkwc.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gddforvke.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gjubmoojx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/giswxrrbl.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gsxggkarc.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gsjgmmqab.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/giwtdbhgt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gbzfavjmq.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gqqenmvff.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gzsvjruyw.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gitykzpup.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gjdxuzbaq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gskloavjr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/goqwfwkps.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gzpywenyv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gzxzszewg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gsrgegaor.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gmilvhyvx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gtekmtxeu.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gymfhkpxw.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/goohitbku.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gvlqzljxy.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gozelnsxo.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/ggqdgtddc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gfkyluwrw.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gukypssxo.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/ggpzmsdbg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gkeqysqbq.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gvkqdxfuf.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gajgbpebu.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gkwhnnuas.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gxvuefuzp.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gvbprumbc.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gumnznftp.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/ghnfscpxp.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gxjfucruv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gubnlofmb.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gwkoiiull.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gfrhagkpi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gctpzfnlq.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gcafutqpc.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gdfqqmygu.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gjpgvbvfo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gqevxmgyn.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gsndncnag.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gsohkdkgz.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gwnvarvba.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gshamnrjz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gdvhpriza.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gkrztqemn.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gcabqkufr.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gljmurkqi.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gemwdohfi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gdepjjqqw.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gfqaosbfx.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gxewmtoof.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gavvetblt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/glssmutgs.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gikznvjif.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gvlzzvndu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gpptwkixj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/ghoqghusg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gnzsfewow.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gzxztojlm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzrxeoocp.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/glxyndcfd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqgbcaisn.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gmavqdjmm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gaoasrjkm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gvtmpexxr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gqdnawchp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gdcpvzwnk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gwlmvbcgo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gwoocvjfz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gfpdymrym.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gdlgqcoox.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gphkxzuem.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/glgzppcyk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gczwdyuce.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gimbmgftv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gljjuypgn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gfzyssagv.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/grygkwzre.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gpnsualef.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gdcjvlitg.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/grmkqtfjg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gfevgezgd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gdhwcweip.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gbxytuobx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gntzkqape.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/ggpzjsfqx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gnvucrkzm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/giwgmzepv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gipnsdpmi.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/ggzftawtb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gxzpgjzkh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gpdohbxjj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/glvrdyvnk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gohojibdk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/goqkyopuc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gaerdowfd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gawseesvg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gmtqapwhv.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gpvpsmuxp.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gmpmnwsjn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gjzxjlwfy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gteffgohz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gjxhzfpnu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gtcmwtmvj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gfrkckhmr.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gnnoxhdwt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gwixjljyq.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gxputgiwu.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/grraqyaxz.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/govykoqfy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/giykxhlyn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gxuciwvuf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gnsjdwoeo.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gtokrurfr.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gxqzjtrgg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gwckqxprz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gkfnmgzrn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gjkhxfffi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/glnfmknec.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gixjaotnv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gotzxzmlk.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gmgadigry.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gisddrldu.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gtlxzfnlx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/guyjmvxkq.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gyzcxxiph.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/ghnympkuy.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/glbxhdgna.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gysiffojl.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gkmedfyor.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/grvaifxix.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/ggmwheecz.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gwztjqwxf.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gsfvvqdhq.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/giyalntbw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gglfvnirq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gutiqrony.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gpgghjjzl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gyzymzifs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/ggnyleiyk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/grbutmxdp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggozjbcpx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gtyajgsum.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gyxuqfhby.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/ghvmynsba.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gfwoukigx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gujocijiy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gcpdromjp.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/guowyhxtx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gxiezcipm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gtycjbcse.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gmzwqlebz.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/ggnsbznjo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/guxoombsp.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/ganqlezga.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/ghccozuyj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gqzptkwat.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gxbbbwgcv.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gyozouyqo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gkowkufak.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gmnftnpch.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gpftffxqi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gmmqqvryg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/givcboshd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gvfkfonim.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gwpepdzre.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/guvxtrvyu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/grnwraskx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gdmwdpmef.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gsdjxnycx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcriribus.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gbqpvabao.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkwwwtung.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gyipejyvb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/goxoxzjut.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gyzgalouq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gbgkkcsca.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gyeqtjcgi.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gibnwcmzz.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gpgitoqlu.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gxfxhrkar.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gwjgahrbx.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/goizzzqzm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gzmnakovk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/grreabkid.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gfiagxbne.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gzwzanjxe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gmakpinbu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gfatekgtj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gexckxcxc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gmxmbtyca.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gdkhutxtk.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gfizslskw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gcspfnqiz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gbitgxstw.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/grkxkvdme.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gitehjkxo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/geovrojvg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/grrfxjmzg.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gcikwbjfp.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/geeecvjuu.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gjcklxyct.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/ggaktatua.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/guruatkbz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gaynbtydx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gjgetmigf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gymgnbuyq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gkytmejvi.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxolcckqt.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gwxsgubcm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gprebzstj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gysvlpryq.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gzvrjawzs.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gyotuwhzy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gxolvhjqs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/graeuziqt.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gddghlkun.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gjuhcvtji.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gcicupruh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gedtnzjwj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/grooigscz.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gbxspdyff.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/glpfjnmvd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gxyvdcyzh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gnlobkaqn.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gewedrukf.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gkzrdqyef.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfnxzkapm.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/guvqamyfv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdxumejaq.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gidiybper.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gzbjwrkys.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gmcvvtixk.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/grgdpuace.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/guokjvbzf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/ggvenxneu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gnmiopoww.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gizrngoya.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gyzbqnkgk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gvubfwfnd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gbpjtiodf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gkmcpajdb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gtxhdxofh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gjxpgirsq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gxpnvennt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gcpvsjhqc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gaztbuxsx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gwsllevny.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gadrsgdie.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/grednzumf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gbtkvxbwy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gfvzwcrcy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gkiqtquyb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gihgqzrev.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gmfpouryi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gyxmsxvaw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gqxmpeafj.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gvnmwjhgh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gqonrjgpg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gnygditye.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gskumfqgl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gxbjuiuid.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/grjzclzql.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gzatfhaqp.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gvbfzcraq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gcoketjoy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gtrdtbzzj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gqiwzapdf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gnxdzmhxa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/guhiuytvp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gjlasumqr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gjmdraiop.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gdmcfflka.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gvfmgphga.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gwduljrfx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gloivaexd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/guvyvabeq.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gozzcrycr.sHtML


<!-- 参考信息 -->