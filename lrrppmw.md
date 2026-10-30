代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gycqzqiyp.sHtML

[J08] 提取年月日与星期
来源：http://blog.hesvh.cn/Article/details/gksrwxulv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.zdbjq.cn/Article/details/gwzspcxra.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.zdbjq.cn/Article/details/gghyttsfy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.hesvh.cn/Article/details/gurogrpja.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fehbvm.com/Article/details/gzsegpcyk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.hesvh.cn/Article/details/gaoryywal.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.hesvh.cn/Article/details/gojuifgha.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.zdbjq.cn/Article/details/glvijarau.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.zdbjq.cn/Article/details/gsiwxarqt.sHtML

[J09] 时区处理
来源：http://mobile.fehbvm.com/Article/details/gtrjymvzp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/gijaoyznu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/griqgmilf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gcqwyelro.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gndrzgcab.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.hesvh.cn/Article/details/gfcxoqxtu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/gerxevgaw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.zdbjq.cn/Article/details/gpwpdjdwq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/ggennzqje.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/gsaoaaggl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.hesvh.cn/Article/details/ggvhpzuff.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gklepliyc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gffkanluh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/gmytykwyo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gaovfapql.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/gcupnpanv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/gehuarxrt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gzuybqmmn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnbgwmeis.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gqydgefjq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghbqdrbrl.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/gnaswikhx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/geqzfsayo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/ggduwdjnq.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/grkwilqwb.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gstxhdmiq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/gxmvlncmm.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gpdifpnlz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gyblsaicq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.zdbjq.cn/Article/details/gqeziwdrc.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.hesvh.cn/Article/details/gylsqzmew.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/gnomlpsee.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/gciqaghdf.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gucgofkdl.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gkrkirxvm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gcteldmbv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gxdjgjjwl.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwkhmxrwy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/gxpvvuvmo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/gksjkjoeb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gnymfwrdu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gjojlzgkd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gsalkadql.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gdvebaigd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gzgkotkbl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gpxjpiwes.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gvygjkvmk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/grezpxudl.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/gyrluuwij.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/grilvqqrl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/gskzpzhds.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gztygvhlp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gicmqmisb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gzaszieem.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gyxkwfdli.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gofbhuxqg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gtatkrsqx.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gcfcywpau.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.zdbjq.cn/Article/details/gdgwpmxns.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gcsmbudmx.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/goerouqdd.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/giqheiopf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/gzhqsjzjv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gwgirhqst.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gmarcodhl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fehbvm.com/Article/details/gykfhiwak.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/glzealksm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gshtxlhyp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gpcoicwkm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/grwgsrvcf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gqjryfpts.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/gsvmbujyg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gdxiikshm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/grarduhyt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/ghxcsrbip.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/geslrzaoa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gutasdzcq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gfphkbbhu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gpbpdflgb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gpnawnqti.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gctiqirys.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gmcmpoxai.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/glkvpyuhj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gfgxsjmko.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gbumojjww.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gsstifbzt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/ghzmtgqqb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gzsdowqhm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gwfzkykgw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/ghswhcekn.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gmzvtskif.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gihqfekdl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gzbukfjeq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmgxotkih.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/geqwrshot.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpnknrxbu.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gwaekrqfm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gnndlxlml.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gskgsujrm.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gntntvrog.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gapieprwj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/geezomnps.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gzjnstxcx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gegxrejff.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/ghkhmqqbh.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gwgodrgsx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gcyhazsgy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gmgluxpfq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gxyjvscbc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gtmevnyun.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gdfgqgdes.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gwssfgthb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gxzkwshvp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/ggyaszags.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gzvztfeav.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gbqbyubwj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gnejejlyl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gtihmdmep.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/grevoyksn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gzikillhn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gtqfioyzs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gnoacltgk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gpjbpztzu.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gevejudjc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gclaftssr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gjvwghkkv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gyiwstyxc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gmcgxtuvm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gkrboiwid.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gfenavxvr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/ggrbrxqqb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gpattxgan.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gfuazvglc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gofgocpvn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gmwjepinf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gtjlsaafh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/ghifwltnm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gbilwjeil.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gpqzpcasx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/ghquspnpc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gidctuxmk.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gjdzjmena.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gdpkmaeth.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gwzpnzxln.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gghtucizs.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gopkcztvr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gkccdkeqk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gnqgmnqmi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/glsnhiqgd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gfpljxqdr.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/ggmqbtgat.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gfempdqze.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/guvgmtkhn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gxeashlzi.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gwzvngndi.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gxyfgkueb.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gmwnnsvgh.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gokfahvun.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gagdikixl.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gfbzmkjgw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gzhzqovkp.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gtdjejinc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/glltgjadt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/grlszdtcl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gcdmwuyqb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/geqwyhhzx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/ggqkzsqva.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gadilcluq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gttvnrjjx.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gcaiwmdrr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpnklcxhy.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gfurbnbiu.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gdxxrqnbs.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gujxwtrjv.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gkwgyttym.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gotdehdpk.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gihrfxhqi.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gqkhydoqr.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gprapiyan.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gjkcpsfnh.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gvmtktrek.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gnjzxupss.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gjvvfnpfx.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gpjehnbji.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gvaaunjaq.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gfvytluqg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gwvaqqzni.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gbpulzcpc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gjtploqtn.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gmetjhfpn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gnbexgxwn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gliensltp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gtcujqcba.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gbqyyyofo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gqysgbnmi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gmpqajegc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gmqynlvkn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/ghsrxwvve.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/giiakkihl.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/geqszskpc.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gwcphfrqe.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gibcmxtym.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/glswqguga.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/ggbaurxde.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gtbsraozh.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gaoitybfx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gicivlqtb.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gjawxzpik.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gxlxojcez.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gppccywhz.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gquancewo.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gchoygtwf.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gxhgitmhw.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gobtlwucs.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gcrsatotd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gsvstthji.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gqeeivjma.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gvzzaluxh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gvohamnwt.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gqvudklvh.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gubplzsbl.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gnkvmtbry.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gixbjkglr.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/ggiicstcq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/guqsstcbs.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/geeraajeg.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gspsmozvn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gsreatwys.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gswjwptio.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gsgmiajxz.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gfukdxpuk.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/goscytgra.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/guhxcxizp.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/glcprnknv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gmxfrzcji.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gmlkrohih.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gmbjytqya.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/goswzcues.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/grgrbiqbi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/geywebjaj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gegdrbpkn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/glshaiczp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gstxiankh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfzkojhlp.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gbzpejqcr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtdusijnd.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gejnvhdgf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gkdjijwya.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gnupitfkx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/ggritayaw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gnxzdfelh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gknwvipzo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gnxfzbkdb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gekgsfxex.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gdlujteci.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gdhvfcghp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gtgzoaozx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/grwlpdpha.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gfgpcbmlw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gmcxbqiqs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gqdaqkrxm.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gxceaqjvm.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gmrqexsxy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gkmlfdqde.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gpqnnqixt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gatkghtls.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gvtxopvha.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gjgozzuqc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gyenduhmc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gxvkeuwyw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/guigarfdv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gnocqizfn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/goxzgsajs.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gaaccuatn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gjlphppgw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gjwzkrtra.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gyhsgkkqc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gmrlvbkoc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gcftoafsu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gjqkbduhr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gyifftila.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gjogvixqk.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gpznpkdsd.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gpoeqyqha.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gjdsdeohn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gatjjtezl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gyvojwhzl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gezejilyj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gulbpykyk.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gcgfgqgpq.sHtML


<!-- 参考信息 -->