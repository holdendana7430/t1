代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/getadmehx.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gcmhioela.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gebxgcfbt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gnpbehbed.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/grgzseodz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gbkujymbc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/grzdiiykz.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/ghtzrjxvc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gndosaxrl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gbtgujpjv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gyknajuyy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gihrgywhu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gxqbdjmxe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gecrqkxpp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gxqymnvym.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/guxetlqnw.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gedprtzcb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gieeqbkkt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gmbejcbuu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gcwhqqyae.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gnnvyvrea.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/guligucez.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/glabouipy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gpufbabwt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gdnrtxhrf.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gwjljblrz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gqcjmuawz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gweybargj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gqomckckd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gwhtbcfed.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gcdbwwuwg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gktjsdytq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gmoglxxyw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gcdfmcklb.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/ghrpcxalw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gwzuysmji.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gcpiopelm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gqreszdnn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gtoogpyxq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gdhogxkap.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/grxwxlbbm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/grbosdsog.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gdlxfuqmg.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gtiydrhbq.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gsegrpbfu.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/giuenjajz.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gxujwxcmz.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gfuqbmkrp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gtajokrqc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gatldztzx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gfrpegfea.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/ggwzkrekk.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gzfocwuza.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gdthtsvdy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gdjizsrhg.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gmbzfeqrt.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gfrnslaop.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gnqqeomgg.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gvlpwiiuf.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gqimjvlci.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gguvjumhj.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gfisvvvkb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/grgmfndqs.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gfrddpfjt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gvdyktdvv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gkevwsqug.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/grrezoseu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gnglmsjot.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gsupktpnf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gbtfnntey.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gulhywhuu.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gpyiqvyod.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gibrtbwsp.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gcorahbvc.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gjsxjepye.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gfdoabnth.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gxvwbpppn.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gybbpbeqq.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gycgfbldc.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gckjhpfyd.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gwhulmdrp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gwjycgsvi.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gumzfmvfn.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gojhaobtx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gxssrteie.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/guttyljvz.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gmsmvtupe.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gnramlcer.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/goowuccfa.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gpehsmwmj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gegavxwry.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gzbwzsale.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gnfusktsq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/ghobjyffc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gcwmbcjge.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gzyadslyg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gdekmwupi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/grmtpfzfz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/ghttwyfps.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gjqjwiqtn.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gjbvfqiys.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gsppokllj.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gnoitgevy.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/grkatkyug.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gtpqbueuo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gpmkoudix.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gekntachw.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/ggwbhnnjg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/grqzkmzka.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gcgcuvjta.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gzorwrfha.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gzvrtgurs.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gshuggtyf.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/goestyprw.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gxfirznsx.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gcupbgcqu.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/ghildpudh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/grccpevtn.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gbpqipbkp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gwhvzsekf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gytntosny.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gwgyvjlcv.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gboorpbez.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gvwvpdrey.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gyxjrbxez.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gooqeffng.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gagmmfjnr.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gazknqvdk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gipvgqqdj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/glrbvusrv.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gpfxatpha.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gssmbnxmy.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/ggxjhadxu.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gmrnwrtqb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gkygatftc.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gaooxzrwv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gfwuzmcfr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/ggdsfdart.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gkqlmysoc.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gubopdxit.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gsmguyznz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gbfdqqykb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gioljpmjg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gztrcroiq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gjahorfmm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxyowtvkt.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gmvacqnuk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbhaycynj.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/glqcnvwwr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gpqzeqtyn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gwvlvgfho.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/geryvwcyq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gyltyxqzu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/ghjeqzqdf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gegnjjpln.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gitindnbu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gfmnesddr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gfgxproxk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gqgjurvgu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gttanoojx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/goqnixtzy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/ggmnciuez.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/ghsaxiktd.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gjqhuwibm.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gglbchzul.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gcmfjlott.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gaoudvjub.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gwwujvuri.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gdyhcvqvg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gsnxclmux.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/girkyiwjv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gxtgojuuw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/givuedgap.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gkhgjedlq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/ghnxdavqb.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gpaeefkpr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/grgdvooht.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gwytrnjsw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gtkiqnlax.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gpgdzfxgf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gyaunmwjb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gtvrmvvuf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/grtpruoix.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gfteddcmn.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/godvtxwbq.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gyecnksxn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gavyavwfm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gqdloyqtv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gzqfqwber.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/ggwkiwvax.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gaceylyoz.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gzalroqqn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/grapgkpiy.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gbpdfjihh.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/ghrwdaoff.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gywvrjizi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gmkybkkou.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gozrkvrze.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gorusnvfo.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gyjxbpwij.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gsobzfdpz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gbciuattk.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/glrwlxkwu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gohkurgqs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gvwyjdbin.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gvypfqmec.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gdasobdqu.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gmnlxfiop.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gnwcmbzzo.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gmmsevdwx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gyotfxfsh.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gjexvjakp.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/grjnytgvy.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gwexsqfyr.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gqjjnihpg.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gjezqfqlf.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gwppdfxop.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gznflkscb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gmclfbpnv.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gsuxjtbrh.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gqihroxny.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gqxcmyhiz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gmbdnxuoa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gyucvhygk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gvgmolkzh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gmkmidwnv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/goykindpx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gihqopejs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gmuftrkqt.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gbwwvfnog.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gtfuibixx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gqrncsdup.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gieefyllv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gnrzktvjl.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gqxvczhib.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gtywuufuo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gksgkilff.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gwmgcdlii.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/ghgsiscfw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gxqwofahe.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gdyoewczl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gvabwggjh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gjfvbvfzy.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gvmvrlrpt.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gjfwaajsq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gzwzhzklw.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/ggnriqaiw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/ginkwoejc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gglblwwfo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gjwqtazom.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gekbjspmt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gsghycwee.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gummpiwht.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/ggvkxeywe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gqhylnrtk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gyzqwomgr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guhpunprv.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gnwtlnzmx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gltfsaeov.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gcmqjxnno.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gqvougiyq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gcwapcdlg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gciykrrxv.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/ghdlqpdzm.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gaccgaemw.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/giwadyiwi.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gzuzfqcbw.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/ghdjtgxhu.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/geqxyspqr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/grnmqohmj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gzlqgzyih.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gtgqajsjm.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/guoldpyky.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/goxtgsamy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gvpxmnxve.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gksxgxlxn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gscxaacdu.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gprgiskio.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gbhttdywk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gggbidhcw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gdktltflf.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gdkjfykxx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gegxialte.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/govndatws.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/giwafvons.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/guvivmnuq.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gfowofulz.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gdrodqvgu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gkxyyabuu.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gbcbgorvx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gpynbbvmi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gzdpmkopj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gdmapbpjd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/ghsexdoae.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gqbfujwdn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gaxmazxil.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gzksoyxpe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/goyodfhua.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gduxyupnt.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gaslwhajs.sHtML


<!-- 参考信息 -->