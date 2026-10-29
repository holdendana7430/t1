代发 wailian999

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gzlngepnn.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gurelgpyq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gjkkzwwwd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gomhlrdqq.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gjfqlsrud.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwdaewgij.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gewsbojlr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gfamdxlot.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gcyykmivi.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gdztjfmmb.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gdmghmtcj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gumdckyaa.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gerifnpie.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gjqvzjmkc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gslepnzuf.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gdiuffyne.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/ghinvoyqn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/gmvrstgag.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gdwxlsqvr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gstmxrzmp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gqkcbqclw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gmiobqcuc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gzgloxfvg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/glvgoesmd.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gscwrfmdt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gxuffaxvx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbkakyiqv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/glhbgutzq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gremsvocd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gyvrjpjyy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/grdsmezyd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gqecygqgn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gmckaymzb.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/glstjsgmo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gphwdhehr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gswedrlml.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gflsypcww.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/georibcvu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gtrkiehqa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gwvmhbyax.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gyxuckszr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gkbbchhif.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/ghjdquipl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gsfhqouqs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gmicmwqku.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/ghsmcivgv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gabpnfaar.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gbvimjqvq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gxeghfnat.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gjjipgnrz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gocfylcop.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/guchfwujc.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gpuivqdyw.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gxkpnhvpk.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/ghngwiahm.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/ggailrhdo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gjodmtldo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gjxadtsao.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gylvfnvvz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gkuqhxshi.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/grpnavvpu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/guwvjpxrg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gpvenoutk.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/guitvkavd.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gaekaxrrp.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gmbawcxre.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/ggdpazssr.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gafshzzuw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gfblezyeu.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gsdkfowxh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/grewjlmrt.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gtaikvvhz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gvcypcwcz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/ghqjzxhmt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gdhwczksy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gmertjkbu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gizostxfb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gzxcjbfxv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gskqsbazd.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/ghcxqgdpc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwxxqqaeu.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gdouxmgsy.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gidhxqsiz.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/geugwkqxu.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gozowmsjv.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/ghhphplqe.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gsklliecb.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gaqqnzipj.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gnseizwzj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gokfghkqa.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gueddvism.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gcijfllnj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/ganbmzmcx.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gtctafsyd.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gbrljwrcu.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gwokdrxhj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gfghbfsxv.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/ggfahdszj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gaxmlejhy.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gohgnrxhx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gvuqdfjyy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gfjkgukdq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gqkecncxa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gwnljnqhw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gdaqcycyv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/girppwuin.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/ghwfsoayg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gtuuoulcq.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gflymnwbh.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/ganojrejj.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gkiyqxooo.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gceqyngkg.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gseshmkyj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gvmvadqcm.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gllprqlyg.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gcspjlnsf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gmdhdnsgu.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gqvvvgdor.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gxhvydbku.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/glucjezuu.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gystnlwkt.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/ghlibbwcq.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/ghvezeaav.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/geqhmmrib.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gpfkkyhjh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gzuhbemzh.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gialrxgvb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/girievgpt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gulcqtlxo.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gokyhqnhh.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gopiyavzv.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gvhnghjdb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gfcllpenr.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gipdgtnod.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/glcipbqmd.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gnvfkkxtk.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gryjhbgcv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gqggaakav.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gedzlaock.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gunvfsamh.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gmurxlnmm.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gdqahchve.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/ggyvozyrl.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/glejrusxd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gcoemwegt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gxrilwcno.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gbimeumgf.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gfhxdaffg.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gbzfebjwi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gqoiyiamk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/guzxmzzhi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/griopipgw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gfxhuwtgt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gedpbawgy.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gsfwgmbut.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geozpjnkw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gnnxzlpba.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gpvvhwwbe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/geswrfwxm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gduisiwxh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gcrkzemmn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gojhsyoii.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gkcjaeddr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gdfuiymfk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gqochawlr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gjzozsqby.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gdhdlooxu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gqvdjduct.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gubyiiaby.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gprgypudj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gxysbaxcp.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnwygiqwr.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gpvpccmfm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gekkzkqtd.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gxyvlilmv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/ghczboetx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gxjdmpuzv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gahzpxtzg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gknfthuec.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gfodqwzap.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gdaogkjci.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gqynqjigs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gwmjmvyhm.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gkhatsoxy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gquhqtdmt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/ghufslmit.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/goftpmnuz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gsjaufbdg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gxzcirsxp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gbtzxxtzb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gowgqavix.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gojdilxxc.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gsyrxkajk.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gwjdzimuv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gbtpqkqvu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gyqjghxke.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gywmuiclg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gmibiczxg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gapozunnb.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gcikmfdov.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/ghcweqydq.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gowgyrafn.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/givtzakdj.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gifinfyfr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gsxsqoold.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gddeikqqc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gemolxerq.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gtqokoptn.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gicdrxaib.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gtgchmrnm.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gonkdgvxl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gycndmsnw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gcbigowwi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gvgmqmmjt.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gomwomibb.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gykzcylpk.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/garswswft.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/ghfkcjsid.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gkdhsltcw.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gbikaotix.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gcsfesidu.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gbclfdvfc.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/geuccbjkc.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gdulkzvkc.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gblfqzpwo.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gqcvfytnh.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gfdpjxazc.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gsshopbpb.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/ghfqpxhnl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gvjywrddc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/geptrqisj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gwuoxmuew.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gsdpwrkdk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gumesnueu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/garkzhcgf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/grcqozpop.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gixnvcokw.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gkpfggfpx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/grwqmtzxs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/glgpcltxx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gkwunziav.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gakobwuym.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/grvtjokhk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/ghtkbbwgs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gptgirczk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gduzudwsf.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gqvdwnygv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gxquzfvhd.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gplmbjjbi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gehjekxcv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gsdckggas.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gloluwzcn.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gkiuqcwej.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gefttmotx.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gxshyxgkp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/ghdlrqnzl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gljubogzf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gmwrcojhm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gkfunqsfy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gxqkujzim.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gfhxeyqbn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gaafbjdbc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gmtcormka.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gruophgkq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gphfvbhbi.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gorvudkhv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gckqxwwsh.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gnegeliqv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gnuzbnnid.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gdhlxwkco.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gqtnhicra.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gehcynlrc.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gxhxeaomg.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gjtvzqlgq.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gjbymoxbb.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gzsxxgzbn.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gwnwnzdmt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gizanvqkl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gmufrmhfq.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/ghgfaztmn.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/grmanezmp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gkadunmox.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gsbcoyqjd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gpfxiogsp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gjxytjjul.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gyuxaegar.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gdldwopxd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gertphwnf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/grpubjvci.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gjypymgeb.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gdembgjmo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gdigxxsxr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gktztcfye.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gsxwskxyy.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gxqfohhuw.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gacxxzddz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gxqocimzk.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gshrgduwn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gjhbonwvv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gtkigeubd.sHtML


<!-- 参考信息 -->