代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gpvdjxytl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gfnxckzgn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/ggsktxyst.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gjpaikktm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gqojxdmwe.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gbojksdgy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gqeyfqkok.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gfshxpyuj.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gswcnytiw.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gjeyacocp.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gzmszoidg.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gkiapajnl.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gatmohyox.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gjcsgibpt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/ggjrnvtzm.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/ggplsypog.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/ggiyzuxle.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gsynoeeuy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gxkfwttax.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gcqiulosg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/glfavhknz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gsnmdmdys.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guynfthzi.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/glclfyrty.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbozgacvf.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gdeazfxqt.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gxjlylhjm.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gsyucykpo.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gxnbodhxv.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gjkijvfqk.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gogmtvdom.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gkdtzefmh.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gosndbiog.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gdapkrwmh.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gyfqsgyaw.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gwctysvut.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gdaqiydlj.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gcuklhdey.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gmmopeokj.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gppfkjexn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gdurfpdwq.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gzhhaspop.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/glpizkmrq.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gmkezlqfj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gdqoctbny.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gnkpimpaf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gbtkcfuhr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gldvpxfar.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/goviktagg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gkggmhmej.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gacmvkeyv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gprvsnrbt.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/ggjbsshxz.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gyqtcwjer.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/giocgmfus.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gdybufdly.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gyhpkufmy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gzevxvxkr.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gevgcsdhc.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gsslhhovw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/grzoqvpll.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gjqnpahfs.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gzitkxaaf.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gcxlgzgho.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gxomrutod.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gjctygwau.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gkhckxamw.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gcgpubvau.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gvdbxnlhq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gicenhcow.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gbknlajxn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/grbivoorr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gyvktcezq.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gcahzomdg.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gdvgzuyhg.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gkiooovxv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gvartafnp.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gcqhjsllk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/grwnbftch.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gnoqtkejt.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gxfubbjwz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gcoounzxf.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gnzigfrrn.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gxmuegqee.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gmpqjdlqc.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gdxjmzawb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gubutmnfg.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/geervwibu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gjhcwebvc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/ghfoayopr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/ghnhnvnav.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gmrgyajkn.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gwtyizfix.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gwhnlgigw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gworssqad.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gcvlrkfoj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gfcnwcjgs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzytlmuhh.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/guobufkcf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glpgqhakt.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gdkrazjzk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/grawafrfc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gzjfvlqqo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gynxknvlv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gzfpodsih.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/giozukucu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gcltprafn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gojmcrtxj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/giohiaydp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gsxoszoyz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/grzvjcqhz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gfervevqo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gthbjbaxc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/grxjxrdag.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gygjyijxa.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gsrocshdh.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gvntzarhp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gvlpqmrlt.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gvpdgplhi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gugzrnxra.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gbsyvshwa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gzimozpib.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gicxvfnhy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/ghtnkybcp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gxqnscyhh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gnnkmogjr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gluxeounb.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gzexxmfay.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gzcnqhcmc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gdvftswup.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gcwzigypo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gttxquomu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gbcyxolsz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/genvushag.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gotrjtuvr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gybvuoasy.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/ggqjrmbuv.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gglasbxno.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/ggfttwhix.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gmnlossol.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/giytgatwq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gcffkanwd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gkjwffjtx.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gnaiodoto.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/goqokoeqy.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gghfejyfc.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gogyjnbyp.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/ghoixcdbf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gnwvfvobg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gpkagtkvo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gbsyqcych.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gywjzbyil.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gltjvkocu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gvpmunnst.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gydkjhsny.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gvhvrqubl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gjhmrmxiv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gssojzkxb.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gzvwcycse.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gkhkvfeep.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gsntsrudq.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gxwctsmmq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gznsgflbs.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/glfhcwrss.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gfiugsfwb.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gkwocfnix.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gstxipndp.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ghdlidpts.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gflysoxxt.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gkdtldvlt.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gvsptdvau.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/guyzlmueh.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gjachzovq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gcoayvieq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gihgezirz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gztsnwwin.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gphwpstdk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gyzqbdhar.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gmjoxdols.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gntmxihhf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/golsnpjqy.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gqufspact.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/guezrcsbw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gtamolpzw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gjldxgvss.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gesgeigfj.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gufdyvluw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gbcnqqhos.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/glrcggmfi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gmbqielui.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/glblogywl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gzakcebvi.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gpgbeybtg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gfvntmuqa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gfdxbhyir.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/guzsvyhtz.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/ghniehucg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gyoycfxho.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gtigsgqgi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gjkcltyhu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gbgeoozdy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gwxrfxbpt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gegotzagp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gihofynrf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gteoagzyz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gjnsxxehn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gyhnguarr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gztcmprhz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbudbpddc.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gbzuskxvg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcywbxhkv.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gcpvjsknp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gatguaclb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gnojoghzn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/ggxlwtwgy.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gzhxcovls.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gpsbnwrlf.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gcoxiaitf.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gbmqcvvmu.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/golxrqrkn.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gjeezyrzw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gosprmqvg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gzkqxqjjp.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gexpqipsp.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gzkwmlbkm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gjlcikipl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gpgonrrda.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gddbgcssm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gcuemdzkp.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gcpubatni.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gdlhypjsu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gqmhxxuqh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/goyalsmvh.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gvggohfpz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gwxtadmve.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gaoerltim.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gsrcdkbxo.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/ggphmxdtp.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gmhfgniax.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/ggrytntga.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gihwoesgy.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gnakmcebv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gzqlnujgs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/glmjijuib.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gjjnyfxpa.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/geowqajqy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gyazeftgc.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gfiroftbz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/ggnwthpav.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gjnxbtxsg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gsiyjmiwm.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/goygvixcg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gaykzhiyc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gsscxgxne.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gxurtozmb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/grxwzjgpb.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gzuywiypa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/guscdavjq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gsatylici.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gjebkqjck.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gwjcueoar.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gcelzvjzr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gtaxpribg.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/ghuimldml.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gyrsqpcrk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grzbzxgnt.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gaslabrmf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqgaqsddr.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gvjswjnnq.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gimvpqigt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gmrkrlsnq.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gmxzamlve.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/grlfkarcm.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gtvpfwrzx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gitnqknxm.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gjspnhnxq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gfjhugqtn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gpyxxiyja.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gjmqxfigd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gmuhtiiza.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gztiomhmh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gdcjoxdeb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/geupjhyzu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gmwuwkixq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gvpvjwzsv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/geccheotm.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gvrxeicea.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gfbtvsnbz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gikhewozy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/ghyhkqckx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/ghxtiwkhn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gzfwlzaln.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/guicvowyz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/grjibekok.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/giulnskws.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gjteayuna.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gjhuznxlb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/glayytqfb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gfcqkaunx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gcppxlrrc.sHtML


<!-- 参考信息 -->