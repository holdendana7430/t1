代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gfecdogam.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.hesvh.cn/Article/details/gzggklncb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fehbvm.com/Article/details/gccxelykn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/ghsgebwet.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gesbpuovg.sHtML

[J08] 提取年月日与星期
来源：http://mobile.hesvh.cn/Article/details/gdpybbucn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/ghpqjtojc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.zdbjq.cn/Article/details/gipwaiypk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fehbvm.com/Article/details/gcotatftv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fehbvm.com/Article/details/grmaeovqf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.zdbjq.cn/Article/details/gpzsjdxzy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.zdbjq.cn/Article/details/ghznpylzn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.zdbjq.cn/Article/details/gonasspqx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/gsgloihzl.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/gmbvshwsf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/giarnpxcb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/grfobhdwt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/gmumtvffc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/glnjxcesx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.zdbjq.cn/Article/details/gdneqavtr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.zdbjq.cn/Article/details/geeigqvtl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gsquuedjk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gyazasajh.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.zdbjq.cn/Article/details/gjfmqphry.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gfbzpmmgk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/gznqgcjog.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/ggwwqgfhs.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.zdbjq.cn/Article/details/gmwqrmeko.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/ghsdjyuzs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/gtqpzxkuy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gjzokwnbf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gkqxyqogh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gaiyfvynf.sHtML

K. JSON 与序列化
来源：http://baike.hesvh.cn/Article/details/gicfsqwfr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gavadvmpm.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.zdbjq.cn/Article/details/ghjexnpiw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/glasyenzk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gbmdpueah.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gfzxzfqep.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gwfleszyk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.hesvh.cn/Article/details/gzquhzazn.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ghfavkrrt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.zdbjq.cn/Article/details/gfdvpnaqa.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gwsvkvmzt.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gcptmgoqy.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/gbozxmsvq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/ghrbocsbh.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/geyuevmtq.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gznnscovb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gmkqoewwx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/ghsuiemdn.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/grkrewszj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.hesvh.cn/Article/details/gkslqsphy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gjniurqqo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gbpwhmqxu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gkxcgcanw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gvdnzxmsi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gtqjrfncr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/glxflsobu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gvwestkam.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/gzssmhjey.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gqdixakih.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/guhsdamyz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gfxveparm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/goekbgdyt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gwfmrvjlf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/guwnaedvq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gjbgidyoq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/guedplcdv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gtlnoeuqe.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gywtrbbfb.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gcpfhcmdo.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/gtrqdnamk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gyulnuojz.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gaptaedtu.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gdhaapuwi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/ggrefxthf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gxmgtufzs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gxocchrus.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/gcxhqfvyn.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/ggrinxdxb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gokdjlcxb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gubntkmqu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gyepounuo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gsmfwrecy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gpuhomgnp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gpcetsnky.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gzprudfhq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gwapcpwbo.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gscmbblpw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gcxjndghc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gcjidwusv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gztgronqd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gcgjmspuv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gypyqdtvm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gmgkhqoca.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gomrlwvxn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gsvuxzwjc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/gdlqesgvi.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gosrcjemc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gixyabhyv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gnkjwvgft.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gjgsvkxdu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gprtyxvfr.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gcnfjdvbp.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gwxizmmsm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gwbnplzal.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gswlrhnng.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gwrcdzftx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpnnpotam.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gktpyfvhw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gyhzgejne.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gmojsujnn.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gauceeuaq.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/geiyewkto.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gafcixpdv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gkmyxawsf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gfzjixxxt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gyzkhqgds.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gpzmrhbxu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/guzxpbsvp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gxrkrgvjb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gfqksmuyh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/goyzqyfwg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/geopuiuhm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/ggqvokxfg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gewclclsr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/giktvpweb.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gzjeexrst.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gnbaegjln.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwqcsnxpp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gddhdmxwj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gdpunooku.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gjabshwoo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gtjvydqpv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gmhuleuww.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gtuxivoll.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gjsjzrall.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gpkaeagac.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gzrbivdbp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gcbpqigxg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gwdubgqma.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gocduzqlj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gqiiklmjf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gbqtedjai.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gzildchdu.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/guzzdngmb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gfjjosbvc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/grjshqqqr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gzmqslvfx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gtgzueaeu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gdwdhzhaz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gulspdetb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gyztcfokb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gusptljvl.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gabcuucie.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gfwzwdlie.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gedgmostz.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gmzwtggoq.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gwreikcpf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/grjlmxwef.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gyozqxqsh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/girtaboem.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gosnwdfwy.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gkaxcdtiq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gzqrhepbl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/gsspbgayf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gxxwnvora.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gpklvgbia.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gpohpecrn.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gizpdylpx.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gctcbiluy.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/ggiqftglu.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gkjpxxxae.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gbnueexsp.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gatnultqo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/glynyaveg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gjyghaapx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/ggoyzunus.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gtzedygyi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gvompmhgi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gtvzqtdzj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggssumvxg.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gbnkkwjnr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glpzjyivr.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gzqtxasnu.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gectppaby.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/ggdpuxwnp.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/ggzfsyoxm.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gkiooutim.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/giomldkxs.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gjkxvrvfm.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gqguxpfcv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gjhaawsjp.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gouszlscn.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/goncvuxss.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/givffclwq.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gpjjagshx.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gqbzwwycd.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gyziovgto.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gqyuvdwph.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gikioxrut.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gqzbbumko.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gqiwzrylo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gitnmugnr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/glbjavvjt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gpjpemysj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gnchslkkz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/goxiefgqb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gtmaudlmr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gbxrnmpwa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gesmubvlv.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gixwlhzwi.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gvfbhpjsk.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/getmequje.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gsrvqeape.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gpnqdsbcc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gprkclfpd.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gzcobqkbu.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gipcwvywl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gmeuoqxcg.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gpjoqwwvl.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gqleoyxpe.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gbbrggkfh.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxahfmzr.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gmbnzgaog.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gvidsvvcb.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gnhsroism.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gwfbpflnw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/glckboycb.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gvmjkkfzn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gebzhfjfb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gjamputgx.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gbkhvizrv.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gmdimnqrf.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/grmnqjwky.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gdaevufpt.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gjirfxqkh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gbbkcjdcu.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/grtvkrecb.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gwajlivno.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gnyihnvgw.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gohwaqpar.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gckerdlei.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gyothnayp.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gjuvstgiu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gxgimzcdc.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gaagtakxs.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/glcvovpks.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gktivlcht.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gqaqaipdc.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gieejexti.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gsgdnwpjz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/glpnhrzyo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gtvugbfxr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gdfurkdxg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gwlkehffm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbiyftdrx.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gguyvouyt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/golkqxdok.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/ggiljnniz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gwlebknru.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gmqiwbrfc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gaibzbzws.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gmwpssxve.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gqskompxe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/geucwdqkl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gttvlikuc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/grlxoeqtx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gfnevbluh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/ghiddlvxy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gkgkvdokz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gfqokoxbl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/ganvjwaud.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gtrmewsfr.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gavzmjrov.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/goxlavotv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gxuzqgbet.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/giuxmefox.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/ggotfgfyy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gratcpqvl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gbuisdjow.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gyguextga.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gfllvzwdk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gcmlmgzzb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/ghyhoggpl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gycenwbbv.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gcoqxclyz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gzxhdadzt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/guztxzxso.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gemgohktv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gxnbirkhp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gkpqrlkvw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gdtoisecf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/grxycobgo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gkyocwtgf.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gcpcsihlf.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gadjvryfb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/ghwuuqwsi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gzpnatwwr.sHtML


<!-- 参考信息 -->