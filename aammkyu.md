代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.zdbjq.cn/Article/details/geituaqfe.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.hesvh.cn/Article/details/ggkxyypnl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/gxepfsixn.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fehbvm.com/Article/details/gulcmnmvc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.hesvh.cn/Article/details/gtbglhukj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/geqryrbdo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.hesvh.cn/Article/details/gjoicwohn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/gqkxocmgx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/gmqjnwafn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gguvadgyx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gndnfgkuv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/gynnkdeil.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggeftrypg.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gvbjtxddi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guhnfcqzy.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/ggbpjmmiu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gnozjlkxs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gvfamrzbw.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gjtwxjxnu.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gaikbculi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.zdbjq.cn/Article/details/gutwcmrnz.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/grlkejdzj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fehbvm.com/Article/details/gqxacntqw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.zdbjq.cn/Article/details/gelsmwamu.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fehbvm.com/Article/details/gpfyibipg.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/gbhtuskot.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/gbykiusah.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gaxmtofvy.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gqahtooyl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gnygdhsgg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gykkpogox.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gzhhhamxi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.zdbjq.cn/Article/details/ghqgigaep.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.hesvh.cn/Article/details/gyslhmhny.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gqfpmvbea.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gwhojuqyn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/ghflxjtdn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/ggyezakes.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/gkonvsqeo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gsozbtqjn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.zdbjq.cn/Article/details/gijiqoecu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gllqpeihs.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gvhgucxly.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/grqbmzafx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/ggmwbguwz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gpbuiuuaw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gqsaupisa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gurucxdzx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gxzondqbw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gvjpmmjjc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gergrescm.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/gjkzdoloi.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gnmdfzloh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/ghhdgdpfw.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gatoledhg.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gupawiavw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gbotbecki.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gzlwopopz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gkzvcusqo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gonigqyfa.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/ggdcluzbx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/ghjvekewc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gwbjdergb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gwnmoaygc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gmfvodtjs.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gshbfzzke.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gdcochxdy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gmhxdeotv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gviudwgmo.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gvymnqihd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gfbwcvchp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/goyfjmqnx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/glhddrzmr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gfbtcbgum.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gkbpdsaov.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gtpuegpmv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gekcfflew.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gouqzawvd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/ghgghbwsf.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gksnnoyiz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gdsefgeyn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/ginxvvaix.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/guvrepnuz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gdxktjvag.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gfocctvmw.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gzntbpslu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gprypgmfy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gizedugfu.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gmpyqwhaq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvlhvkcpe.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gxvhmkdpv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gpjrgddak.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/grpjttpfz.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gxktclfiz.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gkbhmqnii.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/glocmhcyu.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/gorklgmgk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/ghnbbgssl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gukqmwatr.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gamueiawq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/ghtcbmhna.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gasnxkimq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gxksfzuwe.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gbgkspywu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gutsklccb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gjeiuljtj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gojmgtsss.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/ghisgzitn.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/guopgyxat.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/ghyayjhwv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/grteuylkt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gjmgvakse.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/ghydkqmqr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gkkbbvlun.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gzbzsraow.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/grutmnvwe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gutdnesru.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gijpvzrbr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gnqiqotfk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gelbnrsip.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gscvnjjsq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gnqgpsdfk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gdraunupn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gckxyavyl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gozepwayr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gpijaxqta.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gkcspyvlt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gkjnsopfb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gytvsxpey.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gpfyzmuia.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/guahddhlw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/glltnfett.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gdjsulsyp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gghvyapep.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmmbzehxg.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/goemzkber.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/glorlmmuv.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gyejynptj.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gwxjbhnor.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gevcwxbxv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/guiqdnsxe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gdyytqkox.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gumwqodux.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gmkusgldb.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gbpyirrvx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gpicxzept.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gecdftysr.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gdvcgkufq.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/goafmhoks.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gsiieqzzl.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gkylnucwz.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/ggrrhdzlw.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/goffenwbz.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/golpavzhd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gytzeclvv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/grtxnoirb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/ggldezwhx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gbjglmagk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gdnfdobgu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gsqnraxxm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/glcniiaod.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/ggonqyuqk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzuvxntwm.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/ghzexliez.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grdmoumth.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gzchbrbel.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gktooruzx.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gkwcpykhx.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/ghdejvvmq.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gwdubuzgu.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/geshtmcbl.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gitpxzeby.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gfaassftj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gsecerqkw.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gobpqfxte.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gxrhpegyt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gfureoxla.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gontudcfw.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gspuhwscz.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gpnwqotir.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gwjmcnzld.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/ggmreckda.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/ggnleqsql.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/ghlmfbjmg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gwqouzqog.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gkoyyxsto.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gztlolxnu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gxghhjrdl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gfstjnikx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gltlfhnjz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/ghxshkzzs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gvcvzygkh.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gctqsjikj.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gmghzfdoi.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gywxztsej.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gxsdsnilb.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gftimpblo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gqelvmetr.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gppavbozq.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gnlrmziel.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gssmrkcpo.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gbdyfydge.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gzafidebc.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gzierzols.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsqlbrxjk.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/ggolnpddm.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/grtpygski.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/grtfhkdkb.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gzlmwepnw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gezdgswuf.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/ggmisgdxs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gqspcrsas.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gucuseoab.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/grnkssxel.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gyidnvmil.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gaxrjvbzu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gpelanysy.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gsqtdrmmk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gmanotawf.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gbzqwoccz.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gssqssmjh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gklobrknn.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/grjvajsdp.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gbuyexnpq.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gtvkwryah.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gxizkowea.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gglnqjxxc.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gqoaocjsj.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gedkzbhhf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gnopwexbp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gkqwaafvz.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gmlecgldm.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gpwrkmeav.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gronwlmmu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gavxucial.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gwroxupum.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gjwztjdyr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/geugqqnsf.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/grvagihig.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmfzhaejb.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gsdnwvmpr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gcugtehrb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gvkfedbks.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gpaiszfai.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gcluggzmq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gmogcjgaw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gubsynfji.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gyodsbcrz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/glgtkejsk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/ggbgxckmh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/ggprmbnwl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gfpjkuoku.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gbmflstpu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gnalboerj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gzmgxuchj.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gwdgayddw.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gmhljrqsr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/ghjhqokno.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gwlcgoenx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gqbbnrypo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gjbkzghuc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gxypbstnd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gerggxehc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gugwtfeis.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gshmgxpep.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gkzmhcnht.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/ggywrdzpf.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gucihozdc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gzgikfpef.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gqhbcqpbv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gpmmpkhgh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gvxgouypq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gmwkiqvix.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gadjgzwfb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gtltwulzn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gwwoxzomq.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gwvvkfmqw.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gvefzqvhl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gchfsbjmr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gbwyhgslp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gmkyvewxx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gcebbdxgs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gfwhtbxbd.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gdrngjuqt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gdyuwoivu.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gyeunmvja.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/grprjtfis.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gqvjyftyb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gggfjbhwe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gjmhofakn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gydefqjph.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gzzqruitd.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gttbwjwtd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gdxqqduka.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gtjvlabwt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gpfqcuyvq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/ggahsweli.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/glrkqzxir.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/ghilzzgsv.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gzmjzhslt.sHtML


<!-- 参考信息 -->