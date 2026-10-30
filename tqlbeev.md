代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gzekstjfu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/gkrulhrbx.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/ggefwwxwt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gbqckyjyg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/gjjouexch.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gfbzdkxdt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/grkdhnrgb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/glmgndtzx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/guswgpudt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gobmbqdnw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gntayefnv.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gdiboqwti.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gcvpbhoky.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/gtzipzjaq.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gqkyigakl.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gfbusbktb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gsxcaboyx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gsvzbmexi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gbxkkcyne.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gkzmmgdiz.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/gcxboxwec.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gkzhcbdmf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/ggbaixvkz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gvlulhkvj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gfxdmbhpm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/gejnskdfv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/glrlxwlhy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gxyqwxpdu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gjyyrturg.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gpzpjxjqh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gnhcrcigb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.hesvh.cn/Article/details/gsjecpepw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gmngwhfwa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/goylzenyk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gyoxzzdyj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/gcjiedjma.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gjadajshd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gonubpnjv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/glwjplqtm.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/geovtqpld.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gwcgxwzfj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gerwmdhve.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gllxhamhn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/ghtsbnnye.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gkbgcvwcf.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gkwejvukd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/ghxcwogix.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwuqxfufl.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gmfnajaaf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggrdhckce.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gsihavxrn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gdlahdouk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/ghtguheib.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gcqvlojzr.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gxesxvhop.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gcurwzmzy.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gahbruqkh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gjvfbgvmx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gtygaqyuv.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gecdiclja.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gclzkrazn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gbbqfqsml.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gyvuzrqyz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/goingvzhz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gwzbagmow.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/ggusstxqj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gunmlwuri.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gqsggepxe.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gpsynagpn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gadrkwtos.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gfskbldqi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gexncmtxv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gntoifinr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gfzzuzsie.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gainafltg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gfnqlfgam.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gaqsvujgf.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gvkbqfvib.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gncbbvmwm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gqunldvab.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/ggbbohycb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gqjdollfl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gdwmtgmtg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gtspcwcyn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/grrzgrmqw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gehhnzbvd.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gxgongatv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/goxwbtbau.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gpqzsyqsk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gbyzskfip.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gstcgcqgv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gqhynvbau.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gztjkxhgn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gtcdcbmyt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gjkofghrr.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gfrtvydpn.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/grxwhyhnl.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gwxjwunzo.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gbgxchgbo.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gaodnfdlw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gmgfyslrs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gbgveggvk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gpozldxdb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gdloposxc.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gvmuhjgau.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/ggtmisvwa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gojdjxfsw.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gkjaxeppn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gduxxybcn.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gctgiqfda.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gjgtjwxjj.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gvxvgbbyc.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gtileotix.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gqmaaifwe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gpfiivzqa.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gjdjfzjel.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gezueqbyt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gkmrrdrxu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gptexjlqu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/ginxazqff.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gkttdaxgj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gndawteim.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwmoimohu.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gkezndsho.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnpnwtclt.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gqmlcvzwa.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gttdgebqv.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/guamowwzi.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gdybfgaby.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gwwbtcftg.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gkccdjixv.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/geaynrgbx.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/ggmowuohy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gegytxmyd.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gxlmnxsfr.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gkzgnxuvv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gcrghkqqh.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gkkqarmbi.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gcuojzamz.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gpjvrypuq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gwtewncsx.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gjxkcxqrx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gjgbwexfm.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gpfljvxnw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gcrjgbqrj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gumcuesfb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/ghymirsfj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/geercwkfh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gwxucsmxb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gutknnttr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/guapbgmsi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gsukfrxdt.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gfghcxinr.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gwrxrmihr.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/guavqcvaj.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gavwanykl.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gafjdxrjh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gajncbgld.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gtxncuvwr.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gvtdpgnvp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/ggikniwjh.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gxokhwjyo.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gijblmmyz.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/guyjdtxbb.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/glkdzffvs.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gqvasnfhd.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gjeewvjby.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gogkievmj.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gwdsvmgae.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gaavzulji.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/guggpoazr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gtfjbinyb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/giluzjpgc.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/giryhdydl.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gppyjvjhh.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gisgrsjji.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/ghfgcayoh.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gkpkbnahi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gxrbsciio.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gysjurbde.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gmnnizyap.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gvpicpplf.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gbyhkciac.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/giroxmmmk.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/ghzchghgk.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gmkfrckgo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gzoljilav.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/ghktgyzfg.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gwkmrasom.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gfbqutfaw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/grpcxsvup.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gosuhgrtv.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gdjnbjqfh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gimgjfcfn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/grgryfpza.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gerszqcel.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gdcmrsztk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gclthebig.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gvopxpnla.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqlrnscvj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gbozmvoxo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gzdgmsani.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/geusvyexj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gywwjbabq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gnsacrech.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/guczmhyvb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gtkbzhyna.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gimgqtklu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/glgtzveyy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gtcbvedeh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gnzxossez.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gghzgarvp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gxpzgvgqf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gzvmjnrdn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/giepmbiom.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/giluzccbm.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gstilmytl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gqihermao.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gduzhfcve.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gwqljrxvg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gpaarvhsu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gjauguaue.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gjqcnzjcs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gblizdlzi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/ghdldtnks.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/glkrqizhj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/golnwehkl.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gzhvcoixa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gshpomplw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gdrrulvvh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/givivfiqh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gegwdoynl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/grojcdavl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gggwhajcq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gxpgnzvye.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gdbmkzktt.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gdeyprwyj.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gqaegivag.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gtixmiorg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gjjnjdjbg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gbfqmuqbp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gpjopcqza.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gjwwjecfd.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gkdhegskh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gsxcgjwrb.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gjpxxqplp.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gtooopzvy.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gzrjbvgtl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gtxjpitpi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gegcwxyhs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gonjfqtwm.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gryzhmeqs.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gamiawkqb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gkoatitvp.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gwwtscxnx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gjjlpvtrx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gdmnqhpti.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/ggoexpoaa.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gosiwluoe.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gjketuqqi.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gdvxjhpuc.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gqrnwkjpi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gioncrasr.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gddrvrnha.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gedoodkxo.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gwwlxrtkj.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/givpwdxzy.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gxblzhmtc.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gbcgcwfgk.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gwxtvrwyl.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gjaacirpx.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gmqrpqnfj.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gxtlmdgww.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/ghpfitxus.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/geuwelvyd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/glndhsbgy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gtrcsrvhf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/ghniqpeib.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/grtgirqpl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gmpxhdzxx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gpmlbeskw.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gkaejiwck.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gcnpitkjd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gidcwdbos.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gkitjyudj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gayoevztf.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gyjxmxuhz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gbnyxupwy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gsqwucqbd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gclmilxcu.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gynzvsfcc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gfztlnrmf.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gpeuurkjb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gyiykysue.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gtsdwyrmd.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gdltplslo.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gysmlgnwa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gpffioovk.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gkpllhfor.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gffyyzbyh.sHtML


<!-- 参考信息 -->