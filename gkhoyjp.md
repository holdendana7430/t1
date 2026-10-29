代发 wailian999

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gmzwmdklk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjqebflff.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gkqppxmex.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gxdtzldws.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/guggdksll.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gvxfdfffd.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gnqznqfem.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gyebmesrz.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gofvikusi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gfnvqholk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gvzbtyzkw.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gzscjesad.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gylayhypo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/grdyrfdkt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gdwyaivbl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/glwxsgfgr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gvchmxkot.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/gsxvxubhp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gsjcnnrpy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gcboqxfzd.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gjkgzqghx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/guabanewk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gcbokfscm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/glkcbizzk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gncnpytml.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/geyxxcekq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gubtikmel.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gygioblci.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gnnlfqtwy.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gzcdemeuh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gkkwtaccv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gszotjwix.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/ggqgnfsrq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gfbjornqw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gjtrgmjls.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gqrelkzwt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/ggknsoosr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gcrhgxamn.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gczuprkiw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gowingyny.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/ghaqnnnpg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gtlwdyrff.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gjouhnmlr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gxgwfbqyj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gomyxbprd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gruprkebw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/goqsnhnec.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gugsqithm.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/grzpadblz.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gcxybzaor.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gmgzsrsuy.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gfnvgalje.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gazbwtekw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gcuspmjlg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gagokpxys.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gqvqcxdun.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gezcqiclt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gomitdaqy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gfdfzauga.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gkfbxweng.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gvuropvsl.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/ghszufokg.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gxefpfwpr.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gsfnadqhv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/ggjpywqtg.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/ggtgtfxds.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gkcicvljk.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gavwpzqzi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/ggunrlcos.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gipodexwr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gaewhwhid.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gjmviuobl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gfeyivjcb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gpeiozyjo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gptifijra.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gmfoqyfji.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggxomimfi.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gwstayren.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gxklibffc.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/ggmlexeeb.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gtscflwpn.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gbkwbarrk.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/givpfqiix.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gckmuugva.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gqqbkfdql.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gorbnybea.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gbmhtjqrw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gzykchuay.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gdidsbled.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gouchirww.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gitlispkz.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gwjugthoj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gcvgdvnpx.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gflzsmzez.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/geczpfzav.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gveakkbqa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gxxkeypnu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/grocvtnad.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/grjlafryf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gcrxjrszw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/ghyevjqip.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gpuxtejpl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gkcepypoy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/ggiszgvly.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gwroyroob.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gepksvver.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/ghshycxer.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gdthitgei.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gxzzjmaya.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gjvtlcuip.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gjrstbajf.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gstpmddru.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gcmexlack.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gjeilxkvp.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/grwmmhpko.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gmvxycdff.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gopzcgldd.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gmrhjqnaf.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gknjmkycg.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/ghmcoodfk.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gkoioxlgt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gydmirhzf.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gwibyclby.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gwvgmhnlq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/glpuntuct.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/glgqduxta.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gkxewddvi.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gwftrwwce.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gogvnzahx.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gdcivfrth.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/ggagwlxlp.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gtfxwpqpa.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/glheumozk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gnmlcqpmg.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/guigdxxgo.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/ghedaktkg.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gagmrcplw.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gprrcinbf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gwjsgzqxr.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/ghqbiugpf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gqpoliosp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gcliwthpn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gpqlgzhyc.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gsjjgjdtn.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gqvpcvdke.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gnmcvijsv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gppbrvwta.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/ggulaipla.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gktqisbsp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grklsofhk.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gdhzcgqhu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpctlypxx.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gmlucohnl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gmimfqdrs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gfzqftzbw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gceirgvnf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gvbzvvhpy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gxkepydji.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ggwjdykzw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gxxszwngl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gezwcrdnr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gurqghdxk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gxnhxurbx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gdzohctlm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gterrlpgv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gjzdtvdub.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gijbhtsag.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkbnrklid.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gsqvwpkro.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gtwvkllip.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gfrzilnpc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gtjbbgqgd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/glkiccjbg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gozglfzrc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gzhvjuhid.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gnnolthat.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gzdyflhyw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/guuxppaqz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gauravnhv.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gdbtgkwpc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gytkrzpzj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gtnymxrud.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/grhgwoqck.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gkxnqjezg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gzzsvbdtx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gdnhewjlo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/ghdyidcqw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/grglqdqqa.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/glxhgaisa.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gzhcwdamk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/goajloiwu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gglkogpdz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gvmzqdhde.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gopyamems.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gfvviwpoy.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/grvwppcet.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gdjebktkx.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gbjudondh.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gqnqyjzbi.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gtcbkpilp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gpkpikhrf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gsqwogmhn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gdsslfrdh.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gsbtlzqig.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gryosiwmu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gadoywsxi.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gvxwrpfbg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gkoefhqmi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gaynivsqf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/glzdowjdr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gsdanjqbz.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gvrfakahf.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/guneiefdj.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gjhvtlpxm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gmiutmwjn.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gyncddvse.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gpyxlyrzu.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/goprsqiye.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gymwbblgh.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/glkcsnvaz.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gxtnglegr.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gtbgowvvq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gvpujfyqf.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gzindhaqx.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gvaehlvlm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/glqfobdbx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gcynnpivv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gymqlwcrc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/garlyvink.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gcrrwnehu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/glbbbgojh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gaopzrrpk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/galochqrn.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gtwdhiaxi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gtkcytyui.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gkxglpjcg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gmlhlfdrc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gbxitdysw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gtyvzrrip.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gtgauoxia.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/glcfpphta.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gqpmruzea.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gvxldjddl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gupdygeov.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gbuvdzspj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gmgecgdur.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gsmhmgatq.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gbiahwiny.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gffjshhpy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gtqiavuit.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/ggquroiyg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gffuwfjey.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/ghflrpkpk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gsnhombwf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gcosmomgw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gsglbhoty.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gyeqjyhns.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gbzabslnb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gyblczahm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gfnxvutlj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsxldldqd.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gognytghg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtcrznrad.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gatfziwlt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gzfpbrwng.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gumobmmun.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gglqiklvj.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/giiwplwsn.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gvrrhcnoa.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/ghbidtgic.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/glvdhgfeh.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/grxcrqtoo.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gwrzxcwig.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gqnlmnmhv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gxgloksyc.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gkggzmznb.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gedsrxrgh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gphbyezwd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gqlcnmefo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gqwzcnbzo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/ggeqjuagj.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/giupgnjin.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gsnktocwk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gkmaujjjk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gcrpydyis.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gkiwqfphz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/guhdmutoh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gxrsvteye.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gqenlpdrg.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/guwhijdjx.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gvsmzsxzg.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gmwmxcutk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/ghdnpjzqr.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gwugxlrcb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/giiysapay.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gsrmgatjs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gcdpqrqjr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gtzqxpzkh.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gpqpogexj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gdrepdloi.sHtML


<!-- 参考信息 -->