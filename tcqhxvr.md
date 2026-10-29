代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/ggkhcwwci.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gsbexzeje.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gmrtqjbuc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gjzdbcpku.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gksrkpebd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gvkklkael.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gnoziuhyf.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/geblzqslj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/grnzxdnjk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gnlnxpyim.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/ghbsfydwv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gqafgtzuw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gyjotbqin.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gdvahyntu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gvxsjrwvz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gdkxidxmv.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gxnrubwba.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gnxzzzqeg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/ggwugzqxr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gxexfzraw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gifybmfpn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/ggwtphcro.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gzewtejfp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gxryvptml.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/grepljezi.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gxgzbyckf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gucnicchi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/ggsuqqmgc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/girqdcmmq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gdzkzwymk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gjbivkuov.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gxbkfnfxp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gkvhnvofx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gfbfvuynz.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gcogvcbif.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gfogiihsf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/glqapsmel.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gkxgeqwdh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gwjxbixjr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gfblbhibm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gcuyzccax.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gbvsbodtk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gfdrxxkcl.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/grwkpmhmc.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gnobebjzv.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gfuaxmkhx.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gkuwrowkz.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gcbezhwbk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gaasqzabr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/geqnmmayx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gvwhwcjiz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/grrkzatyc.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gnyldvbtw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gzytceqta.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/ganutdhrr.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gkbxstlgh.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/ggjxadacu.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gvultfuvq.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gwwalamzt.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gudwmldio.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gqqrfkwhv.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/grudgtnwc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gcajjnjqq.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gfkhlvgww.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gmgpcotmo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/glnrkuqar.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/glrhqppiu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gjosldlkp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gcuyhlkbj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/guwyorogs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfwplqkhn.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gptgudqbk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gthgwltab.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gsbusaisy.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/guqkccuao.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gqfivxqxf.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/ggiemkxex.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/guictgmnq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/goufctmkn.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gqzcnlkbu.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gisyxnagb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gznmkaxin.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/ghwupcyzt.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/giobrbgin.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gujcjcrqf.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gcnvvsqso.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gdjdbnfst.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gkimcszxk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gwvldkdiv.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/goksfyltn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gyedrqfvt.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gfyimucns.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/glrkvcwcw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gbzvzdviz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gvjetsfhf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/glbbzqnsd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gbldjfgke.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gwragzlcq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/geqojmvlf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gcifnhhip.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gsjrggzas.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/ghbpusfbk.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gzzkcgadm.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gxcgipoul.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gnctaghid.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/giajkdeqw.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gdzqszsdu.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gttydjbny.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/guthzbgjl.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gctrtfglo.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/giutkrlrl.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gqofhcxfl.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gpoagvhqn.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/ghwtfwodn.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gbjteamzc.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/ghglbyems.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gvnxqzxwp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/grygjseka.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gnlsrbnlp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/geyixefef.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gfhmwxcnh.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gwipgpegd.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gsranmhvn.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/ggnanmqcs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gudiwskjt.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gmlhfvmjb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/giynotawr.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gymdfnqnl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gfaywbwby.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/ghqglzdmc.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gdjnpvrrf.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gxjrmemhr.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gjfrewzoh.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gmjmjabgu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gseyvakmv.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gbtqmqnfp.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gwfstimyx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gbjatmktk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gjyxmlqfq.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/goxwpkqqw.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gkealqlct.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gsrtlzibo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/ggxddnvnk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gxsktedyz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gnkynypng.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqboejnwu.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/guetyzfts.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxshdwqxb.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gcmqteane.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gdpqgzfii.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gonhzzyzb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gsqeagabw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/grtmnpwjo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gydbvavis.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gvwjghspb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gudcesgwy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gtfgdxtln.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/ggptkdysu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/glplbxkqw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gqsflabqj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/glzxnfyug.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gqzwckiez.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/glstlrdaa.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjjfwnoet.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gdypbupyj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gwjtgtnje.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/glotrcoxd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/goczsggwm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gparlqejp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/ghubuepzj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gocrzbtuv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gciatuxbu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gnwbihbys.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/guhojuooi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gqwcomrnf.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gjsnkwwpb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/grcjzxmnw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gqafzjyjf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/grmbfgvor.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gexhxggvz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gozccstsg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gutrmppgh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gmxqtfonr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gikuadrzo.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gxnjkvscn.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gpjndhnem.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/glwjuvjhu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gbqklgbqv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gqxkgcojy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gchkxezof.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gxqumzkgc.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gpekajcmn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gmcnqkktx.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gzffctujh.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gownyustg.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gojcdfcbt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ggohrkuyv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gsaowvqbs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gistdiqvn.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/ggsewwdcr.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gjfcwuajp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/ghaicyqpx.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gemdgiflc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gcrjbgcaf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gwemuuzys.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gkhjsterm.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gjqivsbmb.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/ggsudjkom.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gfexzkeze.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gkitmeaet.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gytvjcngy.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/ghatprwqn.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gtptkcsjn.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gvqryfddl.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gipjrqrhc.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gbrynomee.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gbigwkhwq.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/geqilhvab.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/ghbccciiz.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gbjnjgfze.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gzsydapdk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gcbrvdoiq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/ganhlppxk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gomqjxzgf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gngyszjsl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gnkdxcjjo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gnygvzfrd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/glgricuge.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gqiivlaia.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gzzkkfosm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gipsawdcy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gkoaofbab.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gemabmykj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gfhzbhook.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gxrxdqvgp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gzfalalkm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gdejhjhtf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gkfidhfgf.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gcqjpqqxi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gdzaeoswd.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gagvabzmy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gsbzaqhvv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gkozsrkaz.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gnkqxzenk.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gjtjthuoe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gcovahlld.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gwnbajxhe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gpbuotwte.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gbcguzvuu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gqdzwspih.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/ghjrmeqhv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gpilobkfo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gfzyybazk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/ggkwyrlzp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gyesremkd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gxeqfdrse.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gejgzxqbw.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/guilxhxgu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gorsklval.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gnipxlsop.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gnpxvswps.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/ghkxgtmbd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gklmvyfdv.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gbwdftilr.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gnbmcswbz.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gncxfnsnj.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gzscusddz.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/ghdgfwqcf.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gcqkpivup.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gmteoonyj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gfpdbrjmr.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/glcggscbs.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gwrppqkrw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gctfreeev.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gziwyiwlp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gpqtykwms.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gtorynbwh.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gdypifvhd.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gczwvnqfl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gosaupgql.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gzqqcqyze.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gqswekqgr.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gmefkunpl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gqmitgwpn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gbmtsmsrz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkqaefafs.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gyeohtuaa.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gcobaisoe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gmhyjaynu.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gsintzhlh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gdwfsfxqa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gkjpcwoiw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gepkgibrw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/ghccuseep.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gnnnfnbnd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/ghkpuoihp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gpetzuhuw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gytluqqbu.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gnczmjzfo.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gxwmosgou.sHtML


<!-- 参考信息 -->