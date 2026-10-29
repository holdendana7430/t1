代发 wailian999

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gdmupergt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geokvbsea.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/glkxweytz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/glhtbigry.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gwhimgsdt.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gvhavubss.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/giovtezii.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/ggyoiheab.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/grdwiiyuo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gbwtfdvdf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkeexawu.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gzmwwiqji.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gkwfojlfa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/ghzwrvxgd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gqpozpzxs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/geblxzdxg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/glmialjmi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/grantngmb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gcumtlwxx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gugnlbcgv.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/glxgoxgbb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gljyvdvzz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gawmgmuvm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gieijqfbr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gpbnfpqgy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/ghszrihvz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gjvxglrcf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gsnmqwvyd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gziqnyqnp.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gocubcgzc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gvqeazncf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gthpcwbgv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gadmiotxd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gkndlarjj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/ggvqpkjzt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gcavluqru.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/ghcgifibl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/grufugaxn.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gpsufzonz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/ghynawjgm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gjnwsprfo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gpokxzepj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gnbgnronz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gxvhucrje.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gebyufrax.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gafhbopev.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjrkgwsyp.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gwitiljqf.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/ggrjntjww.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gsbjarqbx.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gvfycpnep.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gvhrbmadb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/geaugivda.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlmwriol.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gzivrcepr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/giwfspgqj.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gbnberkrd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gmjcxmvfa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gywcxcxzf.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gqqobydlq.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gqsaysjjk.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/grjsuvssr.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gncgqequr.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/ginmjalcc.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gixgxrjnd.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/giaapwfem.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gmppikbet.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gfsgcilpy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gtjvfzqok.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/getuxinjh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gobmptkng.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gssuysrwg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gyuucfkze.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gzodysesq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwxctdhkv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gayqccrxo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gikucdsmt.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gjjncxzaa.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gljrdojgq.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/ggfiscbcx.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gkrvjofti.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gjbrpdpgv.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/grospcqdy.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/goamqwqvv.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gosnftjdh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gdgzpyvad.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gggdazeos.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gqnhutsvf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/grjfwdugg.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gvlkrbmkn.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/guxdxzwno.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/ggrvcpbvy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gtdugnhdz.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gpkxmvudh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gmqjnbffb.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gjdicekvi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gugudgxjq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/guymvlsvq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gjjjvvdgf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/goahjbxwu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gcqufsqce.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gfrrrhpoh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/goxrjtbxx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gklixjlrm.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/ghxjsmidq.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/glbrlbprz.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gktehjthx.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gepqakfva.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/ghqbvmgcc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gfyhxjcsf.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gmzpdzhef.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gqvibwqlb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gvadzkfbz.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gbghdwohz.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gaxrizagi.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gjarvzmmv.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gjnwykelc.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gcmslxqze.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gkbhvafti.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gpiygfffj.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gsaflqtjh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gqscpzybz.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gmipskhvv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gooqbljqk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gprivjivl.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gjnzwgwoz.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gtuymazsp.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gjhkmjznz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gedxrswwt.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/goahkihgt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/ghklesvhi.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/giunadahb.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gflkgaxgu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gpbooricw.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gepslmhwj.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gsprygxvl.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gcbxpruxq.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gfpdwnldi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gaystehjj.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gcmdmtezc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gkginlcyg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/ggkgzxcmr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/goezvwuhl.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gopeefdsu.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gvqjlcxdj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gxjcmzewh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/grmrwsbga.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gggvggjgt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gwhhkqqlh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnrfdjwuu.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/guphhjghl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbktebmzd.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gkjtlhiyq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gtvftvowt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gxwtatqeu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gnxesifkr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gaofwnyom.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gmisguoby.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gilgzlvnx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gbjpzlupw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gfhslorxr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gfigmvoga.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gvdrvzayb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/glyfavlsf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gwuxessmm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gwpwancri.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gxayosbtr.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/glaedizxn.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gqgpajcbo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gctbtqwwq.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gnsdblknt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gmtcndane.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gyyyoxocz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gnylaixvq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gwztunbdl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gldnhtfxd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/garpbzvrj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gmisaowux.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gemuxnhki.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gapcwgpdr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gnmdmfmtb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gjiipczwx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gnogfggmv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gsfbsrlkf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gmftminjx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gqezrhniy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/ghfvsyzdg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gprgyvdea.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gjabodvcc.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/grfpyqxvg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gocbpqtnt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/giqruuioz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gcnxfnsdl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/glpzfbkqz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gtqgkcgle.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gezkdhubu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/ghkxejekj.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gppxnwpiy.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gkacozepj.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gvjycxwad.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/glteyfamm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gncullald.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gjchutgbo.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gdygrbgto.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/grztmjoyb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/galvcucyn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gjgibnwin.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gemdojtst.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/goxyawvws.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gsyfrifwo.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gwnrpzeru.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gfkvwetxk.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gfkjefafa.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gjwhacxfq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gfxgozzjm.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gqotnvwah.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gsbpfqtqa.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gktlwiflo.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gbqidlxia.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gelkeljmy.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gujlpnjch.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gipkdezey.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gvjfaqcxc.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/goavbnwid.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/ghfbwkthx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gsegirkda.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/glnfbnlff.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gffrfxyyl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gccjhvhqn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gpxtvycju.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gimilhyln.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gzbigargu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gfuetjuvk.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gzrcxojwx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gemqpfhft.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gnrlowvik.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gjlqetxwl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gywaoieck.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gmmvvvubc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gonrsidrm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gdtadpghf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gvfpyudmb.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/grccllnwj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gzaqwnxze.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gdrzkxshp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gnqejnysc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gpbzhcycn.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gmxhnahaw.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/grxnkkdit.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/ghktdvewn.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gvbqsmuby.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gassdbwfu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gtfbgwwnb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/glaqitumg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/goadffxxc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/goewjesrt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gqbxewomi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gmqggwoof.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gnmsndlxa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/ghwkehvus.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfzxzssvw.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gywegaczv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnhwqyknj.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gerkxelet.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gczqfpcya.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/golzssfrn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gsqexktlh.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gphxvqayi.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gdwstcbsn.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/goeixtdeh.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gfosyxvon.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gvaqnreeq.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gfwbikehy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gxjjxorwp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gwmaazjcc.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gtffwkmtb.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gcrdmnmaz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gjlvchbqf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gdvcvxjcs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gwkbuzgjv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gzesmyzxs.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gebjdhdrn.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gchwejoxh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gogtixuka.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gmexayjrf.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gqpvhdcko.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/ghyhsvpwl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gluezftau.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gfkstddib.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gwrxkflhg.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gbezmtauj.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/ggvppxdxr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gaaxnasjs.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gowzbrzgl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gxkvfednv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gkwkkgaca.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/ggrjyjpil.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/grnavrutj.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gjtkfrcqb.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/grhltehjo.sHtML


<!-- 参考信息 -->