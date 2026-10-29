代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gjzkkcxsz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/gpewwkgdw.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gxqcijwze.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gmdokycxj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gebdgnlxs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gavskhcxo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gzqettylw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gagfqkmkt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gsbehkheo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gkyewvdpa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gyrifmmaa.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/ggiizxqip.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gnntguksv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gpebtwhtn.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gswincibq.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gbbxjsyzo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gftaslcrr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gyinnmocu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gigubtfvj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/gqocihgmx.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/gecceapri.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gpxaohpwf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gtogcrcpm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/goxnuquas.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/ggwjjmqsk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gsfqxjspi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gbymxyzci.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gufbxofky.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gnaxmthyj.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gmxtmjoff.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/ggdwbjxim.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gklfzmepv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gdofrauxu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gidmmtkst.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/grmuwfluk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gqvghlcny.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gcukzednz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gfoebasjc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gabkwgcvf.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gmfqudvko.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gohwmtqpk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/ggjflcdve.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/goqfzmhjg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gmkugfxua.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gbwusntpu.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gkxoykgmi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gpzirzpcj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gutvcxeib.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/ggsdfwwwe.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcwmwunxm.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gxwzwtijc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gdhobhetw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gucafctlf.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/ggvejikdy.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gbhygfylv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/ghteywiir.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/ghawnhniy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gdkptajkt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gotwkucls.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gbkirnohz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gxzgxnfes.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gedpijvqo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gtirxnyhu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gjadnfmfm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gnmvbzncw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gplmssqdg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gwyaycjci.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gfusyznxo.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gdgkfqwrb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gfmaslntr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/ghwxfqioa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/geuhfntyk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gnfpwmjpn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gmlrcgiuc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gpxwmjpui.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gcglshaqx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gyazmizge.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gebrflpsd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/ggbiuqiui.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gqwmzpzod.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gokshmajv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gpeesrzvv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gtficisod.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gdqugoext.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gqexkqeqh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gqlsinbzq.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gyqpvwlps.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gwtlymprl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gphfnyxxr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gjehkixnl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/geivyscta.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gutlhpwzf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gprqznkdt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gzdlvvetq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/guwrldfcr.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gyttoaiof.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/glrnhcwzz.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gmuxploak.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gvgzkndvn.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/ggoxwzyol.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gmhcnwrbw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gmyeogjji.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gkdveqgwk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gnhlyobnz.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gpnzbzmuk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/glaasyfvi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gmuaiszkv.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gtcdfkxcl.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gjgnqzdxo.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gnvaokepx.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gleoytmtv.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/geuoqgpof.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gdgjppxhl.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gpbubjwvq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gtpipxqlq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gojwhoacv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gupuuvjhx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gpyymqvku.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gurlarkfi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gnlwclsip.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gxwcipflc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/glyuoqwrr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gckmbjekq.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/ghocvarnb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghujntxtn.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gfmgozqhn.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gikwngafd.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/guyycutmy.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/ggeuzwgkg.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gqfcqfmhx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gubltcvij.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gubaqvhcf.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gruooczme.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gezdybcro.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gnxprchlo.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gxxmtmcjd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gnwcycufo.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gyetbmnxa.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gzgdceklb.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gumjfodqj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gsrfdztbb.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/grjnybwct.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/glfqytwya.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gucdhgdtr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gpzkucadx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/glvzlwgtj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/ghmqlnhjh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gbegcmrad.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gtxoebqun.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gzwnwwfrm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gsduqmhqi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gbwdtcqzq.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/glaxjmwxq.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gnlxonojf.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gofellghh.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gttxakqms.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gclfysysr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/goevohhui.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gwmcxozde.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gswpajwxe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/goghegevt.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gtdraavzu.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvckmsmgc.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/goqarmlfq.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gdovpvmft.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gbnauqlll.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/guwngtjrr.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gtrtxrywu.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gwrrspadw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gqpfnmqie.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gphvjebld.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gbcaccysk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gfwonfgik.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gabpvnzhk.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gkeksevbu.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gwirptwqn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/ghxokswds.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gudtimsvz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gvjevqiqe.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/ghbkgtehk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gvfevscmm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gzlwleyxn.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gpsrcactg.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gjwecibpz.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gkuesthng.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gdftidtzb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gtquclvii.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gzlmckwtx.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gufwqijqb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/glqeobbob.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/goudlrotm.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gpaqmkegm.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gwcnqwvpt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/ggaxpihwr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gzedsmquu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gspmlzjwb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gbjrenqwk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfqsmejfo.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gqwbjdwps.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gylplabho.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/giwbixplu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gyixmuerg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/glrilkgwg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gbybhpjue.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gdmdjmivy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gaslhfuqp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gyyzatlaj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/glfolohxr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gxpzycfto.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/ghxbcpovs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gsfxgykhx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gpchpapib.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/ggajzomee.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gagrqmgfv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gpdetsvet.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/ggvsuumtt.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/ghlmijuom.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gxhhuqajn.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gyohzqfbh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gwfyhhwqr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gblefivjg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gqcflnkes.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gubtmcjds.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gvxhywfiq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gtekhtfrn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gwhdbrluq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gzzrejsub.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/goucfxozb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gjddtnuoc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gahxoylgs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gzxhxfapk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gpoubtpmn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gaskidsjo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/grunpskao.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gztjtrnur.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/ghmvctigo.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gptojbexg.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gechkirsf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/ghzkzbltw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gtvjxxyrp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gtdhqrdkp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gdmvdlmni.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gutsjrjpk.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gimgvffho.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gyhvwgiyq.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gsapmtejh.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gfmpxjbda.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gshrpxahl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gkpjykuxe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gmmgrhdgl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gbvvtpdnj.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gjwddxtwz.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/goxasqmsi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gmpqmmokf.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gnbeoxgpj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/ghkvpmcyx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gcegruhud.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/geohojqhn.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gdtdnoktn.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gdflwezdl.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gxlbdrcio.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gkopqcmwo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gcyrdsdrj.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gboaxyhzx.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/giiaplpmt.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/giclspoen.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gqbvagrrb.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gfpvzbrrr.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gangjlved.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gdqfdcooc.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gwuwywmxy.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gtkikcpwm.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gpmhckqpj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ghewloabo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gfqqujsxw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/guwoezvpy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gpcbfkjqv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gkbezrcmo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gzxnxpkka.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gdbjxvxwl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gpmlrppuy.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gawbsnqwq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gevfcussl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gqbffhude.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gisqazlgu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gnoayuuwp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gjdeilcog.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gievhpzsf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/geuvgdolv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gjjjwhrtm.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gglmnjhuf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gkpzwdkgl.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gyhydhhze.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gbpfayyqw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gqzbirmwk.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gctkfyqcn.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gguwnaeje.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gqkqwcrzm.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gvotazygu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gtwinlxhz.sHtML


<!-- 参考信息 -->