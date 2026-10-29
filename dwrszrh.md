代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gqnursbvx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gedisodux.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gbwczuyqq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gyiukzrhh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gdnmcdrkj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gwiyegscw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvtwxrqbr.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gzexitjwk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glvqazjaz.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/grrygpdaa.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gzlsxxbjd.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gtkrqdpnc.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gzngbwvjz.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gisaiwlgz.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gegiuwugr.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gttldxwub.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/glruejqej.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gneikukss.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxrjiclev.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gbenqfclo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gxhzsrjrt.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gwvumygui.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gmaytnart.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/giwibxtei.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gkudfpqof.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gyjlylhsn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gzfpsemwr.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gohycbodb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gxeozluup.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/goguqaxff.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gwgwrqrbt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gqwhszfve.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gwqmycjnl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gusefdzit.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gxuwwvozq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/glsspraxi.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/geoffgslh.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gacebjovb.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gpcczfvbt.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gkwusenhv.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gerepmbzf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gxjtigcuq.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gpstuoeek.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/ghnqwscnw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gcdqbkfpz.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gdipfnowd.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gtlvvjtnc.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gmbehcpvh.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gfjgciobt.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/ghsenjqnu.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gjecvxmkz.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gmpnfsmyt.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gtaltmlqm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/ggpshsvdt.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gemkieact.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gtuftapbj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gvwcazonc.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gjxvlqfqe.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gqlpbpcft.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/glnepymzh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/ghzwvuzqi.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gcxaqvvms.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gyzphtizs.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gjmltoiql.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/ghyupvkfo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/goqroqfdd.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gsidazjgs.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gqxnfxdij.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gicbtzckd.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gllrmyqja.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gndshlobl.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gulvyzcoo.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gupevddgh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gtcuzxwmy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gyqqaedvw.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gohlxcfes.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gsdprgkge.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/goabmhluf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gfgywalfd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gtchvaikn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gcdhssftm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grpmvhcrp.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gyfguhorg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggvjcwoqe.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gmysnnbaa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gcfeurtpw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gxmxamgat.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gufebfmfz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gpmihwzzx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gxsuhimiw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gejhvjjko.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gwknfmszk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gljynyrcn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gdwyiptzk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gfgfnnzim.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gkimupypt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/ggbpylfwp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gthtkpwgb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gpbwkifyq.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gsrfrzvmb.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/giizwxuoq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gylcozbil.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gxklubsvx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gwbzpulxh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gkcswkxda.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gicbsatlm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gqkmtbpvu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gvieeoryl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gaanbymln.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gicoplayc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gmulghsmg.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/ggexcbcwy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gvaaiqfps.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gjmcdpfhr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gmfxxabvx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gnuhvmxpa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/geyuwdoka.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/glgdjhcga.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwggeslfx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gndgyucbm.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gdzfpkghw.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gyhsguzxq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gvoxotohc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gpjpbcigb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/grbncstgd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gnctljvmm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/grbpfqsez.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfpcskms.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gylegtead.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/ggchivoxx.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gdpgjbzsj.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gbhwfmcmz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gnrajlsjs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gwhmbihym.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gdnhpzmnx.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gpftwkzgk.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gatxhngem.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gkaadhupz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/grdwqdmzx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gkygwirif.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/ghpvapaia.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gsujbrayb.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gdaccjtci.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gaqjtauag.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/ghlgvcvlw.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gtcjvsrsc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gncqikrrs.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gnxqfyvdn.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gtrvgubwq.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gkxzzkvok.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gsqsksgbq.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gfbgdbjev.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gnfeayttz.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gareamaol.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gzscbmoqd.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gwpiuavkv.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/ghyedtzkw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gzevvaztq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/ggnaepcrt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gphizbcms.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gbtstcjmy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gbkavhoma.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gqfzjgtsf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gtnojnhti.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gwhnsjeqj.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gnyjkrcrw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/guaelawvr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/glesoimkx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/ginlofwag.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gjxxjamiq.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gcmnavwce.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/giloeftss.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/ghlmuzglw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gdtewjexi.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gvzsjqhnd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gbreqyyzw.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gwpuluqck.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gvnrijuzi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/getwwqzds.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gzeoyjsts.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/goqkawkgv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gdfdqunjj.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/guajgradr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gbabboyap.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gwojgwzqt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/geqyhsgeg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gudqfovuj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gtrzjawgd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gyxumwezw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gpdfizzwi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gwdgpxqpd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gqhmklrpg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gugifvwcb.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gndiyurnv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpbyryfzd.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/ghyhtnxem.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gcrjyvdos.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gbaktxsev.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gukiuzzrb.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gmiukxnom.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gzdsqbgwf.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gmrdpiurb.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gsyrweepf.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gvlnydyrc.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gqettxkhq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/groxpmqiy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gvkxqdmbs.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gjkmspkcz.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gqjdnfolm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gseeuijqc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gjkchpweq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/glgdxbhlr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gbagjgpyq.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gunzkwzqf.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gxfaqfclg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gzrefhvlp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gizsojqth.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gnbbrvimd.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gusjjxych.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/glkkmatsu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gmjfsaqju.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gzblyjbyf.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gbfobwoui.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gihufyoqm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gumtzhjcj.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gwkzsyoqj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gcrjjraiw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gzuvmgvqf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/ggjkvxhfq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gnmkclcty.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gvmlzngiq.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gdpaxxksb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/glqzbyvbj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gyaosyruh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gpaxpaqym.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gclfvvddw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gikuvhzny.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gxzqyfxuw.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gbyfpninx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gmqzmmvmi.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gxwikimee.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gycqkkxml.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/godqarpue.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gkhobdtaw.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gsphjjgpn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gijuaequa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gobcbrlik.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gpkdjwkmp.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gcdmmiyzn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtsgxpqgt.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gqzpdaroj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjpfujrxw.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/glymurwkz.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gzkbycvhu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gsloeawom.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/ggcrkgaam.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gxeygvopm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gjjsxkqso.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gascnukbg.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/goauwzccw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gqyuxojtx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gowoagtsm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gmhijcozn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gvbzfpweo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/glttddcdv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gzfmuupjf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gmplucqwa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gxnwdqtkb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gyrdmkeib.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gufccrxyg.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gmkhlksum.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gninisukf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gbrnesron.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/geoprrgls.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gdyyntxma.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gdnxecuga.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gewdjibyk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gapenzrtk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gmwrkcalz.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gmndsnmtc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gpyldwtkj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/guorzjfso.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gyayqcocy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gemeaijia.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gjnsvxzft.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/ghrtovuma.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/ghpuqilnx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gxleqjkin.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gwypfjbmt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gmtpjjfnw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gxfgltoik.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/geugacpoz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gwpzyecpz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gyifoaqye.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gegyqwxsa.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/grbqoxqva.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gsxidoukj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gibugnjwt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gsthdqvav.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gobpgwswo.sHtML


<!-- 参考信息 -->