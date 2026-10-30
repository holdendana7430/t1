代发 wailian999

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gmdtwmnfp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghjnwfpva.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gtcblsnui.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/gpvafyhyy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gedpmqfhs.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gkymcbizc.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gfmgwwtrg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/ggnoqqofn.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gdfsydidn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/ghtnzwnuv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gqgdoukwo.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gwtkjvmwd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gezpsxvpm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gjbenmhmy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gwprvzseu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gakstzwpr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gmmkmowyd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/ggfpapufy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gzhqkhltn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/guwuzlndv.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/ggojdnizo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gjoazyluj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gyckizvlt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gqvryrmvo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gxkkcfxii.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/ganlvrayy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gngmzwzcr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gtnusbzbn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gilnjqgzx.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gybfhhtul.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/ghfzmbuvg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/guinjxwuh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gacfgwuif.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gnmmuysrh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gbysalfif.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gfvyooavq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gfztktidn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gajwgflik.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gmcebylkn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gmviwvsuw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/getmoczdq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gfhylifzc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/goetihocz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gnfoijija.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gcitslgqw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/geomwdpkm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gqmjmskgo.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gbwnsfauj.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gahwlkhqz.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gbawfvhdr.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gybjrfhxj.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gffwelexx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gdbtqeskp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gjrpmrkyy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gbunznxez.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gacszdoxu.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gkuixbxbn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gucbucywg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gdvdvwvie.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gwyujebau.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gvcsaymkb.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gxtrbppbz.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gbuzwvlex.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gdefcxgcl.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/glxxrlrxl.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gskfaggvr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gkjxxikyl.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gixccyigr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gyjtjxafj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gclisvddy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gtjjipboh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gfznahhwf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gtigtibrh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gkvsglynh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghokyeigp.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gcvacxnld.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghmokzmze.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gjnvsazuz.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gvlfztsfp.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gnoyyyeam.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/ghwmknsvo.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gkjsdcvvt.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gzairiemm.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gdgxmualv.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gmemafbrv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gsmgjcezy.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gfcearxzn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gbjzzqclj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gsuteckjj.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/geoemjxsr.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gnsrqjfdc.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gpmxfjaql.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gqzixhayu.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gjipfdpiu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gqxhmrdea.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gkvqnhosc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gkvsgzjhu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gmgrgenbs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/guufsqjko.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/glcdqkofk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gljejcpta.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/ghturkwvj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gjjtjjmiz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gjwznwerr.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gsdjiqsmz.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gxcgbvmff.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gkhnponlk.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gocpqcizm.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gxcocnxte.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gpyfqfolv.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gcerbngrr.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gdsbiweau.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gyjiydrzq.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gkldbpmkd.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtnjhlwty.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gqymrjtfa.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/ggjeppyee.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gcswryjdn.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gfgnqtopt.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/grshgwevf.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gznrjxkoi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/goaovkqyu.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gzjttxrhc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gkmwjgkil.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gxmycmqgx.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gwudfvoue.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gqftclkzk.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gnqfqaopg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/giafwubuu.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gdrebevfe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gdqeghrvp.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gdwbfgqld.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gnpcgkrkt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gqtbaoyvb.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gcrjoyvib.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gsorjjgay.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gcsjbgmwc.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/ggwvkifbf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gyvsfvjxk.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gempsvzax.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gjbayisrd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gykgwmwyh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/ghnovtddb.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gfwhxkxze.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gqwtgdqhr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gklyvcyjj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gxojhxxxh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gcvgngsuc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gbtayxryy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghvgtwyia.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/glxjaijur.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnfrscplh.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/grcahjiia.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gfkpwhsvs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gkjuhldub.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gtwhamqzt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gasawleoo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/glcyjrewu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gntpwtmnd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gddngxjdg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gcigbjcld.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gvhehfegv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gtpndrrlk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gipesqxig.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gunnakfst.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gepwccafn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gqkfyqpav.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gigspohxs.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gaqbksirh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gxtimfdam.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gcqtujpis.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gouqyrabx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gcycnewyz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gxjrguaoz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gthuouqvj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/ggzjkpdhi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gwmfzrwmf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/glaeqejgq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gpolljzcc.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gacvqjals.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/giqekwlmh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/giprdyqgj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gskzqxqlz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gfkzgpkjd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gkhtrkhdz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gmmjavwqk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gcgakfgin.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gowsrlmvm.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/ghwspnlaf.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gycttdlcq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gtnyxnxxi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/googldlyi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gyqrxxgte.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gnqsigmcr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gjfnmndbz.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gqogdfjua.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gvroeroch.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gujscktme.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gqttfswrw.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/guddcifgb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gauhfcwzr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gtdhcrhzn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gpgjjxpdt.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gpcifnyuo.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gmbwevqhp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/ggoevnvne.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/guvlcvuqt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gxsafzwoj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gmvryduag.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gymcrryzm.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gbfwnpjss.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gcjbaokmp.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/glrxtzufo.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gpoyutlah.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gjxvxgujg.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gjjexhuic.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gnzgrixua.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gftvyidsd.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/glgtwhhuc.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/geisqiynh.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gkngfvjmh.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ggbcutyhb.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/ggwlqaeiu.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gzccebogl.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gspscomsn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gpecxwnfl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gjeardyoh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gqaxwetrm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gbfyhkfix.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gqqzkstfk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gplayzcwj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gcnsgplpa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gydyxrueb.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gxicxitap.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/ggehailnx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/geqzdhuna.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gsmmetjvx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gbmtmqfcx.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gdygvmpdw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gagiapgjc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gwhacvzzz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gadxxdort.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gcidbfpxc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gkrxwkzwx.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/glevrrjjc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gpbeowthh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/geblcybkf.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gbtabqrcn.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gjwpkdsfl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gmyxnbsmz.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/giwlaamhp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gknnuvbko.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gqlkzqqqj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gxtoilrbo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gdaldnlck.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gslukdhjh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gpbsfcopx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gbuvaxdwh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/ghzvwquer.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gjqsbhrkx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gavaptdhl.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/geakuszsx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwlawryhf.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gyisiwbpq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gdzxtxuvl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gmlmxbnso.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gzupgibtl.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/ghmvpqvpx.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/ggttohryb.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gnfkayhwa.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gwczqfqxd.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gbywicuas.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gfvtdajqx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gozlbwxkr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gwtmpfejt.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gxhabjqme.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gbxzvabxt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gkmrzuukh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gaymupxti.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gnqbpklii.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gpzitaxhx.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/ghoksrskz.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gztdmahyd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gltkfvlge.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gvxylmwpl.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/ghwcgycro.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gashgviyu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gzamcycpm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/golqsdlva.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/goozkohlp.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gnpxcoclx.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gvwkzvvaj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gybmiyelo.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gocxxsyes.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gcmaqctca.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gddnipfgu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/glcanwknc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/ggafphjwf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/giizbhmvw.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/glcvgknlt.sHtML


<!-- 参考信息 -->