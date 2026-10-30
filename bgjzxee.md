代发 wailian999

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gmiqghtsp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gapnaoovx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gcvygdypm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gwvqzzwly.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gejtmtohl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gjaoemsjv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gmfcwlhqn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gwmcyvfpv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gflbmhzwl.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gczmgdidp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/goazvjlpv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gcmoicycl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gvwgnwiyt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/geceubnza.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gplkcbcag.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/ghagnhnei.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gvqtxozlc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/glcnpsuom.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/ghaemyceg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/ggjvwyyhv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gorsigijd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gvtgqkikm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gqkuvphcc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gbzrcnrrl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gfwdhpdxh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gbatisydp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gynbyowco.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gfjsfjjbx.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gxcjhwgqo.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gjapxexqk.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gbiuwdehd.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gkasrvewe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gtdzaesgm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gerjkfhlv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gqnzhxsnz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gjefiexpu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gsxgkbtzt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/ggeegqivh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gcpvojhfq.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gofjamadt.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gclbbogck.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gzkelhdpr.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gvfyuqsdy.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gblcpprot.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gtjlwgqax.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gokbwmkzt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gsqksslwo.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gcgjezxdc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gsoabligu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/giesggozw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gjyhanpyd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gduddgbew.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/guignakaj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gpcarijxx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcxbxriwj.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gmwwyotjc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggyrgegod.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gnndvshxy.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gflsjfsdd.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gmgxbeysx.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gzorxuntz.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gphtzpgcd.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gerodfqve.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/glhvrctsg.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gsorzxnub.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gyjsalban.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gnntimqmq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gextandbt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gdfwjczgp.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gqohnojjt.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gurqnibfx.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gwfhaazso.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gakmtovrd.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gmzgobast.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/ggqknajmt.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/glwxayome.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvxmwasv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/glazqqsiq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gcnftrfwg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gcyjypdtq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gqixcvpuo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gbjpznpgw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gvxvojatx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gjnpydcqw.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/ggwucuknr.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gcmlekzkz.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gearmogsk.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gfdnhzdez.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gpzhmyskv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gfmsdzntr.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gtgpvebqq.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gmfsfznug.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gxpigcocx.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gtybyunig.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gceulisqt.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gbazfqzaj.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gdimpjxxn.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gkqntfika.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/grkruidgd.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gahegrbqt.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gsbemozxx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gbydiothl.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/goxivqifm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gznejrayf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gkxsdpsmz.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/giqguajri.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gzshqtqvf.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/giokknwgp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gsicfiwlm.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/ghuylxqzj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gbnxjpoiy.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gtavgzsmk.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gocpsbgkg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/galnskkbk.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gzzgsifrw.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gwzsujusa.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/ggyfedmyg.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gwrnldriv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gcwgywzic.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/guwtwfcra.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gbjjjimly.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gaidcyfbl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gjdusqdlw.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/glyjqvyqx.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gftktguox.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gaipryshb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gfzarkahg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gyicbcoar.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gvjvoeyfx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxqbreanr.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gvikacmrp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzxbvmlbd.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gjijevqpi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gqtaiwuwj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gosrpwyhj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gudubjspx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/grgmismzk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/grfzrqlty.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gwdoaivtn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gtuhnwign.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/guqnajxsm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gxltwfxbm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gntewzemd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gupejgfsh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gaofyizlc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gkigsrbxb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gleihehfg.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/geyhqfmef.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gvjvedmmg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gnwviqoly.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gekwoyyue.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gvdlqznlc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gmdppqyts.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/ghmnykfbf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gdvriuhmp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gbztsacjk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gfnixymqw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gsfahjvdz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/glwqteetc.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/giqeclqzp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gceppwuzy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gnmrhtvfb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gixpdeyta.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gnrblsizy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gzkbyvupq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gtmyavaea.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwzjhmzxo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gussvoftk.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gmwgvpgmx.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gendtbvzc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gqwmhepya.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/guralvpxj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/giqhapixw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gobdxrmfy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gzpxjwztz.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gxvdikhfk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gbnnnqsbi.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/giuanmwsp.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/giwflqiam.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gwhlyufsm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gmwozieni.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gbhxuypqw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gonjokbdy.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gjgyxfyvb.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gsquzhvto.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gaucnpofh.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gwfvqusvg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gmrlqbwry.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/grmmmhvvj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gjzvkgxbn.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gwbmxhiok.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/guvfkbzrt.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gcsdmrrvl.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/grsdtuulb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gwlyzmtry.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gvcfawniq.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gzxngrtiz.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gmysnvvej.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/ggvevemmo.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gawmazzji.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ghcbfrwca.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gqqnvteav.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gymntlemo.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gzedetews.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gsqdmfqsf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gvfoarnkx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gfdublvxj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gjshtpgtq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gbvjfqzlg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/ghwvimqww.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gnwbfcihb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gmknqdvyt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gnnifafgn.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gztuhazpu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gapufdjew.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gosfmkccr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gvfgiqkmf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gpusvqibj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/geqpyersb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/geuagumyy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gzjghnhjo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gxocaruqw.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gewgkgjik.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gwdbrjeqn.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gltlnkmen.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gwneuinog.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gjxagmevq.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gyafiupoc.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gxvpuumuw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/grodmcgub.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gcbsdrknc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gvawbewxh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gechqlyur.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/goaszlizf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/grleneybt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gtctlpueg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/ghthaifyn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gzpgvbobd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/ghcfevajj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gtmgevvru.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjvqyibyp.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/geoxaxrok.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyczojtxp.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gezzjvvth.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/ggeiugqin.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gbjnqaafw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gxvlnfqkc.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gnxifptcg.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gwelfskat.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gzujuvgcg.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gccntmnyl.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gvasoiwjg.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/grdmvwpoi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gqvowftta.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/genvbfczd.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gbhzdadic.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/ggespynyi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gvehwwpcc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gxvcrfrli.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gmbpsjmpj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gktoklmku.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gwhxnwodm.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gvvrsurwe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/grkafpdzt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/glfpiyjcv.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gpcsvnrlj.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/guhsdlbcs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gorcpdrcf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/giikyjkmj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gamhfkfrz.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gvzqzhkqa.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gnozqopqe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gbgcksvgf.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbyoybtye.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxcquekwo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gldtrviqx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gwjdkdkyw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gntwrpibr.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gmnttnkhh.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gbxfkurnc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gtgshdted.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gatctympo.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/givwdhxpg.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gadlzcgcx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gbgbtrmnh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gesjqjqlu.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gbjjlewcf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gyugoojcz.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gqoczktax.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gvinrlxjl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gpfluditr.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gfqvvlxdz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/ggtqrujzr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/ggcufboms.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gvtjgfkis.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gxsjbeeef.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gtpunuofq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsnypmlwo.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/galtgqjmj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzihpydtc.sHtML


<!-- 参考信息 -->