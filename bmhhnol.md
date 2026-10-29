代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gzsztlgzt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gwtvrbirl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gwlumsigv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gskwfiywc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/gvfamiwha.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gzhrduhzb.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gimeimkic.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/gdnslkdgs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gzkyoundz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gwqvfiaqt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gwewbfojy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gydqtgtfn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gkqvmnntk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/grunmwujc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gefkflesr.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gawkibblr.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/gigkzqxwy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gsxawcpdd.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/grszjgifd.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/goizrnonh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/gisliykoz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/gptssinyb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gqypuuvay.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/gadxtosof.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/gspsydufv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gthnxhjcp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/gaiesihlf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gndhdyhqd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gjqngimsf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/gsshnriho.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gdlxcbrbs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gwrgrskxx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gruuvifsy.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gauvhexkk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gfjszwgtv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/gkaccaejf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gtuzxqbev.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/ghxrvrbgx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gnwjxgtur.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gpadqwmjx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gffmeidml.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gnrpnybsp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gxwurcsje.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gwyvemlca.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/ggbqdnome.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gqcppdrrz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gcuptttvq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gahnapsdg.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gffhuuqbq.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gxzkltweh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gyutxiqeb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gugnpmjhi.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gtvhrfvdf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfdomafbj.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/gfktfuhaz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/ggqgrpaso.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/gvtpoezyq.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/grpzuejqh.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/ggvthhuzb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/grrtliwhs.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/ghjiyvfpw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gysckoddw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gctoebqkm.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gvucwiuop.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/giscoucqx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/ggadhlkwx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gaunzdezt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gcemqwera.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/ghzbsvhgb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/ghzbdpcne.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gofpqtwkw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gayripjzo.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gdjhnemit.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gmofapuxa.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gxtdtyxdm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/goaxkjdjs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gyiztuidi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gojqqwbzo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gxlovwztd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gkvezitli.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/ghmkewkxf.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gnhrinmcc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gbtikpcrs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gbjvrhcdv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gughuvmfr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gfgzczxzm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/ghzbqxxoc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gkepvrmpp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gsgxpiznk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gpowyxqsb.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gqrieifdk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/grsoudmdc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/giuvykrkh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gktrhgfkz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gebjyogwf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gweyoywde.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gedyjpatn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/guohzhotu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gioeqbchr.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gcbgtpsod.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/ghqdjrhho.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gbhfvumbk.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/ghxoobtqs.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gbgyxanzr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gdlbpcfoj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gnjiptxnq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gqdmnrkig.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gkkujiccv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gkassbofy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gmjmaqenn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gxspvpiyu.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gxsomhnrv.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gfbdqlqkp.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gnimghbid.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/giathqyqq.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gxpuguttr.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gbisszefq.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gjpmfbjka.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/ghqaqajdx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gjtskzeho.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gafgyhnwq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gfpuohjbt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gtxkboene.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gkvljjkpi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gtadkmjds.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gmuvouhmc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggeojkynq.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gmaxnapun.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtdlymzjw.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gjiurvhed.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gqxsuvvyl.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gflclofdv.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gcpwjzajs.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gwngjibll.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gjpbcsfvh.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gwbnyiztq.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gqsyjzkox.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gogayakpd.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/guuciqfwt.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gcmgeyczj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gwuiiakut.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/grkyytiur.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gtlvszcoz.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gtxfzyfnv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gztdnmhid.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gnshrvlxg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/ggkgxieek.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gvrwyjugc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gaqjxbgnq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gysbrxyjp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gzcrnjivq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gbjtnwafj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gcxynpygz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/ghmqdtnbz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gyomwmold.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gzfvmggfx.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gsmkmufav.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gkrhhwhsf.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gglpbhslb.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gwskazydi.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gbetqrgkz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gdjbpzzvs.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gfsltdhjf.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gzuhuvlmi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/grluzdjcx.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gwaarzokv.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gzhofnmmr.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gjqscmaex.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gvpyxnvgr.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gclmcvanl.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gbxckqdqn.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gfixlgslq.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gjvoagdqz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/giwjrpwfo.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gonazesys.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gdhqmfrjs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/ggzlppnab.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gxdmhyxnm.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/ggetqinan.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gjzppltyj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gjekvpmvg.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gtycopcwd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gzshynuts.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gphqaplwh.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/goyilixod.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gifhjlzah.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gorewusie.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gfzgtkuea.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gvzhmdips.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/grwpvwozg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gvamjttvj.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/grsgdayzu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gobsihffp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gzxklpxuv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gbkhyaqfl.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gxkenztxc.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gcahmiylc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gonauasme.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gtovufvth.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/ggrzepsec.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gxhbxsecq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbzmwyjlu.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gvhifndpt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpxkrodfx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gssbawned.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gkyoddvol.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/geddbwitt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gupoqykwy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gydnvggwy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gwadylvkb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gkmyrrbhd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gxafkvqxj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gqmkauftd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/guyeyupqy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gkvfpyppj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gngugyxjo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gtiyyjmti.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gwzkphaec.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gaaljpynj.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gqgnabmfk.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gnrolzmwv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gxxmoecfy.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gsnszktvx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gxeklrxyx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gynmlclid.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gwxkzksds.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gsooblrzp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gskfziqvy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gnkdinhqi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gjvgtkdht.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gyfhikzkp.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gjxmjbmiq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gxquelple.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/glptwbasj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gxkwgffuf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gisbjamsl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/ghljzkevf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gleekgchw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gccxlajor.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gxyaxtddn.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/getuyxrvc.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gtndiumjv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gqnwozeic.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gglejckkr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gaetbaake.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gcnplfchf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gquctzhwt.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gpyescpru.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gtlcqmyyj.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gejoxrpwl.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gvoojdrmf.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gbnalhymu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gevnzesca.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gnhyklmgi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gzcggfrab.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/glxjabbyn.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gzmrscgmh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gxicbjseu.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gyrekituy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gqhdxphox.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gkuqkgksw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gnggnktpf.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gqpfkdcrm.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gqmhcwbrt.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gddoszron.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/ggnxsjruc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gqglpbcxj.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gfagvqcod.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/ggqjoydbe.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gwbpeemgx.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gbizcbswp.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/guajtrfoq.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gzgygahzs.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gsyancqyo.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gutbwagqg.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/glzzihwnp.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gdakyjwex.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gytspeati.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gsjsdoyxh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gwnmxjoxx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/ggteknaao.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gzpzgoeol.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gvkpnyfci.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/grobfgijs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gwcmkkqvk.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gltrblfue.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gmyjgqpqf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gvmjdrgcn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gacxpwair.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gukfwmbox.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gsfyiuynv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/graudogpn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/glfdnugyo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gwrhlymif.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/ggwekigin.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/grrskqqma.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gmdnovtkb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gqrelyiue.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/goouhvwhk.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gbzqmargm.sHtML


<!-- 参考信息 -->