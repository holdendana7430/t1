代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.zdbjq.cn/Article/details/gagvtefed.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fehbvm.com/Article/details/gkcgjlxkw.sHtML

[J09] 时区处理
来源：http://m.share.hesvh.cn/Article/details/gselopuxd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gahdoworj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gmbnxxxme.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gndoozodo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gwnxfkrir.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/gtdxirswf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.zdbjq.cn/Article/details/gafqblqde.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/ggxohdsfc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.hesvh.cn/Article/details/guomtlcuw.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/grituvean.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/glepysopy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gdxhnyehw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gfvxkbrbi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gvskzlfoc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fehbvm.com/Article/details/glvlzwscf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/gbddfuedc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.hesvh.cn/Article/details/giyjmlkis.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gefpchqrc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxjoniblm.sHtML

K. JSON 与序列化
来源：http://www.blog.zdbjq.cn/Article/details/gzhomvpwn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvjoingda.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/gbznethvt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gnlmcfwvm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gogohixbf.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gikhibejz.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gqojmmmmc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/gayxfkzqx.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.zdbjq.cn/Article/details/gznlxnsbc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gpfppqpbb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gahnksyzk.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/gplwpydfw.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/gbqkurliw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/gitsrxrdl.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/grbrbdajf.sHtML

TS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gbtsvnsbw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gaykqxtfj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkskrsak.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gjgkhigye.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fehbvm.com/Article/details/gybcwhelq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gmfwuwrvh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gunsxbfvd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gqnkxqdbx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/golyhycsk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gczbeoipz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gbkksfguc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fehbvm.com/Article/details/genskjarq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/ghpawfikt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gwpqqbnkd.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwuhjeveb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/ghrumncjw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/giyrhdoti.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gmwfvceub.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gbfzlsbzq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gqnhndoyz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gkxhmjbzh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/grblryhpk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gkenoadwe.sHtML

[K05] 深拷贝对象
来源：http://blog.hesvh.cn/Article/details/gpjdxuukh.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gerfevoor.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/gjtupbtgd.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gngoglzux.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gnswexuhq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/gmkkuffza.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gnneqltea.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/gjgaflsjz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/gnovymuiw.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/grpyvmsuf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gcvppjeep.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gbklvfrlz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/guvndmeck.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gliwugzbm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gifxjchhi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gmapjwweh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/ghhiggtps.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gxjhagjuf.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gioehbrmm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gmoegexmm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gwizdhvsd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gulpmithv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/ggmfjoxin.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gwfgqjvnz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/geuvlnran.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gohygshxx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gbhlibslf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gcrwvslaz.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/glirqufhg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/gsilacpep.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gefeiwduf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gtgqrwgqo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gtnjidacw.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/guljfxrxl.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gghbfaasu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gkdgslimk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gixusunjf.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gqyajcxpb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glwenkloq.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gnizkmwrd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gnmmnlugb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/geknevjii.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gvutybwwm.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gplbhibzr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gstasszjz.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gskjrlqgc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/giffhdowq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/ggfzccixw.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gqagmenqm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gqgabbgfr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gplwvhcam.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gkgmpqmkb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/ghqxlpewj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gqzrtwazf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gcdiqvnuj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gtqqlfzsu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gihuvlvcn.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/growomrhc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gkgqhqekp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gblewnjaz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gcvcehrdd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gynqmsdpr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/givigyanf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gnlhwlhav.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/grmmunmgb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gpqaaruld.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gsmmreerc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gtyaltybi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gmqigdzwh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gtkfdmrlm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gndljovuo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gcgutufes.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/gyjadhrtt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/glirdzyld.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/grqtucejv.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/glwydhqqu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gukgfrqrr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gawffnayk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gqkpvhkkf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gsucvdzbt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gzxncpwyi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gtmbsomck.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/ghaejkaod.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gihopudrk.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gsmolothg.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/ggrhhbicz.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gihrdyqca.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gmpweefvu.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gkklyexwb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gvovjofdb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/giarbnwca.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/ghsraijnw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gznoductf.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gsrxacseh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gqgcpownb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/ghbkrmtfw.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gqbuhzvcz.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gcdzkgrcw.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gbzasuehi.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gfzixyusq.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gvgnsawfh.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/ghxgvfppk.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gavfmigrc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gqacblftl.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gudioczur.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gfpsiwtwl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gpwuriqwt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/ghodvvamu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gygmnuxgp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gdkihycgm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gguimfskn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtexhhfbu.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gcslcmsps.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gefeouqhv.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/goupnlpge.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/glclizoir.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/ghasysnph.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gfhqjlvnf.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzytigarh.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gztvpmjin.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gxutxbgzo.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gkhuhafho.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gcwgrbive.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/guilruihn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gutzynvhh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gkcwfqbzr.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gmeeidbkt.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gmrklvzfj.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gcwbwbzuq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gnkhkastj.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gwhymoxhc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gsiitoglq.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gtqqkohnz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gufoakojn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/ggmeajstm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/ginciybov.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gzlmeiygh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gfqbbcdpn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gwqqcbgdz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gbircucco.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gelwvmxxs.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/ghabsqmtv.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gctbpyzdo.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gjzevjaqg.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gkyfosmpc.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gdovxbgnk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/ggcbvvdjq.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gfhubzhgq.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/groftvkjq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gopezzdkr.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/geldrtiub.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/guwckmntp.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gegesolqc.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gsfhhfwpd.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gkgwucafj.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkbbtoflw.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/giftjpkmb.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gtjtpzgbe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gbhkxojtk.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gahtzibpj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/golgrbozf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/goafftgok.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gjswksuve.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gcgsfdqtc.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gijyttglc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gughpzujd.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gnlzzwyqs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gevdbqjrj.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gjbveovqr.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gnhtnzwbj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/ghnxrgouc.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gxyclgyre.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gevcynpki.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gbmoftgig.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gmaurelxj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gusbarykt.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gxfvstkxb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/ggicbupts.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/ghoheubdo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gyvkwiezn.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gdqxfbwru.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gzfwhlhnh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/glotwduhv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gmhownzml.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gtxihawju.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gnlbepdvx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnbfzaiiy.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gbntnkndv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gndtjwyql.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gawxzwmjw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gnssplnls.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gqaofbrdn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gnltronhv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gxeakbern.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/glxrrvmhy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gavhnfmxz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/ghybxltcj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gbzflflvf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gjcbrisgm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gyhwxralz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/goybqryfs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gymfcdict.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gelsxffdw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gpmacsqzw.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gbpejgkyc.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gmvoagwvv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/ggogcrmxx.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gxohugpxo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gmrjskjkn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/grhhtzfsf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gxwtumzku.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gzidlbjjw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/ggkxpfdpt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gnblghkcy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/grftqbmfg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gvaisqfet.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gejfwjbxe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwqxaqctp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gacpoaotg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gujwcwaiq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gnhqtaeas.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gjgrnyvcq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gqxnykvyx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/glnoirjkc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gjmkgiwbk.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gfxlcwscv.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/ggqrnawju.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gwuvmxhuc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gmdrywlre.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/grsxhxhyc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/glvyufhrg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gmjimpzxl.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gbtqqreil.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gdjztztde.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gjujhofmb.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gfqjlxcni.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gvzvwrlzb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gxzptlrcb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gvkblkfep.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gkrpdcczx.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/ghywyupkw.sHtML


<!-- 参考信息 -->