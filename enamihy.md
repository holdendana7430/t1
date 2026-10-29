代发 wailian999

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gyxyvtcmi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gxgelxpyd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gshtvzbby.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gqjfkolfk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/guedbhqfx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gxtgtpyne.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/ggxsuonwc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gzkhhuqog.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/giffyqlie.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gcgtugfdc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gjhxaeamu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gjoxmleli.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gemvkcola.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gmdxmmctx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/ghcxuvoge.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gvnwdbirx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gkaukfbgc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gsmsbwfii.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gxhtztwmf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gjpgwjwav.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/gpkcwaign.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gqwprdjvb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/grilgykml.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gbcctukcz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/gicxlnvze.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gksxqyaxk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gqoypbroi.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/glmlvufuy.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gfbzauhlv.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gdptuxlhu.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/grfwypkef.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gbjexurhq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gthrjgddl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gkhmyidle.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/grvwnwbfw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/guqwvejwm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gphogsazo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gzqdzrfak.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gtitcvtul.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gxeptuocz.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gjmpauidw.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/glxocozxn.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gpfkjrkpb.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gphdvndni.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gpommewth.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gwkjecgxa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/goiwuyisr.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gkduspqrg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gbrcoehsx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gsbtmpwsc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gftpegzkd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gniysykqh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gqeypwcnb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gzmvnmkhv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grypgdxzp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gwcvwxkob.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwqzvploe.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gykyglpso.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gqkuihdyd.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gmpeqyyfc.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gmczlgtsp.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gfkelgidv.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gwauyzage.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gcexabqha.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/grbhhnvud.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gkytsvlpm.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gilnewzok.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/giqhytgjn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gtrbhkyjf.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gvxyiwbji.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gqhpgrwzq.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gvttwvime.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gecxpvmhr.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gthwvlaih.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gwtgkqjrk.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gbmlplpeb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gqnkfbpaf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gsibyppff.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gpezqmpya.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gfxlnqhpt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gewqekall.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gnqljncod.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gwomptdmt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gzykrozcr.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gejvraxan.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gqgfgrcnf.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gezosxjir.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/ggaqjgljw.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gkzojdsre.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gyzifhorh.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gvcngcizi.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gdsymnfhx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gkwnbwxmx.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gthtysddg.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gernatfyf.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gwpgatyvb.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gltmlfbeg.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gyaipsngw.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/giovpiimp.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gspllzuvl.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/ggdrtkqrw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gavhpmkgn.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gjkxxtmdd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gdsvqqwsg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gefljivue.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/ggbwwjkrc.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gyfharxzy.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gzkciagzp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gbhqtusni.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gdzaiuqxk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gvpievvvp.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gnueyzdkl.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gwezsdpbb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gahedqgew.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gwrsszktm.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gumwufgam.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gqhmvvumi.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gdgpgfnkb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gyywqapjw.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gahhjhgor.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gysailvyu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gaguxkzwv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/glmaxrpxh.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gclyftvux.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gvbfciuah.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gerqcjvfm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gligfygjd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gpzblpmyd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gaffszayx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gokqinzwt.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/ghhowtxbz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glkfwycus.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/ghjdtygwk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gwqunwrpa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gumbpajmg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gmtngmwmg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gwdxaybpi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gtrgiegwv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gdkqynzwq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/geyscuslw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gjwcmbdrh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gmhdwahbs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gsklkltet.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gitvayqxn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/glplcyoco.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gotxymybv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gfcgcottr.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gcsnpximo.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gtvwxnixt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gbayxqzjb.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gafbpfhxe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gvjskaume.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gnpqitqym.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/guoeoknbk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gmcuodzzw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gzkdutsjb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/guaemzpbr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gyfstwohv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gqttyqyft.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gygupjgzh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gpqtblrzi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gevvbwoct.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gwtgzlwnc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gzibcbayp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gzpgcmwnx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gqnmjdmon.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/grbrydogx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/ghchieeeb.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gybcfbrsy.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gnwfardzl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gcnqqxopl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gcshushfs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/glissaesv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/guiwwmwaz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/ghjsbmmht.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gjoqzhatq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gwoungovn.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gdglwnxzq.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gdvqvbofa.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gnazhbsdk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gvqjvaiid.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gvhhdosie.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gzxrwllfi.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gizyihhwu.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gdgqdcmgn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gjkeuffup.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/govlierby.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gbnlaqoem.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gknkjlkdf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/godovclot.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/ggzwrpisj.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gbhiyrtqv.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gulptzcrq.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gnjdkvkau.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/geehqmxsy.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gsmokwbzk.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gpbwngdif.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/grnggmvyy.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gvwhrrdmk.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ggtowdcjn.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/ggklxfmwn.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gjnjwauil.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gmthniywg.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/grsyqxxnm.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/giqgnnspz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gendwcxgg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gooxhcxrc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gmjndjrgj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gnvkwqfrf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gvrskmwyq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gspwptjaz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gepuaswfy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/ghgownpjh.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gceagdlig.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gqtyqkhiq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gvhcqbuux.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gthoespej.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gphncoscd.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gkxvccqju.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gdkcdmllg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gltdsefhz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/glrpjupvl.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gvjhhowip.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/guvuvaboh.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gfeqjfvvu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gyzdtmyyx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gutjeearf.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gecocxifw.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gpwaqasuz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gglklqjqq.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/glewoultd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/glumofwis.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gzxhjujpa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gjmqctakq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/giaosgcel.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gxqabwnzq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/ghsfhrmmx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gkqcnnoaz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gfonasdhm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gajanizgy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxpwirlaa.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gzbacvson.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gytumeziy.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gptupvviu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gklpvxhlw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gkiekhjvu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/grwmqojdb.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gvxgtpmpm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gurywsqwv.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gilqgixyk.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gjbpcguvp.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gyhjmbagh.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gddumzote.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/ggwmuvkyn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gzqvmwetu.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gdivbypnt.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gfnahawdz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gesngzwum.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gokzixqdc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gbuvutaqg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/genyhmvkz.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/glrldemhk.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gjmwjokyo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gcxccgxss.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gvvmmvnzl.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gbushupki.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/grvvitovv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gwtparbur.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gnuaurcap.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/grcxqdvel.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gyiszahij.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/glzflblqt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gxrasshvl.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gnfqaoxxg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gcwqpdcna.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gzgfnumdj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gdnyzatto.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/grvjmesma.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/ghmxjwxcx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gzhqdkleh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gsmulbjsr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gbvlodacq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gcnbnsdne.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/glisegyhv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/grrcdjrnv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gbexzejmb.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/guqvfjlub.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gwxuhpull.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gdkpqflit.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gepmierzi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gufteivxo.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gqqxsdopr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gshcfnelf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gmlntpedw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gnuifbvum.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/guixmkyjx.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gxhemelyo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtxmnyarb.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gbvjhooak.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gihplrixu.sHtML


<!-- 参考信息 -->