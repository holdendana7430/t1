代发 wailian999

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glrtybano.sHtML

K. JSON 与序列化
来源：http://www.blog.zdbjq.cn/Article/details/gquombfrv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gflmlglzv.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/grpgoplnj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gcujcgrwx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gjkaozbra.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/guuiqllfs.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gclamgtpk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/gynybfhgj.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.hesvh.cn/Article/details/gkyyjujfp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gxwlheldp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gficpwser.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/gpuzkrtxv.sHtML

Py:   json.loads(s)
来源：http://blog.zdbjq.cn/Article/details/gjbgrhfky.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.hesvh.cn/Article/details/gzxhjuqxf.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gcgvuimsf.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gwwzncotv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gjbvhlzfp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gpvhcyndh.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbzcxptr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.hesvh.cn/Article/details/gwlxoxvns.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/gqlioiobl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/ghfshgwit.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/giblrucci.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gqitzzgwo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gejlvagox.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/gxfrrwuuy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fehbvm.com/Article/details/gfpiarhpw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gilyxpmtd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/goxbtoqne.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/gssovvons.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/gucyxvxci.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gcmwiirya.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/grxcvtsiu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gwcegsjit.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gbhwzyjhs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gtvyhpune.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/geacuixzo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gzstexgkd.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gzjtlpnrp.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.zdbjq.cn/Article/details/ggdwtsikq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/gncgqobgt.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gonezyyov.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/ggexeimnd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gawekjylo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gtvbhykxy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/ghuhefstg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/gceufijea.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gacqojpmo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gfagrgbiz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gcmrwawtq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gqnwdhtmj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gfbprsmel.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gwsjtumex.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gmjaplckr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gxwpijmzn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gyarubnel.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gcxzxxjew.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gpjrqinyu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/ggiwtdpdn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gvcawfidn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gyaublnak.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gjmpehstr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gareasbpr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gjgebtusk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gfjwmdjnj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gomnoqbmn.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gnekxutpq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gqjkiwxhf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gsxnlbtmy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/goainduhz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gblsfyxrs.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gapnacshz.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/goeiowklf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gfoehallc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gueoqwgmx.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gjmpffsfr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdmtidhxe.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gdwvcfeef.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/ggvgtvnkq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gpmcwabyv.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/ganpicduk.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gxudhdmcb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/gedyihxaq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gcsulkhay.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/gqehleqwy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gkouzsysg.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gdhstnxqj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/galhzkxsr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gpxlefhkl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gfztazcef.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gftenfnis.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gxyeffsew.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gzooxeqrn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gkxzpboyw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gpoujhmmr.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/ggurqqvrv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gnbxjjpij.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/ggxoamngv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/glhzokbma.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/ggmiueyth.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gjdgywkod.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gwtqwmzfe.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gekqnhcoo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gahoahiux.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gloxknbxe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gguelceyl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gjsadirsi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/guqfyfspx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gqbbuohdh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gjjsfoljt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gabstcanu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/grcaisjmb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/golpenwcj.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gyajymnyt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gcefvqpyv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/glvvayore.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/ggunsnijl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gnvvyplaa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gdtrtrxve.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gyrhaarzd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gucdwoeuu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkoyhtmch.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gatdjgqnn.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gzohphrju.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gizdfxkag.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gvhfqbcdz.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gxtcrbsbd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/grxkndyhf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gyzxenvkf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gnpfvpxag.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/ghvpgbcgg.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/ggvwvrxlx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gmcjxblry.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gputonxmz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gefenblet.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/garemkqze.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/grheiyluw.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gmlxqdanr.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/ghidfzukp.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/godpvobee.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gjmeeduky.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gragbutuy.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/giygktsve.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gqucrvoac.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/guicqzkjz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/grlbrccek.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gntzvmndl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gldxdskku.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gxdiaxjuv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpueaizpe.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gsvqnuiat.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkcoiqrpn.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gsypzzeta.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/geceuhugo.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gacciuzwb.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gbfzrlsmd.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsgeiejuz.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gxpuyuwet.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/ggxtmsjcb.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/ggbhdwtgx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gpmtdmxfw.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gmvafvjos.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gdbxlokxl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gjrgwsuib.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gurhsshpn.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gxtbnaapo.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gogdjalbm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/goptatktk.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gmqyqhypt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gsnsfwhjk.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gtunqdtlu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gxzhrouug.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/goiiewmhs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/ghwhxevop.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/geetvkakf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gkulofqnv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gpghscsgh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gmeauhcsf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gkxvohlly.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gjngxruyf.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gnzablybe.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/guxaentrr.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gdqtmsgjr.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/guzrvgvxr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gadpznxeu.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gsruitoxn.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gtfvujhxr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/goomgwoxf.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gfzuvtklb.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gselstyyj.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gphwhpcuw.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gbxmptrdd.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gwkbdljex.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdikdlmtg.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gygxxcfyb.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gcrpgmjza.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gvoenmbyd.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gobpxhxpj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gnwcturym.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gwfjinqbd.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gumwpfuqe.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/glbrrbzws.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/glxcxqzye.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gxhkvqxjy.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gprlgaudf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gkfoixeud.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gvwjagsez.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/grvnzbeok.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gujssbovx.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gaojdmuta.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/goqbmgnja.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/geomimrfm.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gykzhphwq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gdzjfkroi.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gpvjwdiqa.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gtfmkvgbb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/glicicamv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gobwcgbmu.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gmtanpuxc.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gysyozllj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gjxgbeyea.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gddkeoqba.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gzpxspdoo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gqwocvaqr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxxuzkwxo.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gtiucvhan.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnuoojcme.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gliueqyoq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/grpeutgkw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gexauzbky.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gupnxbfvi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gpcqqojio.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gazbckxzl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gvwoyzces.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/grccuylam.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gyugayyro.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gibjktyon.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gtwrrcqqo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/grkcputgj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxvcjmno.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gamsgfqlt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gchpobttm.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/geahhqquo.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gbevreuhm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/grlidiemv.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gqpjrryvn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gdvruanvm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gsdofnjdk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gghkbohho.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gucohhxev.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/grkphlwbu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gcpjnlkdl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/ggzxcmide.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/giayfdjjc.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gntnxlbtj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/glnqijlcr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gpdzhpjed.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gdawrzrvo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gufkaxowd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gpfwygyie.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gwpxfzgoj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gojvniefk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gypmftpww.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gzbabdbxe.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gsgnyxhix.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gkllfegsv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gyintgjmu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gomagampc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gzkkcofes.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gevaxpnem.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gjgdljrjh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gpcinwnwu.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/ghzfgaqrz.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gvhdnfyng.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/ghbtzeeat.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/giopgbmia.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gpyrokuav.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gkhhsszbk.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gcfohugnl.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gegqlxujb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gmhbvmjlv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gtzqlnndx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gqlceoebk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gzfjgpjju.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gvrwynkja.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/ghxsfnspx.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gekmdivdu.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gcbapjqug.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gciqwbwcb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gcxnqblhj.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gjhsdbzot.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/godtghugp.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gcekppjuh.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gxdbftvgg.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/giqlfgrbp.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ghgornfqk.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gyxfqsrtp.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/ggxwvnaff.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gsphhzomj.sHtML


<!-- 参考信息 -->