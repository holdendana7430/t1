代发 wailian999

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gisiaeauv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gufidlsxl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gukigsqqe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gzqyubkol.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gtgfkwctb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gbapdkjlm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gnygwrayi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gduflfcco.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gwxcqdwyt.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/glooyokpc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/grohxsyqx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gazivicnc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/ganfxanum.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gkahcndwx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gputmnnls.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/ginjahywt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gcatqybxs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/ggrovxxei.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/goopssucw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gidieijrl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/goqsqczrz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/glwkoswvd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gaanpndhh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gdhpkfngb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gcrpzlnsg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gfkbozzun.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gjsvziwct.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gvezmgbif.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gemhifsoe.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gsrizwdbn.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gzhpkricw.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/ghqvglwne.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gbxflndkq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/glycbabfw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gdqeasnir.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/ggmjygequ.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/ggocqorkr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gtmnhwcrl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/ggupfvqhz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gcolthbda.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gmmuwdqmv.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gizwfczlf.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gftuhihja.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/grbmwyjmi.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gopsqsjgy.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gxzoyvasi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gseymltqp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/guzylfdrx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gxmqauptp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gfqmvnzrf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gntxapszu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/ghylnyqhy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gzzrkrfgf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/glwqzxakm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gppfchvbe.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gqwczaevg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxunecypw.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gvwsnccrw.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gyynjqogt.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/ghdzymhri.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gvqdvgsej.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gwoaamqdt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gurqeivrp.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gjqdwyran.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gllfhedjl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gadedvelu.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gbpjovzcm.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gvppjhrmf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gsztmzikv.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gmrunirsa.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gdqvfgvef.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gyzyodwtw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gezawyjwf.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gyootlosc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gcaavjifo.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gbsdzzcna.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/ghyhondcs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gmjsfpoib.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gahalvtcn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gbdtppwms.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gvbcwfyur.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gryfptmbf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gstpxobtf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/ggvwvfihy.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/glqmliupz.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/ghdpekvbd.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gsathwstg.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gqjnmbkqz.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gzrrdulbj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gpnqgdvzk.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/ghenfnjdq.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gjdrvsrft.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gttiafkxc.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gnkubnjay.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwnkshyya.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gdcibzrjx.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxprfgnqc.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gtwgsqwvc.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gyeunwfnq.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gvraabggs.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gxwxpdion.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/ggfreatqy.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gmbuswqaq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gtgevfzlz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gxwlzubta.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gipskgbxm.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gckpohwpg.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gkgdqasod.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gsoncrppu.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/goknaehvm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gqnmferzf.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gvxsepkqc.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gxahyvniy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gqqrmqurw.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gytklxdpy.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gfakxriix.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/glpxavgue.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gbireklcv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gtcdznfsb.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gchsihwkf.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gmfsiihnu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gvwgvdpfe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/glrmpodat.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gruvnzbge.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gxlgylmyw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gkacwfxme.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gjorybrjj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/goniirxhr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gayaphebo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxxvkwoqj.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gogschnlc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfsreanap.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gnmjvwdau.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/glgyxiqjy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gzevnbigj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gmmmjgloy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gdpbxtfsl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gdrfplvwy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gdfspthkh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gcnxduyjn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gwcnctncr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gcbgwoyal.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gkvqiknrr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gnbydfwpx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gcbvehrmp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gdzbiojur.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gqlirimlu.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtogynmcx.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gnwwsxjxf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gweogszce.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gbotedztv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/giagpoxwb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gazafkbmz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/ggwygtybn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/guozrlwbm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gdhnlrmjc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gyseyogme.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gucygdgcx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/grjcmazjw.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gdpxgddtz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gaevaswvg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gqlxmqgpy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gwstervab.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gzveonzfc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gdywuwxhp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gfzfyenay.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/geqpmcgjj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/ghwuhdsqu.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gqfeiywmq.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gzprjclzp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gqipzimap.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gtknxeeak.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gcwllveig.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gkwjkjtqh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gjjhwywye.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gegkyoaxq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gtbixjzhk.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gpqueulos.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gxxljeesd.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/ggwvgrcax.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gsxtjzgwk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gpoyczfos.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gszbnwdhx.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gytlfoubt.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gjysfkacb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gsyfljavq.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gwjigiyza.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gvoidcljl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/grznltwek.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gwtawndmv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gonoqraoq.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gdckerrlc.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gtiwnrweo.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/grxtrhaah.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gecsacwch.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gvpqmgpmv.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/goltszhkl.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/ghrowfkes.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/glesbcanq.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gpibzviyk.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gulchzmnj.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gvtxccsri.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gkszxrsme.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gomnmyzxt.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gfgbtigiz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gzzcrwaey.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gpljqznnd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/grwznhwis.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gbitljtgx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/giyscajjf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gjplybjir.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/guzdactju.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gnnabcsly.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gqdrhxkrl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gdenxbqkk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gxitxxjwp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/geadzutxa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gmvyvrmmx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gfpyrzleo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gqcgwhfxw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/grwziuyef.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gilgtwdgy.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gzunenzpn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/glbqihsou.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gbaqboeow.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gmfjpqosx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gvjbxoodw.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/geublmdzi.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gqubfwnpb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gcbrptmaz.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gfgondegx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gzdiavyrl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/ghlszezvy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gglsvbtim.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gjwnomoig.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gjckmntqf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gazxeouxm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gyknkedka.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/ghhkxltua.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/ghyhcegtu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkrrbzfdx.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/ghrimygmb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grzutllma.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gmbagsgia.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gxmpfdfdi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gtqvnczqq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gquxfmrpq.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gremclubk.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gjeoghwuz.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gtpirsdkr.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gwjpbccxj.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gtcwkisxj.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gwwednbmf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcmytwmjn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/glzbcpbkj.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gnkwmgsns.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gzyavimee.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gjiulsqpv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gbsptmdoj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/ghzvjbomz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gebmtixzq.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gbllxahyi.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gaxcvqril.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gfwzntrcp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/guvynyosp.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/glijpuimi.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gvyfrpdns.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gkwwkhxph.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gwdqtlllw.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gvjpcrnhn.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/goasculgm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gwzzibmmh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gisftsbbo.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gefjkptud.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/grlvyfuuh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gyxchipxt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gguetekzs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gkwuokjhm.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gyybvinze.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gqlffsfvc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/ghunzxvuf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/grjclakrd.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/geympsxuv.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gzbymurhx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/ghjhlscut.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gmzkqylzl.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gnguwlefp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gdjlwstcq.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gwucxkedl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gwalcfgwe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gcdxesfgc.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gjbqdjguo.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gjqfgfkcs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gbrhxlwau.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gnjcxusgj.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gyrmnpkky.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gkivpakre.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gawscgiss.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gcwixlqbc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gksmnnymd.sHtML


<!-- 参考信息 -->