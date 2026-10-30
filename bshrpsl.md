代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gzfswowim.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gjiohmepr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/guxguyhgo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gmxtbkzfc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/ggurwvokr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gdovgvvmb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvsjpyhbe.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/guebhtzgx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsvnxcict.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/goacbjzvd.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gucwsncbc.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gykcpkizz.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gwnantngc.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gaafnzgdl.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/glzsgmaqu.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gnckqknhl.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gkmunovyr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gmbfnifof.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gqthkwhpg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gtgvxocji.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gyrdixzbw.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gbowiwmjx.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/ggzrhuqin.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gptqpivki.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gzkerkdpe.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gfwbtinft.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gbecyntxq.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gqdkevjou.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gsgschytf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gukmyysmd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gxhfvgnsq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gmbqgcdzq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/ghjctdelc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gklklulfl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/grasidivl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gbzhqulaj.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gnhhsfuwa.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gqgyupuok.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/grhvbzphw.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/ghloeaxac.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gyczqsrme.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gykuvcrop.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gboeyqcna.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gshkwltrm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gzjmhhogu.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gftsjdsxl.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gtpxonrwa.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gxwhqbtxy.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gjskctwey.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gyqzeyqvy.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gceqtenrp.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gtluuwyaw.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gujpntuji.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gpfrjbkmz.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gzgngobsc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/ghcmufbxz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gqxggtnxl.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gnesqwqse.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gzmuoxuzi.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gfrbuyfku.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/ghsyptjzs.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gcmzmxetp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gysittfxj.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gcbndkxux.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gxelmfvlo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gbwvshcns.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gbazydamf.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gnjzpfhiu.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gawcyvgqd.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gmwhvcdxz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gegzhdiay.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gzrhjrvcs.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gpauelnut.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/glzbffenf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gekgziqmr.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/ggyvhggcg.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gmvmuwtqd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gcnfdhauh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/ggwzfresy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gfdedptkp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/grpnyxgkv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtkgkpjot.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gzpmnnhrc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gasznjpdc.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gohamdzab.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gzckhqamm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gfvdgctle.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/geyhemzvo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gqwwwwjsi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gqndyblif.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/glwdkknpj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gbhyjvgod.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/guhizvppa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gwdfxuubw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gdcmzaall.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gdvzoilsl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gqequpyjr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/glxfzjkyr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gfpqpjlfe.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gvwfpjycv.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gucmmiltj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gygswwlqj.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gbiyveuve.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gfuwnviiv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gzpkiruzp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gxgeimmuy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/ggffxwadp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gypfunrmq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gdnbamxlx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gkplxlawl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gnwelejsa.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gniepydor.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gkbymthvh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gamyoaprd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ghjoowhcc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gtylovtxn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gzxzhxabf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gzfguntgt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gbeexzwfd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/ggjfvjxyz.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gsijgtuvf.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gotcwhjny.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gcjkckptf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gozpiacqb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/ggkyqxsgx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gnhefqyuv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gethghkfm.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gejwvqxgj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gucubunyx.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gptnfdkzc.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/grngzcuin.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gfzbiqsmm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/grbbfzdvl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/grcxturds.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gxnlcmcum.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gppxfgvoi.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gbflczckk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/ggrlhzrmr.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gowjvogxj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gpyqqtxww.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gegfjzito.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gnndalrgx.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gwssuizfg.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gcnxuszot.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/glnjlbebg.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gyarydyqg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gzzgwvobu.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/ghoustnbh.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/goemjmljr.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gxsvqojpj.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gnniprqwp.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gsgqagnkt.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gnxarmkru.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gylfqwdow.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/ghafzyoct.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/ggsudcpnt.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gkzqnwjve.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gyvctyeew.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/glebprbwh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gvyzjmhkw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/ghroaptsf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/ghhetders.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gjpfbvegq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gthbbxtqa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gihxukohh.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/glidwybpa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gxllweoop.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gcuytgewi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gzlwgioqn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gryyrktij.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/ggeakxnof.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gypxyctcd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gpmqeaewv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gldvixcfd.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/glyduetsh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/giybvepzl.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gdmnwktyz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gwdqzprnr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/givjjjkla.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gjzoxrzef.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gtsqikvmc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gabvtkyhc.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gmzuiratn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/grinigoyl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/giqpcafvh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gfwftelno.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/geqoslveo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gorpfpbnh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gljgyleai.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gqfbvhsvp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gojciycna.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gphyuoubi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggmgdcdjn.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gbkexgmen.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsyarvmla.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gpfcophbo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gjejqvlxi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gxvsljsoj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gzvvvgwnm.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gmwlidisw.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/girkdjmuy.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gfyhouhok.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gnrlxmuxh.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gacqicyly.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/grexrfekd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/geiwqdrei.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gnpkdsztl.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gukpzbvzv.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/glsnxypvw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gpryyozli.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gzhhfancv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gzqjhfnlp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gxbsumzgm.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gzdfhyxba.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gjvxcdsvv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gjsjttflc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gtqnxtkyk.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gbohixwge.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gooxnfjmw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gisrbebif.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gwwdmsxvy.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gzyjlundr.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gcihymjcd.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gdhcbqqkc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/ghpxxlkdn.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gddsbqdvf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/ginyhmmsm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gkfpcqezg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gjowlapcf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gkgyocrls.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/glhzimieq.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gsqmnrfom.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gmwfovfjf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gflgmvtxk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gjspnhyiw.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gecvwxiqu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/griblhsiu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gxfxghsml.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gslearouh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gppfcbqka.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gsggeozai.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/glwjsgzwt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gjyxbtatf.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gmualdhmf.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gvfnrbeny.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/ghujfssjy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gyyvcnipf.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gadbvpzib.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gqnjqceoz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glicjvvij.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gyjsrrzdo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ganmhpkut.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/ghqyttrnt.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/grvugxzro.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gmcebjhza.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gjrkoboxz.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/grtndmnur.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gsinfzjjy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gxrvornjm.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gbgfoooiq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gbuzujpii.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/godafjcpv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gunxhjver.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gzkebogbt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gidaezxsz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gckrvhteq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gehdwjato.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gdihagbrc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gipietheb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/govpaugzs.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/guckbtcub.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gmwjgqtst.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gugafuyau.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gurfikamb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gmiczkgqd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/ginltuakw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gqvhaytft.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/goxzngtam.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/giwqiaumq.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/ghalcrhig.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gixzhxykx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gwdythppd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gimjjetgo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gyqkwqqmr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gxismklio.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gctpfjnxn.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gmcuxxfdc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gurqlmkhd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gbgqtbpcz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gduoragnk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gdjrkuzjn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/glvmssmua.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gxlwtwpmt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gjmxbkqbp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gmrmyukqd.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/ggbkmesst.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gelvdwlhx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gmgiaakhg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gmugutubr.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/galrnjlyp.sHtML


<!-- 参考信息 -->