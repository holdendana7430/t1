代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gkiiahdut.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/ghjkampmc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/gnazdzwxl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fehbvm.com/Article/details/gglnmdeci.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fehbvm.com/Article/details/ggzpiqbni.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.hesvh.cn/Article/details/giarqvypp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/grudddtjt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.hesvh.cn/Article/details/gjmetucwr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fehbvm.com/Article/details/gtwesyosm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gfktvefqs.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/gsevkypxe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/ghmbtchni.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.hesvh.cn/Article/details/glffkafze.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gldcbothj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gvaflibmp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.hesvh.cn/Article/details/gonzpgydw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gwzkmrtqi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/gpvgpfqqm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/goiamvrvg.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gqgntrtmm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/gpcdjwbrm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gjypobiwp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.zdbjq.cn/Article/details/genbdutts.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.zdbjq.cn/Article/details/ghprkiymy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/gpcenkewa.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/gqjumxtqd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gjetcuvxo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.zdbjq.cn/Article/details/gokxfrfdm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvmmrqpbx.sHtML

K. JSON 与序列化
来源：http://www.blog.zdbjq.cn/Article/details/gdxejmuin.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqjnhfwms.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/gwmckrsis.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gakzswgbj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gjirqnmwh.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gphfszwxf.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gmfwgxgih.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/gnkaerogm.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gtrunzscl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/gkemrvkhf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/geynutjsw.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gewneomwx.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gohmxrmtw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/gjczvanad.sHtML

JS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gmftlsxoh.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gvhirnqtl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gdyxinbye.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gpiuvnsyw.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gvdrdpjxr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.zdbjq.cn/Article/details/gtoxnkjlc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/gjuftmoii.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/garqjdpbj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gzampjnug.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/ggxocwuzq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gnsjhbmem.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gtlscnltx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/gvsrlfisq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gjachtyjl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/ghhdsoljc.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/gkpvnzqmy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/ghgxxzfam.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gdtdhewhh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gocdarcsu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gqruvarzg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/ggablzmnq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gvyjzbqmu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gezcrcrxq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gihfxvrrp.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gmoswgbkz.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gmhytnsya.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/glhhcdwrb.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gleehzsxq.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gnayexwrv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/gasyccysd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gigfnkvre.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/ggrsoiyoz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/gxvayzjjz.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gtbjvkbzz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gycglztuj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gdrmhpyqg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gkvmleuhy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/guffnlhsw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/grfdmuxqy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gdbvlkecd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gvkplqczm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gwgwirruz.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gswigoeqd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gqjwsrwno.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/gflapfxua.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gikherdpu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gjmwuwfsz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gcruahjfo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gbvwfuuni.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/grrksvyrf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gejyyoetp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/gkhilemrm.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/guurwavvm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gspiiyfcg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/grndcccdq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/ggbvtfmet.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gumhesxbj.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/guppcldzs.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gqsslcupp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gjddizrif.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glsoztezf.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/ggepjisai.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxtyuydsq.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gfcxlotqt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gvdjstkgj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gfraekxgd.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gnaqtshsh.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gohprecyj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/ggxqapkuk.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gzwloofvc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/ghnqlklza.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/giaynecbx.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gghkhyisf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/ggkuobrvn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gfwmpkkcx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/ghntyovvq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/goxjdqtba.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/gmooukzhf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gzbpboaso.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gfgacjmrd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gmfyvjepx.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gdxeeadhq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gewaxctkt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gaofrcbbk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gdknhzjgo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gjeqinvuz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gchkliemi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gfuqmqtvn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gzpelrpte.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gwchrmspy.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gqkharuiv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gbchkmscv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gzvmilcar.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gvtsaanqn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gyqbqjtdy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gevlutyng.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gkvziojdr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gilkiwkct.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gsaqytzjf.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gwwcshwjy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gwnpbunbl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/glysfxotp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gshmfdkfe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gbgtfefar.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/goielrgdr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/guipisriv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gcyliafct.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkkouiunp.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gizkypwak.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gmegmpjst.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/goghqbdev.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gntnlknzh.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gupvnqytv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gxdtudfmp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gawtsibzg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gxeyrsibw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gbtljkgmv.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gtebwvhsb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gyfhjiemp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gtkfppcgk.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gsufbmzej.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gymaeptwx.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gnyehtxla.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gvweofvob.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gojscxmed.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gsjteaeki.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gkkrpavke.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gapnzitpf.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/guseldlqo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gijpqxsuh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/grbmwdrxz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gappbiyau.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gxtjnvchs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gbtytyazs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gpndkqzhi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzldgfmbn.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gzsraotfj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkfbiyqiv.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/goxhebtoy.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/glgfhdoac.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gkluiiicy.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/govnyyfep.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gxmmgbhcz.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gvbhqgsdi.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gjabvenqa.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gzgyczvtb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gouckjfth.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gpbqfcgdg.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gqsjmxlud.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gvkghebnc.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gbykeqcch.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gbrxuwmlb.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gpzfrpfsl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gfxxvuvpm.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gnjvphcvm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gdkkluvtw.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/giovjzpae.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gvbsqwccp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gfwdxucwp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gkqgtbzgy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gtimkblme.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/geurbkuie.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gheinqeul.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gloccjjbk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gpauqeoif.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/grwgcsnsv.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gunpqmpnd.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gyeoglqjs.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gdnwhhdee.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gqetpnqxc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gahojiape.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gfkiqvnul.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gjojlfdzk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gesdrxfog.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gxojxjrju.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gjnadmhnq.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gvhgblraz.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gppsekwor.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gdaphczfr.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbdeckoax.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gwcmahosm.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gpbgmlhsw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gezfzemdj.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gahtdftcu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gecgqygok.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gwpfokxvc.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gzobwpxiz.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gpmeqxdfq.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/glhoxmgoh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gadnbabfv.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gtypdiphp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gdalbvqsx.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/ghhqibbxy.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/guxziogkt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/ginysfeph.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gqzvoqyiv.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/grqfwrkhu.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gubjjsgfe.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gdghxpjtd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gyavmukai.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/guntuejrm.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gbfgmwvfy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/ghfvurxgq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gyfcrhsxg.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gkeuhevkh.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gpcilchey.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gpftfdmgd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gmvqslyop.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gwwhbpmhz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gdrxcsvou.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gviksgtix.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gkmbfzkup.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxnxfbety.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/ginruecux.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gxrsgtwzw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gklunfmpm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gqlcjwvqz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gqodywneg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gkqbqsylz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gpahkwkae.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gudwgdyjf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gsurkvcwr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gtonzgnte.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/ghaqpucar.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gbcxpiiqq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gwmifnfyx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gexnzgfta.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gjfzchmge.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gnjvelkqi.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gsoeusyaf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gwyitclud.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gogjkojer.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gqicsepke.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/guymerxcx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gsaskycvg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gounvedrx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gfztqecir.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gptzbmdow.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gzvvithyn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gwwimnqva.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gwsyebeds.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gotcarodb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gojfckkca.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gxpryaivz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gdsfrovpq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gnbuijnio.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gkzvecxzu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gunkwzzpg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gmnrxbxka.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gsxztvahm.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/grnktkpax.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gqxijjgeu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gcphfsqcn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gjyzqdhvo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gozietcoy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/guhiqpown.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gsuvgrnyn.sHtML


<!-- 参考信息 -->