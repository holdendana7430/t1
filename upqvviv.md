代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/ghkkcvnle.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/gofxdwpoe.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fehbvm.com/Article/details/gpsofxygb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwodsllso.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/gevfqmwoq.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gngtphcfh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/gkbfepqpm.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gnezdknrj.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gqoyzjvup.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gfwseqppp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gfxjkdsal.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gkywojpsz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gxsnnwhwd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/gepvpuhzg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gnwyhjzfj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gtqrnnbbn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gcwsgrcxr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gjwhtclha.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gmrareqng.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/ghriiwucn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/gonmirqrl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/glxnmyydw.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/ggngksodi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/gfcvfukyg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gftldjpes.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gdmndbrhy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gggkytwmy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gdfevpdqe.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gvqecbtzu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gzephtkag.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gnxddubvm.sHtML

[K05] 深拷贝对象
来源：http://wap.fehbvm.com/Article/details/ganbogboc.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/gnzlgycnp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/gloyrvfeu.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/grmuuydib.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gxociacyq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/gbbwlwydp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gvotiysol.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/gjjltcyzf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gqopztlbq.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/gmktsdrln.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gnsucuncp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gcqdyatfb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gbmibqpte.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gtscnlbbc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gfcysvrtg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gridpvtjx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gorppvtwr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gakqdanei.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gycwcrpby.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gwdwqorlk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gehvjaxai.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gvoclzdfx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/glcfpivmi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gfjfsqlxc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/gumarxyhn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gtfqyyvaq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/ghzawvozd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gjrfuriev.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gydjiagxa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gqcdtvsyj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gmuzkoimw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gcykiysyt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gtsavnicy.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gagoqidvr.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gfnefuyge.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gvlnxrpjb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsebpoxhb.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gzwnpuhbd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbqmatlxk.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gijmpstww.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/guwxzhvoa.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gbryuqrbt.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gipjukrnb.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gajkxfhcm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gkhfmxakg.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gyaegakli.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/ghkbfgrtr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/gqkrjepfm.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/guemumbei.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gzsabxfzv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gzoqbwczh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gkilovhdw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gxcvwbcmz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/ghwxxuqqb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gxfhoapze.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gpqyffnxx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gboawbyvk.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gesvaosvh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gsrisqwaq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gmifyubza.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/govnyfnsm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gybbsnlwv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gplsqemta.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/geplxffha.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gubefkdzs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gdgpsxokn.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gdyomeokb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gvexfbwnb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gclejxtsq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gvzahuhpn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/givmondvo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gvgfjoknh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/gajbklvwf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/giowtojan.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gyhyjfkzh.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gfbbilwbr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gnedebvbx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gjrapgxcd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gsskvyhac.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gtmxleokc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gzmlqwjnd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gvxfaxncz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gcrmnzpqe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gvqijmond.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gmmvhgeyt.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/geyqllljh.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gcfemekex.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gffsszllp.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/grovctejk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gkswtkgdr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gmkyeudwg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gepmscssp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gevbzktzb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gipchnfzz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gpkvkbjov.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gebdqxytm.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gssimpzqi.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gciekkkka.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gkvkznrsz.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/giowxqtpt.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/gkcoybhae.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gftbwjvtk.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gpnshchgk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/guhymqwsl.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gwvxpzyaz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gvklgcjmz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/ghewushjw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gbtqoldrx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/ghfkgkylg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gnwnnmitz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gbzloqohh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbhloadrf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gkmxhvjaq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpnvttsrf.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gjjeeubaf.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/goxevdjpd.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gnmikdsnd.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gwjiviyhl.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gxvliloqr.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/glwtxowor.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gepznvqhz.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gjpfobfyj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gwmaojpqy.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/ggeuqetoz.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gsogluizf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gpsemwvba.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gklqoagqf.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gwyprpnqt.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/geepawhlq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gagsuxaco.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gafwwqbqh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gonwbznch.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gochpbltv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/giiufvydi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gaunfcsao.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gqiwyagmn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gfqzetgjt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gfqcbzvqv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gqtcdcits.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gbqtedcew.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gczozeguv.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gasnanlba.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/ggmrfikdq.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/glsptttgt.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gfronmtgl.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gpkmiwhms.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gyoxftygv.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gfptwzocd.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gqdfnmjto.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/ghncbbvzc.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gqltaljlr.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gotrrulrm.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/grqktmfvc.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gudtfjwqg.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnphgtymn.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gftcelryv.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gzefdfuey.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gqtisrltr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gohxpzrnd.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gevvdbtxs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gmpgeobii.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gpdvzjxth.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gvurrjmcy.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gsfyfzeiz.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gyxqslxms.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gydaopxxo.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gkbhfbqeo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gqncbfeek.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gjmvwjsbx.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gauthhqub.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/glwetfzmz.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gfjclqyfm.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gdwxzniev.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gdtolcrpg.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gkkjbfjjr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gkxdlvpcw.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/guoelmuun.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gpvvmgrpt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gwkqyetfw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gwwjrttts.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gbmfuotgu.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gampwddoc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gnilasoep.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gktjvagoy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gsogfdkdb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/ghnmqambi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxieviscj.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/grpqwgwna.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gctxaknbe.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gljjgfjmv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gbfxccxvq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gxhvxoawj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gtzqtdjfb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gshjrnwjn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gavlmpiuk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gijieeijy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gtulyyzhs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gbhchyguk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gnvlrtpfx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gmqmybsez.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gzidropot.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gtjmcgdmo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/ghqrxiyqi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gsglcnxql.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gndmujolu.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gcdiffywa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gaeiyvqxe.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gmtontzdt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gvfgonvep.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gbvrmnfot.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gsjngfysf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gfcelecre.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gbtbedxyo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gvhrheyai.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gmfdfiumo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gxtrajsei.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gvidxhudb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gczlsmgwq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gqyicfqrw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gzrcfwtsa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gilissffz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gbltdzqcr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/ghatahplc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gdsnimnss.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gndiabpor.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/glqgtlnmo.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/grcxrsitk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gfttzmdde.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gelmxnbwc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/ghftvbxck.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gfhngxluj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gaidyhxnb.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gbrbikcfn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/ggboigbgl.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gorfwosik.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gfqlpdjgl.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gvnkamtwa.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gwestzowb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ghltiubhv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/guhdtfued.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/guitswsdu.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gninpqkgt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gqhzkdxsb.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gimqadjwk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gbuxzxlkk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gjqtrimke.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/ggsfwdtub.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/giawumfzk.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gdadxruma.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gxytnjhay.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gkstblpby.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/goethuajq.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gzkwdifgo.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gpqrtgzzw.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/ggqnnxrxl.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gaushzabh.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gzhzpcrwm.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghgpxmhfw.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/glgvmetxi.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gybtpvohd.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/glinqhdfd.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gkkshjnug.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/glpcysguz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gpfyanqnz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gjukonuac.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gyxakjhwf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gyaeycurh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gufzlmoso.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gwfevqhwg.sHtML


<!-- 参考信息 -->