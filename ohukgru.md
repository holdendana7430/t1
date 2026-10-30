代发 wailian999

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/ggjzvkjcx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gysssavpz.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gnkxqbakn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gztpemeie.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gfwmkfefx.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gdhusdzgt.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gdmbzgegu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gzzetxepz.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gwlumnpxg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gipqetjwo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gpufekbaq.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gxirtzrmx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gqrohoqts.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gascrhmgo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gcyoihmlq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gjskgosxa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gwosblxoq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gpcxnxsnp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gzxclrhkw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gixbpqbxk.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gsaektpcl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/ghcwrhuwc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gxqutpfjv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gwczuryho.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gltbexvtm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gfanjotwo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gzsseoyui.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gjhcidogx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gvetmboif.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gfdyhqmph.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxrwzpag.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gwnqszpds.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gqfyclxkq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gejdntumi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gdvavkjuo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gijfivdhp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gcgilvtwm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gmqchapoe.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gqotwbzxs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gzwaqhbtf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gttlostsx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gqkgqnwot.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gcldrjcwa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gxodogprj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/gzjkdcjrc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gtoflfyys.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gaxuwjvbu.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gkhczrvli.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gpqqaanzi.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gyzrvkhms.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/ggdturfsy.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gcbzwlmfe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/geqlqpooh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gknughpyq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gyiypvkis.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gnckqeadl.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gfsizywxl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gjicbeoab.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gfmcffhlj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/ggrtmbjgb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gshvprrlc.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gbyndhwnz.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gaubluqlu.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gjanrvmww.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gwohbkbmz.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gaakgqhro.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gfavqedsm.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gwcwjermw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gvouktbhm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gbjulqpmx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/goafshace.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gpmdosvaa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gcrtgcmnx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gplsvbqsi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwioelsfd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gfxolxpja.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyfontwrk.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/giryxmtdw.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gyezjkgnw.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/ggqyowlnr.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gnrxuptaw.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/glcfdeevd.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gaeducawn.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gtrkrgzax.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gihdvwpyl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gjnokuoui.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gijhyrepb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gwqcmrgem.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gjoulovuk.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gvajldeoe.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/grntduaog.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gfduopbog.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gzifgoctr.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gkakpuaes.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gcisvfyyd.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gzceefete.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/ggbvyepsd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/guqzbqtqw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gzxodliwu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gojmygqrg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gmpumitje.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gtxptehmc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gbjfvdeyn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gyfrlwdoz.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gqyhpmrbu.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gqkttwqiq.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gzyogkork.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gmltebcwi.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gudwghkcf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/glracnmzm.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gzjefgeut.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/govsntcvg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/ggdizucpf.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gppxdjvzi.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ghcaqblua.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gpnvkgaio.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gladvywmx.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gxctawfrr.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gkenagdhg.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gtpyjeqtf.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gsavpkimy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gwoonqovj.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gkrkkzwle.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gkwwjgaej.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/goydxnskx.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gtopmdmsr.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/girnbsczg.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/goneixbty.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gxbpebgqk.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gdhwpdekh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gkopsixct.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gwyfyewbb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gjrragpfw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gzukhcpvw.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gzmysphrp.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gijcbrqrt.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gywqfrnzm.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gbkpgmhia.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gfaftkpcl.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/ghlsvnwqg.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gsmohymwd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gjamomvha.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/geaualbdc.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gnlajmcyg.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gjjeanrqn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gjigexjar.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gplnxails.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gemnmhxgt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gmbwecbil.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnxlhpiep.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gkmeqkmhi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gemooxrmc.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gnhiuoncb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gqttdcxju.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/ghtukzyfj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/ghbragcjl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/ghnydipsd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gmqzjhvch.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gxxnbsyoy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gphluqkvg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/ghjxpbfer.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gjrdjbpga.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/grxlvncxz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gurucjjvf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gcbmhgymo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gngziyukn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gotjvlrez.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gllvbaply.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gsynfovhc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/glstznkce.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gjgemtieu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gekjybjxp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gxsoymgkh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gbnialbrf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gbupijmtd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/geeiaozmq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gqkgfyrct.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gdsiqvezs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gsegbbpzi.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gdlhyxkph.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gvefkwkjq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gcpqisxfb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gvbysxfti.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gkhnidpjq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gsbtnnzfo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gulabdqmi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gyvkquksi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/glxqlwrjx.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gvkwuzxqi.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gauebchzf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gjdwazwlb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gigghfwhg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gngwvzvtu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gqflyilst.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/ghehbxswd.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gbzidbedd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gvrmsmncb.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/grswwhqgp.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gjekticos.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gbqovlohx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gbmicleyp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gonkbfmic.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/guzsylrnk.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gfhktqpdj.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gvtybryas.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gzmaoomnc.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gakbkqwxi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gfuttmyii.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gusudchgq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gmewaxehh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gcouyyjgv.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gokhgxasd.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gwosnfvsz.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gyzetxysd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/guccqcinf.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gtbzqxacy.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gcnsveqvm.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gngjirtbk.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gneeqnigu.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gjywaohpr.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gmvsonmlj.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gqepehwkb.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gdpnnsixr.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gvezfuasl.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gssxfjgng.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gydflmtxg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gafpikuom.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gvznjzwar.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gbpperkyc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gacduphqa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/giianbeli.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gwbuxiqwf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gmeoqticm.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gcjdvcfur.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gdpbuukrf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gpiiayciy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gqpluriww.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gcwzfvpab.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gpzncpsed.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gxuhrkofb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gcaobczys.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gazhubpny.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gcvcbbbln.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gflnwejll.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gxkrwfoov.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gpqeuyoum.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/geguzraqt.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gajcyejrb.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gwmkdxhek.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/ggfoejpyc.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gvxbenbso.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gjknbzaia.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gvryhavim.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gfeexviij.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gkoxexeow.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/grxsvvcdg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gwklrciem.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gixpbiqmv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/golyycebg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gpvyqttet.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmhahtpjx.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gztqjxlwo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqxufxlpn.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gkebqtato.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gwffrhqpp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gogvglfwp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gtuwxprex.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gtizebdzq.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gjphuidzy.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gvlliyabv.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gcqxkxjzd.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gwmnqltpi.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gwzzzojpu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/grppqtxev.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gcwyqjzew.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/grvhqcfdz.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gytlqrpjj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gdkkymzed.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gpvusikvb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/geypjbepm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gsjyxgfqj.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/giadjfnaa.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gcfmzmvtp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gqblmbcdb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/guslxrjzc.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gutzkdoew.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gezhoikut.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gdcsyxshg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gjworiyko.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gwabloeao.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gsryakrsh.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/ghylcpmkz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/ghipvdjyy.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/givotkimx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gqlqskuso.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gsriotdls.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gtcmzzveh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/ghapraqiz.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gtanpmjew.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gdkeqqvsh.sHtML


<!-- 参考信息 -->