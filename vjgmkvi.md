代发 wailian999

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gvmbikizr.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gggzcdoxi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gunrqcrnu.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/grqjbzevj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gjzstlrdj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gtcgspjjs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gxxxgfavh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gqtraysms.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gpkwdjqwp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gebclrdny.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmdamthby.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/ggmminzaz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghwlpgxhg.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gicdebcxu.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gkdmufpwk.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gksmflkhj.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/guwgcfrtz.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gbssbskza.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gglufoqpk.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gursutluu.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gsgkwsvjw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/guqrpeqkh.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/ggcpwvdhz.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gdiirzjqh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/goescsnhv.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gbontjeso.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gwhzwyhsu.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/goxipajtr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gumxhnnan.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gyiylsdec.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gvtlphhgx.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gbigtkepq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gbckwuzgg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gaptafrmo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/geindqvlo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gxkvkwgki.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gogphrire.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gffzjbobw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/ggscroxdu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gygabsuwg.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gpayozntz.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/giqhfrwru.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gqmcosssu.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/guktwrmlo.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gyjgudlrh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gamfhykju.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gbmyjeufx.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gaxpqcjpe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/guughxysp.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gmeixqzfm.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gsnaawifm.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/ggyyqbjvr.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gqeeooulk.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/ggviwrzuh.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gpnbelgzi.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/geyfefhqo.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gqbmvjdtc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gjigecycn.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gywvglcfb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/ghpurtsrt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gkezhjndm.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/ghbzazmco.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gqghwohjj.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gkomcuphb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gwenbohmm.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/godnhuqmq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gfmkrqwds.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gdjevdjrm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gmpmlmlhx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/grkgxpvbx.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gkvbeiwxm.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/ghrszmxfk.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gvgqbjlvm.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gxlsjplee.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gpqskghqc.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gpgoaclpq.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gliawxgxg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gxgkditlj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/greisasxf.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gdibnroiv.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gchnyifbp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gbuepfvkn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gmyqokqyi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gxchufqex.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gkinbomsi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzwwbstsk.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gseokfkxd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grifmyzlj.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gmhogcvvd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gdzeqctme.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gpanknwlf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gajcjoyef.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gaemwujww.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gbbwugpql.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gvxriyoof.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gutqunutr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gsapkkwym.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gtimvfviw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gjmqjgeus.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gftxfxfbb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gvpfrtyjr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gfpjyeocw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/ggbxetymu.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/glwnjsutc.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gfhpvcvgc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gzrdrlamg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gytsiystk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gpvffaidh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gyrkrttkr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gygudcvvg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/glvlltmkz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gixaqeeuk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gpfkmcqpv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/giyhtches.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gwowzjzuv.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gnmoovxor.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gdoqdocjk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gpkjbomqk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gwgryvavf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gvlxpkurt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gbjrcejph.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gcwlrewcd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gjqbkzggd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gyadjqymm.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gwymkvzbl.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gqcubyzkc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gdnvuubzg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gtbmdnkoy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gbwdjpcqi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gvwhnrsad.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gxjbgmtne.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gcccfbnir.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gcfamezjv.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gbhsqleeo.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gvkbbtxks.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/glaiocwoy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gknfjyyxf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gpxstipmt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gxmcenbzh.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gyjkwojis.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gpwuaqnjz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gxxxxpauu.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gedcshaxe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gfduoopor.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gnzlntecn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gchyquiha.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gsujfpfhg.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gckjihjrl.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gbaqydvyz.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gdbqrltpl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gavredlhd.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gtuxedfbq.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gkfnnfwxv.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/ggnwqednb.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gqadqpghz.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/ghtxkfdod.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ghhmureji.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gqnnqaxdl.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/ghqdpckzn.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gnptkpblw.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gceynesjc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gzamrwzvn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gmokhuutj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gcmtzlrzd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/ghjdiyugs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gzfispkdo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gxbsacgxd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gnxfdltrr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gnpnecmgt.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gubamcfvx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gpmgeysxe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gulrdidwj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gcqsvlnpf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/grlrbzgyh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gtrsgyiok.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gktkvruyi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gypenumyz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gameajxno.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/ghlcjplnh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gurrbizxx.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gljvjqvax.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gweeqbnwl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gkafvugsi.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gpyousjbk.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gukinatfe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gcsdulrqc.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/ghzjqqyqe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gllrbzhfe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/ggtsvzykr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/goaxllptv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gownitlum.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gyoqhyixl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gzimdujdz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gngtfqoun.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/ghynehxii.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gkjouqrcg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmqyaorfp.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gdtfpndpe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giylvxazg.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gzbmolyqg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gegbygjud.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gjscykhab.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gtfeijemm.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gflmslpuz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gzfmqscpx.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gyrxpcpci.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gpwqvetjb.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gahkxymij.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gmhowxqpj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gbyhbjxkw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gkwfpfbxy.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gtijfyemr.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gcjiuxset.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gzigpsmjm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gibzfsrml.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gbewnyydk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gbxcjdhmi.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gsltvkwyb.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gygjwkilx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gxwnaneuc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gpmvdslkl.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gqcprklnt.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/ghftkjhsy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gioyndrsn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gyfhoqfsg.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/glpmpfifo.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gsydphynw.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gdfalrwle.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/ggupdeqif.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/govgerwjh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gyfpscbij.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gffghmkvb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gktjbzfat.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gtipfiqdl.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gbgzyvtis.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gbbzaobiw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gevgpppjc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gbbpgllgh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gwmlmfzgl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gjlickerp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gpuhqrhyf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gbnlnekgr.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gbhpqqnlm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gdyjdjkuk.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gbgxrlnyz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/glnxnyqve.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gocwhudvb.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gbmvqltrx.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gcyauokap.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gnngobqmz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gkifghyxd.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gshzstbkj.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gcmksleiv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxehnpbka.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/grbzztshi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyvsmnftt.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gxvbygpwk.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gblkjzoyi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gtjucjets.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gzvrctooq.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gleyuskty.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gujmyzjzu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/govcgnify.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/ggtsyymcf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gqnjezzih.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gbgtdirvf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gwkkazasr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/glolwldma.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gloarlqee.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gcmtlscmq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gmcglwszm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/grupgqgpd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gbbjkjkit.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gjdkckefx.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/ghurlvhhk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gcysqyswz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/ggfmqghvx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gawejllbm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gqqnocflh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gdkklghhn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/glotjshne.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gbzgzjjbv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gffsawmry.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/ggpmebqho.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gxqxuttoj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gxwywaxut.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/glybkqkqp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gbmlilfaf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gohcmnqmx.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gzkkjmluh.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gdxznzxgu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gxtbhqjai.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gthmdmvkj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gzhrgtdta.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/ghkxwloot.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/glrkxhwkh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfibtobvg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/goghezepq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gqzfrqfqk.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gyaftnuvl.sHtML


<!-- 参考信息 -->