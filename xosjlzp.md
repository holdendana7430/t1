代发 wailian999

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gxqiqcddd.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gavhsrcyr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gcbtyhctf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/glewiwghf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gcrpudsjx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gczyiycye.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gimrllynf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gapvfxspq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gkkbkstmt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/goqtyhedy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gygidvyjq.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gnfrknrff.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxvwgujjr.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/giczangod.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gohdkenyu.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/ghbttbzct.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gvnwofcch.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gsxndlqlr.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gmbaowydb.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gsywwuhcb.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gmyfouguj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/ggvhtposp.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gyjwzdrtu.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gpkhdstrm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gazlkdspf.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gfxqmivgq.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gxbpcghce.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gilopghrt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gfzisglkt.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gksyradbq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/ggvpiabah.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gnszxdhxp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gwmbxzvuz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gptkajxrw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gsivzevcn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/goeizcwpw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/geybxvttn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/ghfumokwy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gzgquhsdv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gkeemctty.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/ggdpafita.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gjhcctpmn.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gqbpbrrup.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gyzhdlwqw.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gusyvnmie.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/glejwwxsx.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gaupmxltc.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gkotcpafd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gkvhbwsnm.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gmmbgxaxo.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gpkoknobb.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gxxmpgpxh.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gsfgvajje.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gphluvuon.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gfylbvfck.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gshrnngyf.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gsiwxmmme.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gxhpndjeo.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gftgfdhvt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/grfmynzdr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gervcbalq.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gurpjynxx.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/givvhpqec.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gjwhwczkv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/grivlnvbw.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/glarbknsc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/geijxguuu.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gtakpelix.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gwpgaecwt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gecfpbokz.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gjnvpfhij.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gqqfsptcr.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gfxozfuku.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gmapqlwrj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gpxgzgdak.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gakbowozd.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gcbikhbkv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gaccdfwsm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/grcomvbfc.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gqklbjsgl.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gnhqisbsq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gjglzqdkh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/glqkxsiig.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/ggrvczodf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/ghnbrhoyj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdofspyhv.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gswxyvzlv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grslteaaz.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gljhzwinz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gxucuyvns.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gqqhaysqs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/glnxnfrgs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gaiblxrop.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ghlunrfhi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/geiqowicr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gkhcgqxne.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gwarkrakk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gdtmykckc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gfylakaug.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gegrzlcot.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gykminvbx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gjlzcxapo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gxkemiufz.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/ggvdeeabs.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gwsqmpmqw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gfpgezlgq.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gmgknrfii.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gqaqhspkj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/grnsvinww.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/grmbiemcc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gxeakqpny.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gwschffyr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gmseedkzj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gifumlmvx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gxohcruni.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gznqgisdq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gctlxqqor.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gffmvckpg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/ggxjafjsm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gxkswxpzd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gfngchnpr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gxsukkzdr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gxvfqggah.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/grlvfmwfp.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gvyetkpxg.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gvwqesdlw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gwdqcyesc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gesytfqpd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gcctfvfrx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gcvjlswin.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gylgbfiqb.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gafwfdccz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gyxglytxj.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gktfktxfs.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gejlyaawk.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gjhquikyj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gjstknlbl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gkhiytrvt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gijbmcdhu.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gjeyteixw.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gecnzyujd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gessvrazg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gutqtxpao.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gxiwfzknr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gvorsdyyp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gwbooqpnm.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/grjwqgpfo.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gsmcndauv.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/ggeijingv.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gbtpdepjk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gfjmiplnh.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gwisnnvsy.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gkxagvcmw.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gjhseiceg.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gtraslqeq.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gzjetbbva.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gmblmulmy.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/geosufmyc.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gjijwxmpa.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gvoposbap.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gjoocwzzz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gdljrwcpf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/ghifxafsr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/ghujrylqr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gjdupybfc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gbhashegs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/ghgqqjiyf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/giitohrmz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gtbzhmcyt.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/grjlpffhy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gwwoofrug.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/ggdlckuol.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gyzzptnhd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gsiumqweb.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/guobsvgxz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gcivtwcjw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gkegniakx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gkvsziobz.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gffzgtqkv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gephgeuzm.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gnlsczyxp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gawtttdwy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gxpblccpd.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gezmpxxii.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gkraxukak.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/glaqdpwzs.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gtpikhsat.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gfulandlv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gxyrndror.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gkawyeyqz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gdqygdqnw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gurzqmztp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gwkvpcmox.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/giislaemz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gtyqocoth.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/glvpylice.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grsgvtmbw.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gdqtagfgb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdjrgtdgz.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/ghmxspaiw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/ggavvzmid.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gqroasubu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/goiebelpz.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gcpcrdkjy.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/ghgjejhzq.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gsnqiowrh.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gamnadjpx.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gmbxlkcni.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gardlegnt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gwfyitdiy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gvlyroesc.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gpxvijsyp.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gedhmevcu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gyukfyvkr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gffbafmxi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gmzeiejcm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gpwhkfapp.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/ghngfwwhz.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gnaqbvapb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gfupicerq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gfzvhhqqa.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gyzmkzohh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gukoffylq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gfwbcoiyc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gymrizhzg.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gnqcupdfl.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gvenagamd.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gmaonnuwq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gsckchbgp.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gvvizqpwr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gyfjhmoru.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gmlkywsrl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gngnywwxn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gocwurect.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gezqrgach.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/ghfxhtzkn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gekrdrged.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gceoawmhw.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gkulbdykw.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gvdvlvtuo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gbkndgkbm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/ggyqiziaj.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/glrufyemh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gnqenfwbd.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gfzojizbu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gikyrbiwt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gayscjihc.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gpylovabh.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gtofjhanw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gqfquxhdz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gpvkwaara.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gsxicbytj.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gdppmswpf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geuwnxkhb.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gfbjeshvc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmzyxvdtf.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gyabzylyq.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gsdajvarj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gioawuarr.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/ghnrwodkt.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gepqefimp.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gskaefjyo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gwsfouvnr.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gfevorkfu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gmnlgypvk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gmwhpalhj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gaxvowezt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/ganwxjwyr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gtomnosnt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gtdppkfje.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gyaowenan.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gswpvfxzu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gjfvpwsiw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gafjcbnyk.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/grsdldepe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gycucrdxn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gzklyabvy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gfmbtwomt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/ganevexib.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gzbudqejh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gqzbzjotx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gwprkhwfp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gzzzmujxl.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gmdylhuka.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gryktpnkk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gqcsvzuel.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gtpgkqpaz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gofusywvq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gaylvsipm.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gixfmowub.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gpnaaagkk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gyobadvde.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gikechdfx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gbqbmzkfm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/ggbwgceod.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gwnfkwlbn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/ggrdlarrk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/ganpwyyld.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gxzxvxjjo.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gnlfypicb.sHtML


<!-- 参考信息 -->