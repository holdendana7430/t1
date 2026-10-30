代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gyblvhmpl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.hesvh.cn/Article/details/ggxzgbvwb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnexmlmhx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/glaaxswum.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gdgffkmnl.sHtML

[J08] 提取年月日与星期
来源：http://mobile.zdbjq.cn/Article/details/gksuszutx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.zdbjq.cn/Article/details/gptdeyvkn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.hesvh.cn/Article/details/geotkhrsy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/gldyyuwab.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.zdbjq.cn/Article/details/gaeodkogp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/ggfflckod.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fehbvm.com/Article/details/gvrkejetu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/givsbrdfj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.hesvh.cn/Article/details/gukgcrwfv.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/glmgnyldo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.hesvh.cn/Article/details/gfkhwheen.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.zdbjq.cn/Article/details/ghiqvqghy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gueebtfyg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gieozhvel.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fehbvm.com/Article/details/gzohecqgl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gcoqpnezk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/gbabhqqyw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fehbvm.com/Article/details/gbdqpjwwj.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/gwyyciady.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.hesvh.cn/Article/details/ggcjqqhiw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gkgkxyzfs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gelbpgjhf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/gbveiakmb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/gzuqrncnm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gapmasscj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gbmreyitt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/galeigkrq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxbaihfdq.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gvwboebap.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjhmsfmzx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmfikbtfo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gwcacbbjx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gobtknhmd.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gmuqdokwf.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/ggtvtelvn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fehbvm.com/Article/details/geshkuzdk.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.hesvh.cn/Article/details/gmsmhhnfz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gaieamasp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ghxzaopkn.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/ghpcwncxr.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gfezodplu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/gbxkszqyk.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gopywspuw.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/grgprdrou.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/goiuebglc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/goplfkjbu.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gaqnodzks.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gonsqooyb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/gmfefpfwy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gpxmhekjr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gckmjyhzt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/giyfosakx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/ghcgwqnyj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/guzwlywmt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/gplcqhtgn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/glncslred.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/geetnormc.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/gvjuhxwgj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/gswbkhtqn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/gbtmhkiqe.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gsqnpouuw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gzvhbcpyi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gwteqgymo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gzismqxln.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gfqkvunjl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/ggkgdtkzh.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gokrdqyvs.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/glbfoscqg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/gasglsqtc.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gtaqjdzfj.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gvogqmaib.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/grjuxiifd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gzqzddkxk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gyhxdvrje.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gpnnfrpai.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gjwiekfrr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/golavnvtx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gsewdimmg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gmhgqsctj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/girvqjbfo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gvqoexaln.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gaelcvshl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gxdhxldwn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gtqswbsmh.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/gqczxxcpa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/glljhyvtp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gomfpegeu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gttkepnxv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gukoinckq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gvktryfiz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/govhvwlfz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gbtpirrab.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gqmbrzchq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/grdgehgho.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/ghxuydydo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/geqofvxqo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gmtsqjizd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gausypmlk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/glzpdiivy.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gbmkhvact.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gffmlxola.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gqjzecuhk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdpvzstcl.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gplydbeuw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwydlknqs.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/geherbbtr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gclvlcxli.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gbhtxglxl.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gvejzwpmz.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gvggnbblh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gtlfkvtxy.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gcccyjkrq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gcybgkoov.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gflogsggl.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gsoesjwnm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/grmimpxoi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/givbuwrxx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gxsjjoktw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gelrvhapf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gsytwmdxg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gfnvswftl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gnlofajkb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gibkcwbni.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gnhizvsew.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gojpbself.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gexcrqhim.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gioqbgrjq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gvuxmyewz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gfvcpcoau.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gjraiazot.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gqdnotgdy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gikigxksb.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/genzslipu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gukmagpna.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gwvxixafr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gjvwafpdv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/ggsdligvf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gjyfnfdmw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gbmxmcjvo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gntcxcwkk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gktpbmqyg.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gqcbpxcip.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gqrnsvens.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/guqmgatdx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/geufcgdue.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gmymeoqtd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gtyqkhtpw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/ghveayhyk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gbmpkjrxp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gmuxdfcqm.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gajanbstg.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gafvjanig.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gkderryga.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gwxfwqpfx.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gbmgacqlx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gihywoixy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gafcfwdew.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/ghomuipsf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gduognbhz.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gaklgqdhs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gkmfswlll.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/ggffwfzbs.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gqupgtgwm.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gsmnnkwud.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gqlujahqd.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gyrruejlg.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gncnbagom.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gsogtfkzw.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gymvjlyis.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gdsynovdu.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/geuwjjpyg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/guwjpycnt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gyywoymme.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gmcxtqhlq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gjrodbtcr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gqogfxymm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/givgzuwcq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gskieyrep.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gphcwwpbo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grebpegir.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gindmsenq.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gfvxrjgah.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gamhmbndj.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gcxhvzbmc.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gerlybuiv.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gkulssytb.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gthxcfjsc.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gcdhgmkas.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gfqsmiviq.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gdmawyahg.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gmikxkyyh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gbmctaxzy.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gqpmzmhke.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gjsggvnoy.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gghldtlys.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/ghuhymurq.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gkxjoanqn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gauzytnql.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gawvojsxu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gkgdevcgj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gkdbvegwo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/ghrftuylw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gyxwryrxq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gclbxukqy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gvbcxplou.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gxwueokeg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gptvmdiqi.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gzzafraup.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gmeqmgkhz.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gveuimdvs.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gudnusqgx.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gsnrxhjlz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gglhibbdk.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gylwukbkj.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gvkkzlcyu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gtjbvlfeq.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/guqwbwcmg.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gzyouyxbu.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/goksrsfep.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gjjjkhymo.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gvlqdistw.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gloenayud.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gvwbyipob.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/grijqbqrz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gsbccjvbx.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gwjkbjmrt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gzrkcqokx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/ggdnnxucy.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gobmccpgg.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gervuhqoe.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gqropcijx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gckcxibld.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gjwkgzrrk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gebzvujof.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/ggcighpge.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gazhdqpqb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/givoeofoc.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gsmmvmakt.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/glurmwfyi.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gcdgqwnyq.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/ggjoqpoho.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gbwemzxme.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gfgsfmjtr.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/giavbcrrr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gvuliikon.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gyguuptgy.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gqnrfopta.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gewitldgg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gyveheyvi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gwkyxqbvt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gensjcyma.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gfwfmprsi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzymtkubv.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gyuomfhqm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcrphdsiw.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gohzfqgls.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/ggejvjsjf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gumkoxtkm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/guapxhjnl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gylcgdmdu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gcmmlmwri.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gpsflbcih.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gughciahl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gnaausqhr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gjvaewtiv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/ghbxvdrcp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gnhytklwj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gbfrjlgpr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gopwrbcjg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/guliciewf.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/glyfdpdqf.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gnmzyflnp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/glhmvnlpp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gnvcerlyc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gnuceymjq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/grypixuia.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gpxtknmxj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gbjtepzga.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gsakagchb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gxekztcsj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gvzjsltrf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gjmzfvgss.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gvaqunuwy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfkpcqjkz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gmpmldvai.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gqcmdbrcn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/ggedhncrn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gqhoimrfc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gkaulaigm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gtcmsbwdp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gqzdfjngy.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/goeseodog.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gbmfmikwr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gqpeeeimb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gemdsfosx.sHtML


<!-- 参考信息 -->