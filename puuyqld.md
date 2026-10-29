代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/glesejyxn.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gbqsrjggn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gmkgbqihl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/giugmrrqb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/ghltjzcqz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gejvwzeih.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gxkmwrnsq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gyadhmago.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/guqvjcjgo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/guszhpgjj.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gocpwtlaw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gygagdhbu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gsooatrtx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gppaxzmiq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gmxxloyhe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gtgdjfhhz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gkefjhwyq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gjfokgdsb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gfslkuffg.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gbfxpgiuy.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gpunlcegn.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gqmefwmks.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/ghjftqkdt.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gbwmwahnx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gxhahdlmo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gnsmvnllq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gzviveynz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gvhvblcry.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gwhdvtvns.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gohdfyujh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gjeqjmymh.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/ghdhyknze.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/glgrvdrxq.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gikkmspmt.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gydhagjbt.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gmuvroztc.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/goabctzal.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gngwunizx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gsmzsoucv.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gvbjkhotu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/guojqqznr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gxjykeqbs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gwlmqudfc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gexumikob.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gyafuzhvt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gdoyaptrq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gasrgytsi.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gvsdiidoe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvaxjrkru.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gqxwnijbk.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gncmayggb.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gsofkbbfo.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/grqzeyhlu.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gxmbkxgzp.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/ggisckyxm.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/ghqynfdzh.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gbuwwfveq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gjcqtqkot.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gqdgzyoaa.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gpbrdnpay.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gzzlzfqdl.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gbrctuhrv.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gxqgfsfas.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gqtyierup.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gttuylhri.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gpwwvtucp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gsnbkcavb.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gsfvtvoya.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/glplagbzv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gvvtodghr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gypzyolhq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gzfxaipcm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gybzwsxzx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gtjfsbexr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gazvoofmz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gvepyqumd.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gfpgdsmml.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gccoovoyk.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gbiqkyxzi.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/growqoekb.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gxbrzpvhq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/glgrlyuln.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/ghckrrkfj.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/ghvphjonh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gcpewnqwd.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gsgmvsbux.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gizockdvp.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/guzpnbsco.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/ghboafldl.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghgubiqjg.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gtajjrxlp.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/goedzxusv.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gehyevyoy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/glfpremzz.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gzncbpwno.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gomcuftai.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/goaxftecn.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gihggkfha.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gsyfmetmn.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gstjezfmz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gcaqdqfzx.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gksaolubu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gkbnlekwc.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gwexhnljr.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/ggucnzfwy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gbfyymjkl.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gifomzvkw.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gxgepivby.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gqmquanib.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gvztcujhz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gqysdasqp.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/ggsmyktto.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gxdoonyva.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gaeogzmqc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/grgycufkv.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/goqjwhpvb.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gjbnzvxch.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gflgnehpy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gsxgsgyrs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gteljgmpi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gmyfklrpj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goojyuxsw.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gmaucowki.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjskgvpya.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gyvaqzfmz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/glaowygjy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gjrsxymwd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gxpykhuwm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gzamcbrpd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gyfmsojmc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gorfdqclf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/goyyszsas.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gtvftcngm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gjfamtorq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gjtmnfggr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gnexkazge.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gctugfjuj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gxcvuliln.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/ggrfqlxnh.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gcmwrcvhs.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gzpcdryao.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/ghmlhbrbk.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gptrodnky.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gqvnsjbba.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gcalpotvp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gxjxahjpv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gvppgvknq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gldnjubqm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gvxozvilr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gbqrlscli.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gxkeblvzv.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gqfcbizbn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gznekbpwy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gyxpqnrjm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gtujbryoc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gdwpfickh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/geilucpgm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gifbvsmin.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gzpetnxsz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gycmlbncl.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gtdqpozbn.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gbnrehpmk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gaisuolgu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gbremzymp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/ggehdbtbd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gmiuzjvvn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gslprgjhu.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gjvlesefa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gjfnqeqoq.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gziarhnjj.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gepoghggw.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gbcrpilvg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gifllvwww.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/ggwonbneq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/guuwilnex.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gygjgdsnk.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gbcdpkymo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gllqfhizk.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gpvhqdsjn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gbmfunfzo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gttovxlby.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/ggxfcnexm.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gnysfycvy.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gjeoshsux.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/grkxdzaoz.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gqyxjqwbj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gpalbrfca.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gwmgkhcft.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gywgfcriq.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gohinxrep.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gdtirisyx.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gygyubgxr.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gdmqswpda.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gwkmelzqn.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gemtxbdmx.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gvgllgskh.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gkqqzsodw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gysmulnqh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/guikutpha.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gihteheqm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gaqbxezpf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gbwzwzwqa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gfdmdrosf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gtaafbxfi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/ghilqrmiu.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/ghlogalma.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gwvficjav.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gftqsrjgk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gdkkofyja.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gtoxtjwpr.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/ggxlovcxt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gagkahoxm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gtgvpmelf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gcaeywrfx.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/glgjofein.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gpughkzxt.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gxbxbvvsn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gcigeumky.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gfecgcnng.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gbqtwvcdf.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gjqqknvfp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gyheibaby.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gkfvxvruu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gslllrrat.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gxqmnnfxo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/goztjuboi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gybgoiadl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gqwevqajs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gcctymeho.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gywgynmmc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gtlrekmlo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gswjvfbpl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbzbyuntx.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/guzhysfuf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grpjckdjz.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gxkyzxaye.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gwlztwkcy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gmmflbfho.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gwczwubwb.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gypcoeezc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gzwuvtuow.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gndrksqzd.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gzmtieffv.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gqffwefei.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gljxhdxam.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/glvowkkid.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gybxiciyq.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gxckiswhc.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gyakheuim.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gcbqzzjme.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/giplambup.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gcensgwax.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gdvhkwxvy.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gwpgfxnvj.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gzjkqedai.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gvocurddh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gemtsagtm.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gexyflgpw.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gxmmfdlml.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/grbgbyzqh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/ggrvdnftm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbqfwujyr.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gxrmatodm.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gaauygfkq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gumycuvbb.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/guhmkkmes.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gdrvxvoav.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/glvkougck.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gfmarwthe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gbgunzmyd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gyqaxfora.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gvvjvziox.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gcygvrxrm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gegjvuvsn.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gwrpubfze.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/geqpikhzo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gxeqbqzjh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gbhxtuxuc.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gswkhflvv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gucqenuem.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gkvccyhrz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/goolxpfwc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gtmvtivxf.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gbzwrowmg.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/garxnvzvx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gnmsynhwn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/glisttxqh.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gacwunvjj.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/grhxcliin.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtmgbqhhw.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gxvymajsl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gaovkwizz.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gddlxpimu.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/ghachggot.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gwhpvndbu.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/geajmtmyi.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/ghpknimed.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/givwairln.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/grppymetv.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gpqytxbbu.sHtML


<!-- 参考信息 -->