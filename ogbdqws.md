代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/gknepctfw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fehbvm.com/Article/details/gdnpozyoh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fehbvm.com/Article/details/gollgswwl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gqgyzhrhp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/gfbqzperu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/ggmjxaopk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/ghyuwztna.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/glcishcum.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpayxurwr.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/gkgukmsuh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzcsyvapg.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/gzrhbkxoy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gxltjhyhr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gcqfhihvx.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gececnrms.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gtoontten.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/gppgwadre.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/godckgoge.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.zdbjq.cn/Article/details/gdkfohoro.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/gtddahkce.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/gqiqyxiky.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gxzjsstwe.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gxbmzcbxy.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gfvnqgkbu.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gucwwcuvp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gugvsuipq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/ghwqoxuwu.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gvidxagch.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fehbvm.com/Article/details/grcqmohzp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gbjwonenu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/godyntakk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/grmyotxxp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gkbqqeyzj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/ggkoabqug.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/gioolkfot.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/glvuakjln.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gpmgbtddc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gjchmtmgt.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gccmjvtua.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/grydfxvzi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/grzmhgvbh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gogvkhcbi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gvlucnjmg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gxkboljtq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gplszrrbr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gcwegqhyh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gijfvcpom.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gllgjsdby.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/gonbgvaas.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gzyirlbdf.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gscimqbgb.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gytfljbgf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/giotjmmrh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/gsvkqteed.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/ggjxeecad.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gpojyxffe.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/groxnqgdm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gmueztlad.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/gxgngunld.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/ggregysui.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gpmbtkftm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gfdgizpos.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gkbrigrts.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gtgrpgtpo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gjumyenio.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/gnnaycxhh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gsckmzvev.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gpgisdsgy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gnmnfvczd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gjaoitngw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gsdlasxwq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gfcvrpvbb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/ggeprrwwx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gbyyqikfj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gdkwgykrr.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gbylrqpvd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gjyiupzco.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gmdfaghkt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gmpqnfumu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gvsaqskfr.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gickcsdur.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gjsbpazbr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/goyfkdujm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggkcpyqwq.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gkmxugjnv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsadmuwtx.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gxqvyulen.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gkxvbgaqx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gxieaizfu.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gfvboggxr.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/ggsanffef.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/ghstfyubj.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/ggrfktjfk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gnpwgthro.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gjsnswicb.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gxnwoyesv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gkteoqpwo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gprxwabis.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gaxnqntbo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gtcylozls.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gurgvevdl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/ggkndzkxg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gepokmctl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/ghlhvrill.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gfahnksap.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gumkbtqwx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gggpajwrk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/getprftyc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/ggoskpkvw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gbfksxkpa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/guebiyrmt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gkgfrwvgk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gevtzekeb.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gmgqfanmp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/garclztem.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/ggbfgynhi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/grksfsvub.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gbkxkutfn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gafshvmac.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gnnzxupcm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/grukfmxgw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gpogqxjbt.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/ghuukoutn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gnmnkltqo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/genbykgao.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gtaiujgie.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gmizhjoil.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/grmgpssnt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gjnequkqc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gfyfrqxaj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gjagygvov.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gkzwnthug.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/givdllbac.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/grosbzbfr.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/giwrjikys.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gexmjaopw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gihzijali.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gyvpfuieg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/geafbgtvt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/ggvvbbxua.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gypbocwhk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gqzjvhbca.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gycymfosq.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/grotuktae.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gzwnxxskf.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gmvqjpgwq.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gtsbztoag.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gzsmmmpel.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gnwtbskxe.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gisliitqt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gtibkwrdk.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gwlpknzyj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gjwkokjwn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gpaploseq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gmzrgaqsf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gaznjnwsr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/geyqbyhjn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/grezowswl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gximjeejk.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/ggyrexspb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwyilxgcd.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gtvoppbud.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gwjazlzxb.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gjbehhuef.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gsvhwhnyg.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gpsnqjxqi.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/ggiqffefa.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/grzewczyh.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gqrpljxqe.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gvrhlartu.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gbxrxcgwa.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gnrwtliyo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gjawkkgty.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gqpohsluv.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gdjezxids.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/grgwlquzb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/goyritrxh.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gstsbspnl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/giibjegrk.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gazkkdnme.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gmmtdhvub.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gkhxwqwzc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gghikgvro.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gvjhwpdfw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gpifpuhtm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gyyzvouct.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gzgwrkwuw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gbnofivuy.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gcndxejgg.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/glcodqmhq.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gqfqsvrpa.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/ghgszuplj.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gghatmsch.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gaglrtazu.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gtampsbkr.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gpcsvfvwp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gstslppei.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/grozjhtvq.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gwemtpmda.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gjbmwqyzg.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gzesbidlo.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/giifzqbns.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/geafezlcv.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gaeylugia.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gnuaymnlo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gnjjokmra.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/glaogirkl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gbaqzfscd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gxhcequdn.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gfyaikluw.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gxppqkzch.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gzetqrwcq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gtiyjtbvc.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gltnlelim.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gezwidymc.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gdrcexpre.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gzpbrgfli.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gywpssqgf.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gyyoxawwh.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gdaznhrlz.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gtolpsldf.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/ghcckjeca.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/glvtuavxy.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gmsxxymth.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gnqtrwbwk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gketeqmnc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gwwwmkmbi.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gxqqprblc.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gqecmokxv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/guqnkczpe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gqgvzrmyd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gdftruewt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gcizrnwfb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxalluwfv.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gvpikwwve.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gutlkhakz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gqnlyqjhv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gwbpzsiwg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gqtiwchiz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gigljhtfg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/grgyoouvg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gkjcjohrv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gszieofly.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gewfpecrv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gpeiqjkjl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/goywcjzzu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gwfybrcjq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/glgyxbsoa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/guhoxymwj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gatiyjmcf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gkyvyqhhu.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gechkedbk.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gykwcvoto.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/guzlprowo.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/getzgvdhi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/guyzynvrt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/guqoskvmh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/geaarltya.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gudxfvowm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gczacseby.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gwmzyqjdw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gyzjmjnty.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/giwawlzfq.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gtgxfntyx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/geywlulzg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gclbxdbal.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gbzthjlaq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/grikwilko.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/giihgqzjj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gjcesaxci.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/ggjcihxde.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gcpwoiuac.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gfzipmwyy.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gbelkmqnn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gpjpuwkaq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gjpkuysyc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gvtufkuyo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gzospfrll.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gitoxmwoj.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/goitbkpiq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gswqkgxzg.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gsopjfvew.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gpwtoxxuy.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gbdcwleur.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gpxbrltld.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gzjcxfxvf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/ghflhidjz.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gybifczzb.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gimfngzyc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gwrlzphbt.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gdwcpxviu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/grxwcmgbp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gqxvslhct.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gultjepcd.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gjjnuyeed.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gntkqjiyx.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gpsfvclvu.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/glcjtpvez.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gjofypuvl.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/grywqprzu.sHtML


<!-- 参考信息 -->