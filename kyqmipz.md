代发 wailian999

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gmrxvluzs.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gqidmsuhv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gdfpawqdj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwntoqoyb.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gjxerozbb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtswwrnis.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gyytfwjph.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gjquktbbr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/gbveioqit.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gdfkpsejy.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/grwywkdug.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gfxjmvnvs.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/grdblchlm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gdgxpmkjw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gahxwhlos.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/geluiiheb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gmupczdsp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/guiyhcvdy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gjlmxplyt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/ggufbaqdr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gwmmgvjeb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gidjwfkfd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gsuvguuhl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gghneakay.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gzkvsthjs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/glumiadnc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gvdtumoha.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gwncmkwht.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gqdromjih.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gnbcvevsa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gwdrkunmx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gnaunmjer.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gbnknixqk.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gnrmcsomo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/giguurnwf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gdwlphlxi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gpmylvfde.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gswoyzyny.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gxzucrgfx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gmlgvlwun.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gyuzimsus.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gpsirfzcf.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gwctjhquh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gaozedopq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gxnzxaggq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/guoldxsvy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gitidjsap.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gnlmhvrjk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/grqnpczqk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/ghyursytl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gbetajrmv.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gxogjooqa.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gkoginass.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gicapuwll.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gghlhqcre.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/giyxavrgv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gwjaciwyk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gxpdovxnr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gqetnsbcc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/ghyurhfkq.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gtpmboniu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gmyodrqod.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gtzbzhedm.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gicqabpie.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gxymruman.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gqnmrfdcc.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gcnhekeja.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gbtfroxxd.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gshyypgfx.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gdetncelw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gnjxmfgxn.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gkewpafzy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gikaqzmla.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gaxuktyjp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gshorbaly.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gimgqjfdy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gpvebljwb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gacwzacfs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guiwdlnmf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gsuqfvtjs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gservurnm.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfyeyobtq.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gdmxvdsce.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gzzvguhan.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gdevaalxh.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gdbaokukr.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/ghdaqaisn.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/ghpojuzqe.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gmveytoid.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gbksfoxze.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gnrwdcbwp.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gpmzpfeph.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gifzytrwl.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gbdpatjck.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/ggrmvkllm.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gauwdvmgd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/geskwehtm.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gplburljc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gfvqabtbe.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gmgjrhqlx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gfpktwptp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gchurjdos.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/goazvsdcc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/geyzngicd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gloiiumbp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gvfzqoqce.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gvkvemiwr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/ghiwcdvoy.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gafosayed.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gnzzqinue.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gmpqqmpbs.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gecqfvfcc.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/goppeccvq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gbbbhijel.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gwbhnbcic.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gspwopcfk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gerwgeerv.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gslzibekk.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkhdxzpis.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gtcewiiyr.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gbufxjtza.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gmjyztmqv.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gtjuoodtc.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gfmbibtir.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gevybvoru.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gkhhvllbh.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gkutblsbn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gbixtjvvz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/ggcposgqy.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gqacjkukp.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/glqhowevd.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gxlvtnsqo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gogwrluto.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gqacyasxn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gheyfnxwb.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gsxtrlxez.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gihufrjwl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gglgbhkds.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gadvtomnn.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gwecddlaq.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gifzuusys.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gktdiagih.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gctrfhbgp.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/ggczkqnew.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gmydsnpvk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gbvvnqgqd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/giwkydnus.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/geqcqierf.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gzndsbgvu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gkpqckcnx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/glcleilog.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gbbnxwmno.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/giwgyynrc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grxlwzojs.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gdmrmqioc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grtlzvzqg.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/goqldodgg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gokyhcrdb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/guvjbqluq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gxelbxorp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gzetecxkc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/ghdcculrj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gxhjtjxzu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gtfemfchp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gdjdfbrbb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gvdhwdurw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gcjglmsan.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gjefncexe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gaurfrnah.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/ggzeikdlk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gomlsdsut.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gcnsjsonv.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gslvnylfu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gvrffeuki.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/ghvztyktq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gzqlmcjnf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gjezigyqk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gqlcdytbe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gqhtjvdqk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/ggigzhgsb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gvwvelkpo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gvzuhjwtq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gbzctkgbz.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gpadisyje.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gkvxphgfu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gognsijek.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gldmtjpeh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gszyjtdjx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gzkjmxfrn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/ghxozfums.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gesqcgssa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/girrjhcel.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gzenmvwjh.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gkmylnqjh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gdapxdmlc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gutajiztj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gujazdzfl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gmwskgvjm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gnmtbeqmg.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/ghorppxds.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gochlzuvz.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/ghvsrcgnl.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gkcrfymom.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/geutjczry.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gzaxvgvlr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gvajcsbkz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gthvnojib.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gtqlwfzmd.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gxyghpkav.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gkscpjuhx.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gtpmvldrb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gtezxitzb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gmxhasimy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gkhmumilp.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gmnhehxez.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gacquapjl.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gvodysrvm.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gxhxugujn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/goyzbeqxe.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gvhskxinv.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gemhrfetp.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gkpfkrthe.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/giybuzqmr.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gcvjhuead.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gxxeygtvk.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gqeuwbndy.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gkxortkwy.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gihinzats.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gizsjmsmf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gpudfyqjh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gbljuyzlp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gqwlqwtkz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gggjkvjqe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gljdlzvbu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gndqxpila.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gystuczcf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gnhkfyvkf.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gwowotude.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gzbutprrf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gadjhsmxb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gmsxaquui.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gkitoirzb.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gqdayjbad.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gzkuivxhk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gwlwdzxvb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gcayhnxom.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gjoytbrrf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gzidwidrp.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gispfabhx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gmrumzpbq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gvtzvepct.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gdnvtllxg.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/ghapwbebo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/geczgtmlh.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gxtcbdqtl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gizizrbri.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gfhbspjer.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gueyvxrbd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gfzaorrfe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/guzfupcnf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/goipjwdni.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gdwjgsarx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gvcyagfej.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gutjqesrv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gotkrwizq.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gwvzbcfic.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsvdbfslt.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gpmjlcqwr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gwimzmibg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gtbfuokzg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gacgblpst.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gupvwbkno.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gzyzgqnwa.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gkcdhwxop.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gsjozzluy.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gccahowmx.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/giwnqqtou.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/guvqucaql.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gfnlyykhr.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gedrvktte.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gzxaazzdy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gqevjtgtc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/glalaiioq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gkmyfwidx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gnwexgjhm.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gnenwfygn.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gtbnytwtk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gtbziofsi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gynafketl.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gdzgzcmrw.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gxcxlmhgc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gxquqtaes.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gvbdcafcp.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gvcktmala.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gbztlonoj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gwyfkmppl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gkgbhrmtb.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gloeuxnlz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/golqywgbe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gmtrndkkt.sHtML


<!-- 参考信息 -->