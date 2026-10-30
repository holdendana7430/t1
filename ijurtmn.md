代发 wailian999

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzhejyscb.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gjobkeioo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guhcvhrcy.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/guaduayau.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gqunhyfwi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gmgjerqvg.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/grdytjtmy.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gnexxuloc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/ghhimywgx.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.hesvh.cn/Article/details/gvyebueek.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gatjkpsvz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gepmzqprj.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/gqdcnxlsz.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/grzybwadp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/giobjxxlu.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gokxbsues.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gufcvobqo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fehbvm.com/Article/details/gzehmzkab.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gsuqkmvnq.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvfldtcir.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.hesvh.cn/Article/details/ghzxngpnp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gchbcsevk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gmrchpibr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/geukmoskr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gtviniboo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gqmtpxabn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gkyiftrnk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/ghqqqprdj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjieekjui.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/gdmywpkqo.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.zdbjq.cn/Article/details/gzngtbswl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/gtnrzyliw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.hesvh.cn/Article/details/gmwfxluop.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gpnwtxbzu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gqkihruyt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gkjacvtna.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gdefgdycx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gznolgdfr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gbvjpkvqf.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gmjybnxyi.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gdeqdzcbe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/gmytpgsyb.sHtML

JS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gpwmrnwwa.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gddmdbqqd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gnmcjqflm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gcdqwfask.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gwqppismx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gktybixyl.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/gehpvnqcq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gbplcblcx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gijtjrujl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gyqhqricd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/grmoltrvv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gcnygchxs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gthebamme.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/ghmeaiwha.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gpoecyfrb.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/gmtwbqwkm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/guyrpwugu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gnhurtrkj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/guexikxen.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gpuuyfahy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/ghxhbjhbo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gjyslnymn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/gnluosnoc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gmpccrlst.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gvqrgoubt.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gsznyrsdg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gmulrsaat.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/grhwxmpbc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gimqzrydk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gorqyqkeb.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gntfveqlk.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gdiynawcd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gkyabjosd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvchkftve.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gmehvkpnn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsdxyqzsu.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gnhvsmurq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gpabkfkyo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gxdouqqmf.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/guzydctil.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gddjlxrtb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gjfrntyhi.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/ghysvxzlg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gsigbjvac.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gpcxldxtn.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gfenbouhm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/grkrsnuqs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gvxnpxnum.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gsuwpuiys.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gfrbmzthz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/ghgbfkrlm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gtxpvzreg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gxlgtthhe.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gbtwjhoow.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gsmaoxzye.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gzwsgiqlu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gupewwlvq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gffnlfgum.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gzuqcqiby.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gvoymhwmq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gcdyyixjv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/genjcbegf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gysjerxux.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gcsgakgju.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gtnegsxxe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gbcwsbxid.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/grkwzomlz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gynpsafpm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/ghxvelliz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gwmpanlmr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/ggqbcgicy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gziprufhn.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gjuhozumj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gtoycigvj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gbeskaasv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gfurhvikw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gadfmdrsd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gzbxdzrbl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gawlfzrjs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gzxxfyema.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gvarmoafq.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gxcelljik.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gtikijjul.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/ghqxjanam.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gajblaiox.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/grfihdfci.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/ghjyssnmh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gdryhugjz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gflysvrma.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/garbynwch.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gzfkltdjy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gfsmzigsi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gdmowdsuu.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gsjtlhcyh.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gpmluihai.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/giojplfmu.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gqayxequx.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/glmovuwoj.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/guyctybgm.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gbxkaawzf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gfmtctcff.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/ggxylbvri.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/ggoshjoik.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gikdenzyy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/goonuicio.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gcoyayqdz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gblcqkuvu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gkjgcobxc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsuemrdha.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gczluzgyg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbydtikvs.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gmkzvhadk.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gmtvzzzes.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/giayriyzq.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gefexzfpl.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gglvaekdg.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gibhphtds.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gnqznfnnl.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/googyoazi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gzyodjkvd.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gxnfwllka.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gkzycvipq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/ggfvbhsqn.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/giicabbyh.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gjdittqyj.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gzpbhzkjb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gvedopidn.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gsjecpise.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/ghlzmprem.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gaioxczxo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gkwyqdbkt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gncslhjce.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/ggoqtvxxv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gilpsqwot.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gyhpyqboe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gbrlcnnwn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gazsciwjn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/grybeicrq.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gazyofdqo.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/glflemrnv.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gyayqcehc.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gmrcoffvq.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gadnmqpej.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gnvuukavn.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gfwnolhji.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/ghqmqajgg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/glwbyclbo.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gkhdamrnf.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqffazhla.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gbhdhojmp.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gwwfnhzzw.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwuuryupr.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gdekhszef.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gslkxvzem.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gfbigzakt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gchiphojd.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/ghvffoyvp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/guxkaxdgg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gyszqpldg.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gmvlymgbp.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/glqqfbauv.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/glefiuvye.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gheabtcnm.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gappwbonl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/ggdzsvkmq.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gljgeoifh.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gyruantgv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gyxjxdvss.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gfnjernkn.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/goicxezvh.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gfplvyoll.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gyqakowvf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gwwsakmyv.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gkiyhakao.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gaatatgsv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gnwvwrvtv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/ghzejrjud.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gqjcfmhxs.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gtlrkmyzp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gyqsrjeiv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gxgettdqj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gevrnshad.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/garuiijws.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmgdjfkjg.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gaafgdvvx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmgcwjbcv.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gwgmilmeg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gcjbfmahb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gfkirbsww.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gywdelpwy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gcavkrqzx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gwpacpqcw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gvboicyai.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/granucxoc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/groscutmo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gsvdaepjv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gljzejvzf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gswmvueaa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/grbvmrsak.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gnbgvlxqz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gxqohvhph.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gobqndmeq.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gddvtugia.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gunzdompt.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/ghiaxqxbc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/guwnmxvml.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gymjuzexh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gmdtqbxku.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/ggiymaucd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/guavpeyqv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/goatzkchr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gdhrpkwzj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gcrtpsqsl.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/grigcpcub.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gsvcnxcep.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gvuaswpqv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gjpnnshoj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gpappqdos.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gztnhodmc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gruejkhkv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/ggmgyrsot.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gxsdrtmet.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gibmiaxco.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gaynffvqp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gqpxxbkhu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gkpbxpckj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gzdamcntb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gpuyxenra.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gilkfzsrs.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/grtendmzd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gzggmtdog.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gfwbsgpfz.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/ggctlcizx.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/glprgslao.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gjfwcnsaa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gjfmgvnfs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gqvukauer.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gkesfodyd.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/ggdnzojfn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gnadndvex.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gejsakqly.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gdngqxfnm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gzwuzzmbk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gdbklqtlt.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gmldmxwau.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gagxzgnot.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gnmxkxsqz.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/giljomlko.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gaavlatlq.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gipxfvups.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxjfcljyh.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gcujhxzqb.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gzeqiwapr.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gxloeyaqa.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gxdiyuudr.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gbynbupge.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gvkbuzizq.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gkoeseana.sHtML


<!-- 参考信息 -->