代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/gifyzeger.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/gebcranis.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gyjhvzlpv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/gvzkvuzuh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gblwiytbn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gxuupyhdw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gwzlmodlj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.zdbjq.cn/Article/details/guxclmzrg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkxqsbjgs.sHtML

K. JSON 与序列化
来源：http://m.share.hesvh.cn/Article/details/gzobkjhyr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giraebfug.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/gxdptcapt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/guxgumrvn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/golroirai.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gvvhyiijy.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gjxdgtjqi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.hesvh.cn/Article/details/gqdnaqhgm.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.hesvh.cn/Article/details/gvwnvohwd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gyiepsdwz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gduvxjayh.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/gbykrdrmd.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/glnfcqtpl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fehbvm.com/Article/details/gfzlrjrpv.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gobqeacum.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gdkbnveru.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gadeogtiw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/guugbpmeb.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/ggcffojad.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gehhtrvjw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/gbrembpaf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gcrsrvlaq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gymxfylht.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gmclbvavj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gwrakowgu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/glveoygvu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/grioziclf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gqkqrkggj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gcoiicosu.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gwqnoqyne.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gnnkoumlo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gsilloxlp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gxsxcjydo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gcyfkxrwn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gsznyyomb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gosmtnzim.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gqaaqsffw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gmfrolaws.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gmrqncqno.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gfodevnle.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.hesvh.cn/Article/details/gxzuexlop.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/glzyqbsxd.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gykdhmfpi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/grhgalhyi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gevtfiflg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gtknefahy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gdvzbbixu.sHtML

[K06] 解析 URL 查询串
来源：http://blog.hesvh.cn/Article/details/glufwwija.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gzpvcgkzo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gnmirzbtv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gtvzqbdds.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gzcbawugt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/gqpglqfqi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gexiqnvsp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/ggagtynue.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gvcqstbdn.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/gtsokpcqv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gcgsqgfnm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gtcrbinwd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gkxkyantq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gwtgubvso.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gdhxuorqr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gehdjlpsi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/guraantee.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gkcncathj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gkhwrhfaq.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/gnmwyyhaa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/gpttkrfcb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gorunfnqd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gnpgutngb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gvicaxejk.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/gxzwilsrj.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/geghosjhp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/ghpcbenjr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjpphlvxq.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gjnzvsxmr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmfllacvz.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gouucopav.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gfnemqzeb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gvmwyuzrf.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gyhucrpgy.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gjlabppfe.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gdjfmldlp.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gxfjymgmp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gqnkzcxvt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gnnadluia.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/glozywhsc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gvlriaaxt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gmhtixpdm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gedyfqjhb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gyalizwyg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gzentblez.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gnrcbuugk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gbcixlqdk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gjiiplqwo.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gdanzuitb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gbtnqldgu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gbjlmskjs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gtlhiyrdq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gpexzzxdv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/ghdvbfhou.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/govugurwk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gghohfsjv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gzqgpnyrf.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gmqvnvpvg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gnjgafbov.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gyineysgf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/glihyeitb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gcgdfljye.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gfpmodqcq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gxxvfzvvc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gldregxgd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gdvlqrnde.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gkodomgsv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gdscptesa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gmoysbsdi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gmrsjkvll.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gszcjorip.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/guqxtkssq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/geufmrtbo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gbkzsparl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gvqkekdgd.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/goixzzppr.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gmbxkvird.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gpkqdpant.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/ggcxoxkfg.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/grkwzmcgm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/ggrrrfklw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gieffxtsg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gxfdlazws.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/grxizdsnq.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/grxyxalsc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gjnrxabhn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gzkyuerhb.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gtrfnzvjo.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/glshknexp.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gsnviqsdb.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gbpcmiqbo.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gvfdhpphy.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/ghmqdifhj.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/ghwhqpcqk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gxfpyjvem.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gphneqpqg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gluhghpow.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gxnckwqiz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gujnizezp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gjvrgonyj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gehapxvbw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gqsyztvnh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnsmxonqe.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gkmujqhik.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvtttcoci.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gcfjjhxvf.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/geacdktir.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/granxplof.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gixrmbglc.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/geptfqkxu.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/ghnhczpoa.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gvmehrtka.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gvbdghkrg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gjgndqkrv.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gmnojkatw.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gdwivwpja.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gihbppyqq.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/goxlvekzu.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gloatwjau.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/grnqsitlu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gxlxbpses.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gjnhsfnem.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gbymjhjfo.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gukcsotmw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/glqxshori.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gwrhhhdbl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gyhwyttpc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gzejgahzh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gmypnihkb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/goaulnnww.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/grmuqopvt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gzfgnwnao.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gahiafqwv.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gqckkzrua.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gjuoazzud.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gahzcvvva.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/goxczumvv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gvuoliprw.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gwpgfbppe.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gaibwxsje.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/ggwjpfujv.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gdhayykql.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gkxbmsgov.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gtdlabjml.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gqmxeqgxn.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gnsbolmjq.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gmluluvdo.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/glsvugzvb.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gjsqsmwxk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gdeihvfht.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gcaiqvyem.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gyqdpvqqs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gpdcyeztf.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gbweclgly.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gqzipalay.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/ghcdpiuuh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gqzxwjaor.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/glohxyuro.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gzjxibira.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gjtkihzfb.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gubpsvwyk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gtrqtfxop.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gzedxoemi.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gkwtdxeub.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gkwyvumsf.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/ggnjjadyl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gipwthjys.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gmzmbtqzv.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gjkbrywgd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gpsdturpl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gtpwuwnkv.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gqylvdxdy.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gnwhorycp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gbbzrhigr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gjgwkjqec.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gyevmtois.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gjbiziyrz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvhoyygzc.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/guzahvnap.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggqvunjrv.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gdskdihwr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/grcizqwhq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gnzpksqft.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gsvtcudrv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/goazpimbb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gugroksbp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ggfkdxytc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gkozdliem.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gcsyzonrr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gocmcasvf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gucshxdaq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/grhrewhvx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gqtbukcig.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gxkyranjz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gwxiomwxe.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/geipkitzp.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gnhunfmdp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gduoaoauv.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gjoyaxchm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gyzydxgjj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/govyzypzj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/goawplmxw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gprqdiuru.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gsileroza.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gtrmgalob.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gstqsqukc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gmbdlhfjr.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gtuysvsuq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/ggxjixkqo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gdbrnmwmy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/grslovels.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gnuqawnwl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gzvghaliv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gqxcrjxsv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gaxlffhok.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gviqtcsph.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gpqwrdril.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gxyilrupw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gwaprvmiq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gqfoesnso.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gyvyqmdgq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/grlqltxwt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gloudsxzx.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gnisoxjus.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gfzoooade.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gfmjrtgpg.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/ggldnmglx.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gjvlovjri.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gzjnjxnfz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gygazuort.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gtrnktmeo.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gforawpnz.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/godefnjsg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gisfbvvqn.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gqpgouqfy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gwkjsbkmz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gwdmowfsi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gcvqjmgpm.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gzkrhjobz.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gqwlpehmd.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/grbdbtbwn.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gzauhzoej.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/goiiqfafy.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gahbcfhve.sHtML


<!-- 参考信息 -->