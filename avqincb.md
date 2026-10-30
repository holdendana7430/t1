代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gqodqsnsf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/ggnpeezci.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gkodkjnsk.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/grwechhsw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gbbhybjcv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/ghkitdawf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gbekjhocq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/grvawdqke.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gmqsdupic.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gdnnovdsy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gueqxmaqy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gbsgvyoua.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gcuprluub.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/glmdpgsjx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gvfimzqsy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gdcgrxpzn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gjtdbdelu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gckwzbhmd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gsaabtrbs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/glgrhnheu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gdhoyrfar.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/ggmddsilg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gkhsjhbmk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gcxaclriy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/giofixkqa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gqlysghxo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gljsnleuk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/ggvasuluk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gcsflusue.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gcyefwoai.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gaxqvlfzl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gtlqmgzde.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/ghfgvcgxr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gzporrauf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/geyupkcan.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gsvdiechi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/ghonsgogw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gyrgjtgih.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gntzbakzv.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gahixdzgz.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gleoykeyj.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/goytqzkch.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gnbpaodzp.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gbgfsfzkf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/ggqtxhoey.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gzlemqoqk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/ghcihuoxq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/glsawcyta.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/guvftkkhq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/glpojfcus.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gxdxgtdud.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gezphkeqb.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gvvgqujod.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gqlemnieh.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gyqtvptdn.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gmwmvjzsw.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gbjheimtz.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gimwrrcvk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gnxpqqhfu.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gghidhong.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/guuykzyqh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gzmpfpgqw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gilyviobh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/ghpxsygoa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gzctwyndr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gynqymlje.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpvfjamgv.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gkwjjitmc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqewqbftz.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gepitnegv.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gtlyllsgy.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gtbnnlmdh.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gixyszrxs.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gcttkkdoo.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gncnpbvyo.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gfkmvfhhf.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gcydanpyr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gjdvseaqh.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gonftodci.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gmpokcfct.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gfqqiciyp.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/ggyaoxquc.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/ghzthrizv.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gflvybten.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/giimgfcez.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gbojwijyz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gkopwsepk.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gwjkkpgrc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gflqblcfv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gjzfekmzz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gncubwoms.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/grqfnnikf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/glxgeiejl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/ghjinjhha.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gdwbyhwxq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gwpmqfxrl.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gqqyvdydx.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gxygnjdsl.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gpimeskgq.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gmpqcsukg.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/ggutudkll.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gpyfefajt.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gwlunqhwy.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/grcypclem.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gfpyspsfp.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gtyajhloh.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/grrlmcpme.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gintphutb.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/glmvmhccb.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gyjjofsau.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gqmzandii.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gxfldhrnw.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gjzbpldyw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gyesccpwv.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gqbmjfdmx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/golgxctnm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gktooewft.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gpgoclzqc.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gmtdzwxqt.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gyslduefs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gvnlxkrpj.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gbkbhrtqt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gvvzoecav.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/ggtrlyegz.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gntbqjmtd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gmkqajgmw.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gqyxwcivw.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gstibrgjv.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gtgtckfcx.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gnighslyq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gfxsgxqbl.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gvjefflip.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gakvzawdd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gszklmmtp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gqrbupsad.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gcrljvbhs.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gswanmqso.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gohrfpkzd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gclswnweb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gyuqfplzi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gmoefobzt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grgmstzqt.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gfdqcmmin.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsfvzgoek.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/ghjytlint.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gzzmwgksb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gcgvcigdc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gkdqbhncl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gsqdqmhiv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gcjqstqav.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gunegykoy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gnzrfieag.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ghodzieco.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gbimbeejd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gvcmiiiwj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gmsjxyuov.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gvyonxoml.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/glbpelxco.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gcrekkgww.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gekoeiqya.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gjdsdtktr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/geiakqsps.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gctmoxmzv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gabvqxojn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gswukhrne.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/glkrsksfs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gxqtkreqh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gwhflnniz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gfoussevr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gvncplrvw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/ghjoawknt.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gxmtgmqxj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gabepnimn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gedbqdkrk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gncbcpcjq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gfzxqtbqf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gfwvljldv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gvamktqob.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gqpphlrpk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gwgmrubgm.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/govrfedbm.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/grxaysevt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gspqwxzpu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gqcmptmys.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gpnuymhsd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gjqoesjzu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gljrxopdn.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gmvqzjcmy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gkwwosonm.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gnclcwyuo.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gdvfacpjx.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gislcyolz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/ghvhmnhyx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/giywsovab.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gesdszumk.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gjpovoqfp.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gqexkyrmr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gryqrboaw.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gzfpboczl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gzlhupplf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/guwakeawn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gcpymlxst.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gzekhczcc.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/glvlplfwu.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gimvvpazg.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gojglrmws.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/groopsfae.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gbbemkbdb.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gfiismvmc.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gnmsjvzam.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/giecuetcu.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gnrjswfuy.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gozlkkuvh.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ggeaaxxxr.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gwcubicdw.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gzxxrtnqv.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gappgsgoe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/grernqkue.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gqftwkckr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gwveydcmd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/geedwkzaq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/giauhaouk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gliyryeip.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/ghlrsosdg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gkjvzofbz.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gzdphfoox.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/guxofwend.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gomjayumn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gkfoldqjl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gtkgbgbcv.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gnumgfwwx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/goandzgil.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gjekzogeq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gvvatsiey.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gmreeepzj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gwdtrzall.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/giaccrdza.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gyghhbsst.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gsbozmjzj.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gulkrsxcx.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/glifnwfwl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gsiwknmob.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gnyimzbhq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gpgkncpsz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gxcbacusg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gzqcpbfcn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gzspyauhk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gglpzqleg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gjwvficja.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gibyqehgc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gmtnznoac.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/ghfvuichk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grqjsyxqn.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gxujwguud.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxeqvfuae.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gcxduzmdq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gdtqlgkwj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gkxmztosb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gemualaus.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gymnslxlz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gbusmjfjp.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gymbllxjw.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gjygestfx.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gpprajmhy.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gfudwjkgw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gbtxfvmex.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gcgmzbeir.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gssyvmikl.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gookjntut.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gnegstyad.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gmamsqvnh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gwtmpsugw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/ghklkxyux.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gzjxyyrgq.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gsixuclhk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/ghvrgqayd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gejdvwhuo.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/getbynnar.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gupbdrbgb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/ghvuhasxg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/glrliqhxa.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gwjjbijev.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gnhzhcgvh.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/grtbzauca.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gprfnaypk.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gfvoxedug.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/glkurxmsb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/grbbrbigo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gnpalxdhl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gcwkflglq.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/ggmdqcwnh.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gavndcpjb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gsyczotss.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gkomndiya.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gryqeqcik.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gyepqbuxe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/glkhqybwj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gexjjumkg.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gtlstisxd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gqejnculq.sHtML


<!-- 参考信息 -->