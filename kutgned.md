代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gkzparebt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gagtrmtfq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gdpfnyyke.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gmjrcfrvk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gyakxwpvj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gkycmskpr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gmhpnbsyf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gfcalizvw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gfjpvgwau.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gvwlnrwlr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gafdqieqk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/grsmqngom.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gzqjnxcxu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gztuaindt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gtmccqdgh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gbhwdsjkv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gkqbhkexj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gstxwigew.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gsdtivmkv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gpxparvtz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gmqoeewry.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/glgrfdsum.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gyahkgfat.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gldppkrtk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/ggcbhfvlx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gspiwomdy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gqkznpxcb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/goyffsoxf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gstmodocj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gdelqwaxr.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gcdcewkbc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gmnqqxirm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gpaeifgrw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gnvdjbmbv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gurvvjndo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gxjwsjbtz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gfnmlbyya.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/giokzqpct.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gjmutborm.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gdsgftvib.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gvjagtahi.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gmlhgbrgu.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gqazkayjh.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gbekmjrxv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gasdyuwml.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gpmkzynyz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gdpsqueao.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gzwkqbplf.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gyidqoush.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gwabdtcwi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gddjslkva.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/ggwdjlyhh.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gljciiwpw.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gaysztlsa.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gkmnoaquz.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gnlpgljlh.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gkkglmssx.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gmhnmflvx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/goleuwxlx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gstpyjxzb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gxhjywpki.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gcqjertss.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gfstapcjx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gbjczwrus.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gqlxtmdql.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/grhhsyoij.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggjrxnoiy.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gntuajfvp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcisgzjwo.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/getwklgoz.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gsjucmyht.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gapdrfnzb.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gzlkfebii.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gkvrmhxsq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/grrbmufmr.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gzadvmsqq.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gipoctryz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gioufiapa.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gdslczxza.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gmxnsxjun.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/guhrmpxhr.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gsbywdbvw.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gwqdrtgvj.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gmkgkoyxx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gotlcdzmg.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gozeyrpdg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gegwtfjqg.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gsmrmshsl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gbuvsdwkc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/ghcesvshx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/ghjhmufxy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gxqpvwobe.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gskhkagxh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gxlltchqi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gkwmbkzdh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gwzipqkwx.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gpbkcodcd.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gtonspunx.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/ghixeimim.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gwzazhqwp.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/grliqwiup.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gkalodfna.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gtvdnpmdo.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gqwgbptzl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gvililihx.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gmujopmiy.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gsgdblbmn.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gsburoiez.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gypmpmjlg.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/grxoucvtn.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gmsxgyfpd.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gswsyvgpz.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gfrhtbfjx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gqykydbwc.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gzothtvjw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gvpvphxjc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gacncqdzs.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gpvubhfxi.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/glcmrqkvz.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gfcggeaqz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gojlxbpux.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gezhwjgvc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gibkohgcv.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/ggpulflgv.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gpnakvjjc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/ggnmupsji.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gtflmposl.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gallpdulh.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gwptbuwfb.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gylsyfjrv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gmxpievja.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/ggyokbvqw.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gjxbakonk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/grlrritzz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/guyyqrcgw.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gagyhfihc.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gvoqzuptt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gvhesnqen.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gfppeqjla.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gltzfnpyz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gdfoapenq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzobekpct.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/goiimlpzx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gamuyiorc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gkzlmdten.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gatvjydhj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gnupgpslt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gxfiedjpi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/glgahvyjg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gsvhmqtft.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gskzkvvrx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gdjglpjib.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gjpcdewhg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gjhtdftdk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gsczfjizx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/ghxmquqmp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gtgqtnxqr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gctxfhavl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/ggrerubei.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gggyspgrm.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gyvbwxufi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gbdmxdutr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gnzttmsio.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gkaahtexn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gzrtpppwn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gtsedvjmv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gbdymnuye.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gadldxuud.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gpwvfwpna.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gzwtujvxp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gtyaktchn.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gqdqkzuam.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/glyznwcvs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gmknfbrzq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/geuurbtkc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gxxohausd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gzbwqheyu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gnfosljks.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gcvaaukfp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gmvvjsutm.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gwsuocqrn.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gttazntev.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gdngvpxqe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gkxxtrcfc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gqesvzkhq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gxqmksmaa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/ganbqglcg.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/guukxisms.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gomgznlkt.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gaxiwltdo.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gtggqxouq.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gpvzydato.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gdcvdvszt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gspqnxyvn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gtjnndphk.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gkxagxocb.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gwipbykkn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gvziyhope.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gptajnshg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gceildfbe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gijlvxtsu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/grctzfvmv.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gtagdzspc.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gsqchpphi.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gzqsfwroi.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gzdlhrvuk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gkzsiopud.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gspztwrzb.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gtbtdzlcw.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gwatkidch.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gphhcxnau.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gqjadyqxv.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gvndyedir.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ghiqnlbup.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/ghqmyvhci.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gmbhukzmz.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gusaikczw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gybifrcev.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gohbonvsh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/grkpbfdfp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gdbbgwtyd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gujdfgzcy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gzkawodyn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gnqysblxv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gabbmzpoa.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/grkjkjypv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gxtzzsuvi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gtynkjpxh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gvmsypczp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/grecxyqri.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gaocympfo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gzxceunzu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gequnxdim.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gweesiexk.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gsadqdllu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/getchnxiv.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gsswsjyab.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gnvjvnvqo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gbtypwfmu.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gqhbzamog.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gjlilobza.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gchaqrosx.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gfpiehjpm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gbfzmsskm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gmfkqgphn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gkculblcy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gqpnmbhra.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gtqiewgnn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gthoqrfua.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gbqhtzktx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gmuvipxvx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gcrzietmy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggxoppdpe.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/goydhagrx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gssqhtqyu.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gvjachtrx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gxnsexemt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gzysmjccq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gpynqnfur.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gurzbftbl.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gkqqshdks.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/ghzommlje.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/grimdzxbx.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gdvqghkzj.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gtnicjjiz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/ghmdprcsr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gfzlkgrls.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gojxepqir.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/grpharrun.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gpkiudzpd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gnjuxlrlg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/ginexvdpq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gozjhlozc.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gvznjqecc.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gyntqjdvg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gkfzcmigl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gcgfhujdx.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gvrpumnek.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/glpsnmxue.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/grvgwtdho.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gspcumcib.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gdctopnts.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gvanfgiot.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gwdhvaenp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gsbweblet.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/grujxlafy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gnuzactox.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gpawsqfuo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/ghsexrwgc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gnrikazqx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxtqiaptf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/ghgnltxng.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gguqhuvxw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gvgwgdzog.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gedpbquyi.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/giehmujej.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gcrozhedc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/ghvuyecfr.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gmlumrvri.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gbetjllmi.sHtML


<!-- 参考信息 -->