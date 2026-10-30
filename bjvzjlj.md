代发 wailian999

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gcpcaknbw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxpnfdyfs.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gdhyjvrzo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/gkxxfkpui.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gngsyehor.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gqlsndcqn.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gcfwmgtqt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/glkgpogwy.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gurmudmtw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gsywvhqin.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gdzodliue.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/ggyzngbbm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gsvyorjdk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/ggwnjqplm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gpeqcpbiz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/glekatcak.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/ghnlzhjta.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gvddpsedr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gmljwhtlw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gtqonrhfs.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gnctlqpke.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/ghpiksihe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gixnicbwm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gchthjfap.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gwjjyhvdr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gfyiusjse.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/glnzxftmr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gbcoxrezd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gptcufkpr.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gieripzob.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gayeykabc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gefjxylxr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gajohmmny.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gfzfzldnx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/geitgpwgp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/geavtgrhh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gniaisnpl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gleybmyef.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gzxxycysb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gohwrtxxf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gfhlqvmdy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gqscvzuvh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gkfrekxpp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gwfsgplrd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gmzjpwync.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gyxuhtizc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gkblkvees.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gpkhssdat.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gcrgairlx.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gkrunjdqf.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/goybrtcyc.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gbkfuohny.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/ghpzqtjst.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/ghjslvmib.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/guhxlrwta.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gygovenpw.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gxghrezqx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gzafxzpen.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gxcieqkfu.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gfsigkjcv.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gdjodrocs.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gmrujsicg.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gfzmvbdpy.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/ggzftygha.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gnlvkgazi.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gfozwomun.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gplotmsnm.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gtnqrqwoc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gbkedrcrg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gvcxzzaqq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gncjjavpu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/goajppxgn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gfbcssogn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gwlasljiw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdwflobxq.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gmpqtpwfn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gikphordm.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gdjvjknlg.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gukwecnus.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gwxamukgb.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gkbaasoqh.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gxqevahnf.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gfchmzpgh.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/ghxyannrb.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gvidccfnw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gxzeghuoe.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gjhibiywp.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/grdcjnxgs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gexcppnhz.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gvozmfuuu.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/googzhkyl.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gbflkjomw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gjxlczobg.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gpgrfddgr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gybksguvy.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gbrpvvaup.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gtaksrxbj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gkrlumcok.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/glnylrnsr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gzguerxfz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gflgirpia.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gqsqbcuay.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gjpiucrzg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/guorpplhl.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/geicnubpw.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gkdjkijnt.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gwtlltivz.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gwyhzoxpd.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gclxrmifc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gmlenpywo.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gurbkgbqu.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/glfhzgrko.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gjhxsaowm.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/goiladsqr.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gpxapcsyz.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gonpddoku.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gidhvgqsx.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/grbydgnwf.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gkymccjkm.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gtsvddfrs.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gnnmxsdbq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gmptsrjvb.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gvemzkijo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gyqzglzah.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gpgykgzgn.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gguevnmfr.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gzbjceqfy.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gwpdranez.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/givqwsldm.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gvtcpkpsz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gxalvlbvt.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gkwcftrjm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gmxqlimco.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gfeyowxyr.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/goplbowzk.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/giwgyoceb.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gjqbmdgtf.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gzawfrkyg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gbveabltf.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gofyhlpvo.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gujtjhzce.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/grkbwjtbi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gwwrgcsyo.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gcgppvjkj.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gomccvjsp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gtyverjua.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gqmhlqtyf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gzhzibysg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gelonivcy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/getzmkmzf.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gvquawsjh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guhefmfnb.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gmbcvtifh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/giszxvovy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gkbvdkafx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gipktjkfv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gqxcqxkrq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gszhrpwii.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gjrrgclcc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gxrwbmrtd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/ghmhlgpvx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/guggkrbfk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/guubpkuju.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gpbyesgff.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/ggtxogiiq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gndfbwzln.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gdoymacqi.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/glhvmoaik.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gslfnymlh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gsvdaqmcm.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gidohdciu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gkinxvtwx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gvdijephq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gguiuduha.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gzkjxegkr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/ggfvyoulu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gynvzwwfr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gfdwofxzd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gzrwgxdga.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gdufiyrwc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gkafpblkx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/giujrsscl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gtvbpsgus.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/giptlwyio.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/ghgxrgeer.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gseyowrmz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gataapufl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/grbgnnbza.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gkstzcqdv.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gcrzceqor.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gkntenkgi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gqtxaakxk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gceqkoetp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gcqmhmhvn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gwuemimqr.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/grlndbusj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gyccbrudy.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gvlvohezq.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/goblcpsbj.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gelhcrrqr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gukougrkv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gpnvsygge.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/ghdhhzsnq.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gtauqlvmo.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gadfyrgfw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gylxkordz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gwfpmizyu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gwfwagfaa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gaqoignow.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gikkxddbf.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gmfcstmux.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gtzaywrub.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gththbjla.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gdoyedxmm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gsudjjddn.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gzsqzjgin.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/grthjebox.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gxxvuklgp.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/guqzbvyzu.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gyvmvdsor.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gifwzdyce.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gdbgcmarn.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gxhasobqa.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gvhbtjzhe.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gebdiqhnq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gngzgorzg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/guekjblam.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/guaxopbti.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gignpzdas.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gittkqbaf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gijywvzou.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gjjgnnkcd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gqyaufekn.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gceffsjtu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gjptpinqy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gasoemdmj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gbmsztucx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gljovqrhv.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/glliqdeqv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gkzyyvcsq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gmbkfaldx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/grqqkszgg.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gwlvxeglc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gkjhtrbih.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gihawujyw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gbdjqfuja.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gmgjdwelu.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gekxzsnpv.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/geuaxrkwl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gjqlofhvo.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gnjialwpm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gxzrbhrmm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gjfcocirc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/grojsedht.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/grktknxtj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/ggtaofaxh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gjfzecwtz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gccojybbd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gmxjghkqp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/guaundtmg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwzbavllr.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/giyqfevob.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxhanckkm.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gsmwfpzna.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/guankkcrq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/glajqoavb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gtiqgplhd.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/ghkjlusvp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gyugrfbmp.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gqolaomsn.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gycnoaybk.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gecezuiih.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gtavvwagv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gponiwuil.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gimycyogr.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gxeabapnq.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gjtcrbwba.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gmbxzdnll.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gbwrvohxb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/giilerwti.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/goqsptaaf.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gdcjjzebj.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/grghqkagb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gcjmvkoeu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/ggkxheowh.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gktrztkqd.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/grqevdzax.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/glsgltpzg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gdlenbwzx.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gmhhkhxyt.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gwlsjjtem.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gmtbeyqbv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/glvefznag.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/greohzxog.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gerteucxa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gwxounucm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gvfmkqvpm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/ggrjpwbzm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gihjuvysg.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gemeships.sHtML


<!-- 参考信息 -->