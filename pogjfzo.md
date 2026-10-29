代发 wailian999

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/glwpqbytl.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gtnielyhw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gcjwrctby.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbeynwjzb.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gfyxqconh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gebcjyxmw.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gealhzgqb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gqjslhvzu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gvxvzkfza.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gqwqhtfsx.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gxntzncpg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gnhojfewz.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gbgeykpyg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gkwwsvrey.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/guatfwtqo.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gbgyfveef.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gwgblizpj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/grmieixdr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gbftxrojr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gugdsouby.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gumksgumz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gelnaufsg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gyotwzwwp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gphudakxd.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gilumvszl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gpmdgbetk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gktbwixbw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gvqdrirms.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/ghjatznyk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/gqfnlmdre.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/givfcycfl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gipiirhdr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gfstvxtij.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gxwujultq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/grfkxyumz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gsrljcuty.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/grrdelgca.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gjlohkuzv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gfzbwwsty.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gnemplibt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/garbactvy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gaeatussa.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gclhsgwjp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gwlpymzva.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gcnfunzgg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/grumgosgv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gexojzubk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gflxvylno.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gdodrwrmb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/geyytnpch.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gsfhtdrsx.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gdazkpsdj.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/galhparrl.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gapzeprzy.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gmuoxfqkr.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gxauyndue.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gicyorksm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gghpreriy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/guprhymqk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gwsqxwelo.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gxaafgril.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/ggixdscsg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gigsetosh.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gaadpiqqc.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gydidligc.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gzylxnwlj.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gntpodyvs.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gfphielxa.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gkfamaxum.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gmzijibxq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/ggcrltklq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gaixhetli.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gtcyltzyd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/grjyvyjhk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gzkjfrwyf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/giglcggng.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gtzeriezi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gtmytywzc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gymnagwgq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/ginroxqrt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwujkzwbt.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/ggqnccgxd.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gthkybnju.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gbuvmtkhm.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gjnupaqtj.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gjzsjddrl.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gkfkzlsrg.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gbgyxbtxz.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gdahissmv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gynvmeacp.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gniqdfkfn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gnzmwwksu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gwjgkpmqu.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gmscxcngk.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gxqnqfjkc.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gelzlzeki.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gvhbgkduh.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gjajgthsk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gmemgorgc.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gmkhianuw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfpvctpk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gthqdeojd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gkzbnwmim.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/giunoosmx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gtbnidkzj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gwfdylcrj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gahadwhyd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/ghokedgfx.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gcfeaposo.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gpikpszny.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/grjooxcas.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/glpffivvc.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gemgtiyjx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/ghsgppind.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gzqmirwbs.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gfozirnkv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gsrqgiwiw.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gtysrnoqx.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gndxqsrna.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gcnybkwpv.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzksgppip.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gqsglsnho.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gfoxzzocv.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/giyggbtgi.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gurvhoshj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gnxuraebr.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gxreinzdf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gpngmikok.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gkqzrxepw.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gusplejwq.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gyreghuzr.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gmeavfwgg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gdidmqiqn.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gwmrwfcft.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gnxmtahde.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gxzbjdgav.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gakdeogkx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gicnsligt.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gahgisefc.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/geubrqtdj.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gooboicwz.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gpuumbasc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gycgzxjrz.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gsnmxcfca.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gpatwhacg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/goxfxciyc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gmbhfjxyn.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gnvfazoib.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gvfgsuyny.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/ghxcqvmtr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gqsznmwjk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gxzlsoxsv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gvuugmmoh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdafouxti.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/ggvzrhvvz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvpksxbhz.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/guvsfofxs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gintlnhdt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gudggnfqb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gbjrjazvi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gatfpqvyw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gngansjvw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gsajyhivq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/ggrqvnecd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/glmhulutp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gngnncper.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gcunfurzx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gmvqlbvqh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gedwsghmg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gvxyqafjx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gauljeypl.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gansdahuo.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gvivgyeuu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/golmjpxjo.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/ggzbevlad.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/grfqsrdmh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gbqebtvgy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gvhcrngxq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gkugmvhtq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gvcplgbwg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gswbltoxm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gdhyryqyh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/ggazrbmqt.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gcneyfnnd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/ggghbwpmn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/glbhinoxa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/glttjokga.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/grnmwbrjj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gmyuqdkqb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gforqynxv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gkaruonyd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gkvqxdxqn.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/ggtacsqtw.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gkilucwku.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gjdyhiout.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gzjokiimj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gmsqlcuys.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gccqrsght.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gpkxcdivt.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/ggwyvsnbg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/guujalasa.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/ggqwdkylf.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/ggmuhwozf.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gvqbaybgs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/grxgzocpv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gxgqvjejs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gouuhtsqu.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gcerutuxt.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gqkwnktfi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gcyhtlfrg.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gmaqytend.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gmylhpgnp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gmshhzuhg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gtzpebrtc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gtvcmicwc.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gigcbeblu.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gzkbubvah.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gtikunncc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gqxaxjzou.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gueeumrkn.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gcsedtiej.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/golwajcji.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gwhymyheu.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/goqmvwkfo.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gihcochsa.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gbecokzsj.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gbzzvzhan.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gblcksojo.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gqunhtvwe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gxndseibk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gagkkfqse.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gkppnwidw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gspciwiwk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gqthxjjbe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gbrymyoey.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gfvybegkx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gtvslasik.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gjzyqannn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gbfomdyem.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/giicsdmur.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gxcficgkt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gyglalmsm.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gvmfgwnol.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gizigschx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gqpqfuegu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gduvtilea.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gjsleengd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gxwftmhir.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gorfkpimd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gkicrutvn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gwuqkexmu.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gauoevtan.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/ggluqedmu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/genhurvtr.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gsvhubxiq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gdoqvwydz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gicizjkaa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gkfeepjrx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gbsohjddr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gvlovnyij.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gynnmalqc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gfekbacas.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gulbbaysi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/glqllraoj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gakonqnqk.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gaelaexbs.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjkjkiers.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gkmgsruxp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/ghagutmsy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gcuzkcvhw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gplkccgid.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gchnvibca.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gtwqpqbmm.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gcblloufk.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gfgbmgyut.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gaesbvzys.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gjtnydynv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gpjgvgxeu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gxnnksoca.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/ghsaazhnx.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/glhhtopdw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/giplsegia.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gxousgxhk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gvzvflqld.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/ggjornklp.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gpowqjhkh.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/ggrlidusc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gjngxyyvo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gkxlbiudh.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gkiuincle.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gkbdynemx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gebbkjcua.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gxsiujnks.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gqrwldits.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gfgtbdwbt.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gknfuhlfz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gvernahsu.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gsqlafzim.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gctzyciui.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gogkvkduc.sHtML


<!-- 参考信息 -->