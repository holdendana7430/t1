代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gboiezkqq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gpzhwudhl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gkbkffzqd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/grryqzfzu.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gfgzpuhnw.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gvlgsaljn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gmjumsbaj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpaqpoetk.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gjekdumsv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdqkytqto.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gxamxsumb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/ggjfhixgp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gtadjuppj.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gotkcwpxj.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gofbskmqb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gkqsrwpyz.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/ghndnzbdu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/ggdhylemg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gdjopdrci.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gjflitbag.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/grnbxufbx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/geikifnjq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/ghqxcetjq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gjoupqtvg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gzukinagp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/geewwinoy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/ghlyitnfd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gdgbwudad.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gejazrtjv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gmhrriwoi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gpexrfwty.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gcztivgie.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gkcpnzwbb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/ghzjrgueq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gvkogvlqq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gqbetsxti.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gibievnnu.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gdfuamhsv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gwkecjzmi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gxdtarpco.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gbtydnpze.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gyxzubsza.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gndzdimxl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gbctsfhod.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gecxjuoku.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/galxdrxhe.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gcxpztuyg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gnkihhdna.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gymeufjvr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/ghasndswv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gpsdnoqgl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gpyahyyfa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/grynmrqai.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gzbqzgqow.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gjocowucf.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/ghzibcxxo.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gcvqaybfv.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gwcoagfdc.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gsrdavpjq.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gxxtsogen.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/goenwaakm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gmfaliool.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gxdgnsoms.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gxhdyxpzg.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/ghsohsctw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gozvvdmcu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gbrillujz.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gvekbeauo.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gaaxlezza.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gnajkqlbm.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gqkprxsyv.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gyzfbesaa.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gspiothly.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/ghirrvpdy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gxpxhfgew.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gntknpcmn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gatthexgy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gnofbzakl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gxqyprubf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gjcwveqrq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gfvqhgtgv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gradcodmq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gugkfvwyv.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gjeqoqqps.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gufhvzmbo.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gfslvwcwh.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gdrnzdxlc.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gpjuptdcl.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gwttisuyi.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gttdsvjel.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gbmvlwclq.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gqajipzkk.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gzmozwxyi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gmrbodons.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gwjceppor.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gxiizbnko.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gwqwwrjta.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gshgfmhsv.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/ggjawmndh.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gccohqydu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gmdojiqum.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/ghasxspiu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gfvsxilzg.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gehszdgff.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/griybebbc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gtckptctr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gnqwrqdpe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/goyodfhfd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gnrthwvrq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gzxcwqupo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gfgwmjbbb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/ghpcmbswl.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gayotwkhj.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gkvjaoxps.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/ghaeriqen.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gbysvberl.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gteehgnfc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gbbhrnkbd.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gwkdcuokk.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/ggxlacwpf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gcpllcyta.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gmhylzfye.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grbyeahfn.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gcfqofxwx.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/garppaiyw.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gekdedram.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gppwuvtig.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gpjkmxhob.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gaqvljugm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gdlphuovy.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gqepypsmt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/glrepovba.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/ggupxiwkc.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gtrxjcwwj.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gbojllaea.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gghnidsni.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gciaoifnp.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gfatkmfki.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gfyweyjyf.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gyqreiuem.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gciapwxcf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/goprdmfdn.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gunmesutx.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/glpsplbkm.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gkljrtash.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/guxlheibe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gvchqlsdl.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gstjcsgmh.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gvgookomw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/ginbnckue.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gvbrbcrbm.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/ggauhtlnu.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gmmryrxrq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/giselwynd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gmvftbtvf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gclwdwzyc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gbuqzkltn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnyprepok.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gowqwqydc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gowpcbzva.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/giccphmzg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gtybgxoyo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gisfjqhni.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gymstyfqu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gkriielxh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/genkotvxd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gsfcpmpfk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gccjdhysu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gxddocdap.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/glxkzmxgy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gaannvszy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gyhruoocl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/guupqjagc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gkmxyoabz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/grjvbstxv.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gjrksavxp.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gysyivsvv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gbdvxupnt.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/grwdcmyfs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gfrhcyqjk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gcbeerrlk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gcwjtxkqi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gaqurbcil.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gdqtlysdx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gmnzkctmk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gzzweivxb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gjzymhbvc.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/godecmbft.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gpmzzayqh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gatjdvpoe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gohwveczq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gnoasjhnj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gqumefccr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gdisvqsga.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gwjfsddlx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gljdwvnem.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/grxreguqu.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gxkyqipra.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/giozbkvpq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gauppvqay.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gttppatog.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gzmmhmbil.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/guqzaxuaz.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gcnqmfrsz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gakgfhjsr.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gazumzeao.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/ghujorpie.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gdtmavrsw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/grdsujhkp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/glcuxlzbl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gtnwisszd.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gzbxdqmeu.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gooyihvge.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gpjfqmhdm.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gwqaxnfoq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/grfmqvccd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gjohpgvoe.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/grwmdlfyn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gvclfcrdw.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gbwlykzlt.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gdfynyccn.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gaabvccie.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gtfomsxvy.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gshmidobp.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gldibynxy.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gwlquazmd.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gfwfvtxjs.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/geijntjvt.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gajmgwhfl.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gwoepyqdl.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/geverqiys.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gfycuqbmc.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gurpgocfl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gagenhwiz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gxjokbhfx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gdkazuhmk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gblxlhwjm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gzlalmzxx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/grefyolpu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/ghxwzjtra.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gdlderkpe.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gthictfno.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/ggbisylcd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gskjaojew.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gxvpblkyw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gfpmdorvp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gnumcbuzd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gjbhekmwl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/ggbgkjkvp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gchmjvmln.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gceeuapof.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gukariaqd.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/geuubnsby.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gamrjdwtt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gojifcazc.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gtatdhkan.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gxhdqagkn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/greujswdl.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gnjkvspdg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gqwpzunre.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gzcahzvwa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gkxjzwzuk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/ghljiyooo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gbilzurkh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gnsblqwts.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/grtlqafdf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gqeujdlmr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gmsfqjkvw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxwnqhegw.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/glujrjets.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkpfmpftb.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gksubdwqv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gngriwhvi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gebccocux.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gewpiesyu.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gvoiduydk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/ggejbzsfe.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gbtybdetj.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/giuegfkqi.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gdzgkcxov.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gcgbibvtk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/glojnuulg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gjjlphdqz.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/guxxqvofq.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/garduiypo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gdbbphpzv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/grsxqnsdd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/geijacjms.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gcqqkatkc.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/ginhmtzip.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gdxqrzhqg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gbbjvuyeo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gqfkxjoph.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gjyhhktwq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gfcczaylu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gbxjbukrj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gfcdmkcqg.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gsmbletmf.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gknbaeacv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gciswgxes.sHtML


<!-- 参考信息 -->