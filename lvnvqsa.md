代发 wailian999

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gotqkbfep.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gakyqpwwa.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gsnpvrxwf.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gayflimcu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/ghzoyffgn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gkfeggvge.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gmphekxcx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gaqzwisye.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gecgdcgaf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/grebsksdo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gdbkdtzwq.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/glazcbtyt.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gggxvhrgt.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gbuaeykdp.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gwaeinvla.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gscslcbst.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gvircwwxf.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gnqiopngj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gktkuioiw.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gakppceve.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gxhyrlfdm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gbqavhknb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/ggvientjp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/grydwolvo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gzxatrwfb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gxphpcjre.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzbjgvjpx.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gphoadkvy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gauwwjfgx.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gzlvaecey.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gfaqimmgd.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gfxpjgrxx.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/ggzovpljt.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gjxhzmtft.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gtbkrbted.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gxavzizki.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gqmaucdsh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gxlrvbrdx.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/givnktiuu.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gyesekiux.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gzhmapmyo.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gosugoruk.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gsqqxwimb.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gipzbdeog.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gscnypcbj.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gvroophup.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gmeuqqhub.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gcflizqnd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gytwborno.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gitzgstkc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gcyguqxzp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gkjbbrlxy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gyzsodlno.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gsfgajdca.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gosensxez.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gwaarthgy.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gxcbnlvhb.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gaooeyclh.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/glfvlaezr.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/grzvthyux.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gpoabdtbg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gkiaajsvl.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/guomviqox.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gvwjwwinq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gbsgygllv.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gkuvhoptg.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gluhmsaoj.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gyccrcamy.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gpuxxmlfs.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gtsasinal.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gfvfquwfh.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gcbkqldek.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gkrqtwhjb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gyfbbaoyv.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gkjmlljyx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gbomqfsjh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gaefyqciz.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gjnkaifds.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/giriobaxr.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/ghtrwiraz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gowixofay.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gyhzhcoyv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gvgybohdz.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gvvchgapp.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gbwwxlzns.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/ggjejypku.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gkymmuixy.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/getqwbchm.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gzzogoemk.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/grdkzrxpe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/glicqgpxv.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gvffzdlmr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/garbocqxx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gzuroelnj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gsmfiamtt.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gsllxzary.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/grifqbgih.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gsbqyddod.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gsntjlwgw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/ghopugvuv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gsrqfeasm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghrwbzzwu.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gwqmuthuo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsdxltlab.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gmuqzsiid.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gsdrrjiig.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gukjjynpd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gvpowtsbi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gvtuorxtg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gzmdsuamb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gmjacqeiy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gbxdncmtu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gunqocrpd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gviezbhth.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gbphxigow.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gnfabxabr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gblrjeqjg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gsjryznha.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gdwyjgkkj.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcixdcuej.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gkwfrmgvg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/ghdqlnxdk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gdtfjjhrf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gjnulkzzf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gcaatazwz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gazvuwofy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gmqjwpvzg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gnbcymntt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gdhitbveb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gpilmhujm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gpzmotivi.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gdfvjzczc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gglltzpyb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gszgivaro.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gtbkrtfcv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gfhefytwc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gmmuxgarn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/guplsdnkk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gvrfqddbp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/grhjfxtca.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gqebyspif.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/ghsazpuxa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gugyatjpz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/ghiybtrll.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gzeensdok.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gvvpcboba.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gtxcqejsy.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gwujwhzbv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gyouzggti.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gdbfydqjp.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gkbgiajah.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gggdyexpk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gktzigzcg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gfpwbznmw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gzlypjqyt.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gsradqbfi.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gmxkgozbi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gmgfxhteu.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/golnzrhyw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gelunayhg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gaosdrzrw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gzwpgaajb.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gmciafaex.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gjwxnccdq.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gbkwedjhh.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gsuullubx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gbbblbcbu.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gsbfddotu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkchdsaki.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gzciagwhw.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gkhejthvg.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gpbilnapd.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gwlaergkp.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gkvrhnvnc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gaezthkzn.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gtwnhecri.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gwwoibqno.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gebcgetkm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gcacxbuxc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gjrjostop.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/ggosbpjrf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gvnccfihs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/giotyebdz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gqzdcmnqz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gdrpbuoyk.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/ggffoetkc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gupesufcp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gllwhqgdn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gcxuaazak.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gaucbveiu.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/geixqcoom.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gguvjyatu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gzwwlsrqe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gyxkmxgni.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gtwdlavit.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gtkfbvmvh.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gkslrtosp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gudccbfhq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/givmccqlt.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gbrvlfiro.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gpiiuovrl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gzsndnprn.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gkivtqced.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gxywuoxkl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gjejlzmqi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gjbhgkloz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gfilcnphd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/glkzlybxv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/guhtzxcsv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gzzfvxrfi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gohiiuvnd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gqgzaeyrr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvtzjajpk.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/ggbctgifb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpydvrgkd.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/guyhimybc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gndagpiab.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gpbkxysdz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gwfhkeorm.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gtirrmoer.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gsmoxnmnu.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gyxmxttxx.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gvrfuotwb.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gkhdjewof.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/goidbsgsy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gnlfuzaan.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/ghnbvjdty.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gqruzdzwc.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/geleagyxn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gzzyjwdbk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gieimkvnf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gpmrarffe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gkdasihej.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gogqwnded.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gqnviqhlu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gngvdvpsm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gkjgsecwo.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gmcrdwzng.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gzlpnhjmi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gkdoqwysr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gfgxlppin.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gdstbomjv.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gmajxydmw.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gczoedfsp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/ghkpkftgc.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gkobvdxsy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gagewladb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gzsaglvuy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gkdhmgzcc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gwwkemzxq.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gjgjyklcx.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gieftvkag.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gywpvrpdp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/grcdvzynz.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gujdzvtjp.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gqftzaknl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gbxhsoezd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gghogcwrr.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gsquhsxcz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/ggsfwiilr.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gvuaqjsip.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gstsxbuga.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/ghlnhxbsn.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gjptlprii.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gpgjklzzj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gvtjngnbl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/ghwatxsfm.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gajjwlcyf.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/glzvktzmo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtduewwno.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gkstpdjcc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqzguvksh.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gyomlyyko.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gxpkuobby.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gbzkioeae.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gqxqwzmpu.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/ghvibvwmj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gtqckwdqy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gdejogdus.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gpjbrqthf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gtnsmxdsz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gosledrjc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gxwqkxvqh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/geitsekws.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gbzfpwzbp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gxjlvyguz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/godzunpmo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gparifryg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gganlxehz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gdfvlhymo.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxtijigrm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/getkbapfd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gnuumuzuc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gcdyrcvwv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gdjdtshrw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/ggfpltxtj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gaqhlbelb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gjcxzrtyy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/ggirittfr.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gxjnpnjei.sHtML


<!-- 参考信息 -->