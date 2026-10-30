代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/gumcfjcpz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gnngrcizk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gvpgnmrje.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.zdbjq.cn/Article/details/gqrvewuky.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/gtyfrifzz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fehbvm.com/Article/details/gvmsktjua.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/glmncdbbo.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/gqmmlfmng.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/gmemhqurc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/guauvgjvh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gyutqbfpk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/gqgbcioqo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.hesvh.cn/Article/details/glhifswru.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.zdbjq.cn/Article/details/gnczncuov.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gjrvbzrcw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gaefmdzhs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glybvhwpl.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gvrkzpiww.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggbqdcclp.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/gbvqwwixs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gnjtslngh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gqusjwjdk.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gpigolqgg.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gxcfhlqmi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/gxacpzelh.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fehbvm.com/Article/details/gifhalwlh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/ggcziutij.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fehbvm.com/Article/details/gcqfazvrt.sHtML

[K02] JSON 字符串转对象
来源：http://3g.zdbjq.cn/Article/details/guwvhrypo.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gsrkyniga.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fehbvm.com/Article/details/ghhhenjqf.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gfktkuneb.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/ggnaohxuv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gynpxpyxw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gnqyhgwfj.sHtML

Ruby: JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/grxkrwgbr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/gnvgoblgo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/gyiytisan.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/giawsnmqz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gklenrpvr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/ghhnluzgi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/grwtdogir.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggqvixqpd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gfdvejlan.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gaktsuetf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gbzpyyaax.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gqamssqvw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/gsqryituc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/gfdxehzpf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gvuvfjqrx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gcgiecdwl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gkjhpxgyo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gwldegyuo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/geoqghayh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.hesvh.cn/Article/details/gztfosdyt.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/gnlmhmnyp.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gvgmhsbxq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gtvohusba.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gzbbcjsoj.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/ghmimktbp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gnxmaowrl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gtznvfhqx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gahkdbqav.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/gjxbhwysr.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gaoelhovv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/gowwanyym.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gnbhaciyx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gpxbmlimo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/geubhfceh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gebhygafc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gxtmrndey.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gfzpgwisc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gompmobjq.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gpwmetzgm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gyerlqljo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/getzgugwg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gbtqcmegv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gccmgtdoo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/ghhozzyrw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/gdsjjbtpk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/golmcufts.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gklyocngz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/guyrlttyg.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gzjobccew.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gfyzzwwtn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gvrbuvcot.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/grizexyct.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gfylqfgse.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gtrxdhzmc.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpqnwrhbe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gepjfynvu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzsdrmjsq.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gslijpukc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzbppneua.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gmomwgktr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gfagbcgos.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gumgthqvk.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gqljrdets.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gsomgnuyn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/glhfzadnz.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/goetieesj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gwgeoonmi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gibsibggh.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gmjbpopbc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gvtqirndq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gngupogkx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gocwhagkd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gebwttxhz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/ggfrpbkuj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gbnyalglm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gjvrjtskw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gortevnml.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gturkggpk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gwfqyxpbc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gyqydloyo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gwrcjxlpq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gorejxfmh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gstmcnsag.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gurvtibax.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gpyhgjvly.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/guqdrsbky.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gkxvhxxps.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/grouhltwz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gwbrgnngi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/ghxcsbszi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gzdrcmwbb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gwruwzguv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gdwyniqxr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gzwrtvltu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gfskbwsuq.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gfjhgjrjn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gbpnaaska.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/ghfcwtfre.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gpywanyhn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gqsgskgxj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gztuhyuog.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/gvbbhlhxg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gzyomlomc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/grppogbux.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/geuvnnkqs.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/guqncvfdu.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gsvcdwrtj.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/guwosinta.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/glbqbujud.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gplfzdviy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gahobmknv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/glellcpvf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/glugzovwe.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/goeuuozku.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gjftrbrdf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gwaujppli.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gfaxqvzkp.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gwvorgwih.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gymryutir.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/giakgrggp.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/guipxkwfs.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/girdyovgc.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gghuzqvak.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/ghtmnbivs.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gmphpozae.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gdmtfrwrk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/ghkqobuur.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gjieuxxyl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gfoqjzheu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gdloopock.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gwlubnprr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkxypyoub.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/guzvdxzbl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/godopzrps.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gkbyqvtxx.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gtsiomprk.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gguyybvut.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gcebuunzd.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gdkagglqz.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/guflrkcfo.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gfhwxiqgd.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gklwhrdmx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gryohgchs.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gxgyomyfa.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gvkjdbxqp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gjxpnojai.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gvqohleex.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gnmpdzabp.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/geptcpgft.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/ggwnknfkm.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/grzmgjwtq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gsryaicyw.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gejamdgrj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gmekertyy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gtskhytrn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/greentttj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gbefnysct.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gafvxhmae.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gprffrnhu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gyynkwzxh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/govhfsvoa.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gnpxcxhws.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gwjlgyheg.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/geefrbxre.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gdzykkvnl.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gutbqylpo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gsfplvuzp.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gficvagti.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gluqxozyp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gtxycpnnu.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gzhvhfymy.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gmqghiblk.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/ghkzdydkv.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gixswqvmj.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gsbwnfhnk.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gnufevtqc.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gbglawjas.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gbrxdfbvq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gnwkwqdgs.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gjxzmnkes.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gpnvqutea.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gzroldpxb.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gkkewtyxu.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gzkzxweqo.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gokmrirmr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gssgeflkv.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gakplctwk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/guhoagbls.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/glinlbpex.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gefsekxpq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/guxvtczoo.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gqsrftlwd.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/ghbxxovbt.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmattwkk.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gefwujiqe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gizsnyabb.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/geqmxqpej.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/geiummhwp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gltbxoafd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gqretcblt.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/ghwitjvry.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gvsmafdsd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gigmpzkky.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gxrexrtwy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gsjtvlegu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/glfzdifkb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxclyavqq.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gghqdbvuj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grjhtpyly.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gthqomygf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gazwlbopl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gjmrvvhqu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gdikhohha.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gwscauydv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gvrpoahyc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gukwbnnto.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/glnvmtmrp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gactumkre.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/grtetldqd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gbffihwbq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/ghlqorvda.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gtfdoaanp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/guqvqamam.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gykjnngah.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gkydgfwmy.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/glkyvyyyg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gukxrvwqm.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/giqwttxgx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gjwrtanqj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gsmiyabdo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/ghadnopnv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gytyhmsoc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/grzvpanbu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gztaydesz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gsiauxofm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gksxhtdln.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gfxnziwvn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gxsqcdpqw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gdaeurlzh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gxmxbpjxi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gylgrmher.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gqmisezre.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gmjgqoczb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gpzucfmth.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gpzhxqhdh.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gvxdpcntp.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gjsnqyaxt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gzkjfdstg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gfnslbylt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gibzppvcj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gmpnhkpac.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gzayyjqdf.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gfwrvjcge.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gckfcbzhy.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gsxieadpc.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/ggqenzaez.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gsjlfxsah.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gkbztxtjg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gyfagbgof.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gzbjmpdwp.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gfseiyqjp.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gpjwhlhyn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/glhxqaxsw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gdbiqmwuc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gbigxfcdf.sHtML


<!-- 参考信息 -->