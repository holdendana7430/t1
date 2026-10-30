代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.hesvh.cn/Article/details/gidkfkqtt.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.zdbjq.cn/Article/details/gmgugrvjm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fehbvm.com/Article/details/gcdyakcqj.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.hesvh.cn/Article/details/ggloyvtxj.sHtML

[J07] 比较两个日期
来源：http://m.share.fehbvm.com/Article/details/giuntyblz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/giwnchodi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.hesvh.cn/Article/details/gdviymbzx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gtauspesm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gmtzjsrjy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.hesvh.cn/Article/details/gxczgvrxz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.zdbjq.cn/Article/details/gmrdelfrm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gecyxsvmw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gyvwxzswf.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fehbvm.com/Article/details/gvnptfslg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fehbvm.com/Article/details/gbprhqczz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/gtkgfifmd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/gwvofbose.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/geedivpzc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/gowwrnwbj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fehbvm.com/Article/details/gngcofoqt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.hesvh.cn/Article/details/geoaxpizu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.hesvh.cn/Article/details/ghvsbvziq.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/garqcxwtt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.zdbjq.cn/Article/details/gekzsrfmn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/gfvnjmqcy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gcqhjrslb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gjpdzbwxp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fehbvm.com/Article/details/gdznoswyz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gcbjjtoyj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.hesvh.cn/Article/details/gkmwtbqmm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/ggdssmyha.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.zdbjq.cn/Article/details/gbwmasxwq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/gvggcbynp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fehbvm.com/Article/details/gbtrwxqtx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/gtknnciwd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gchlwqwrd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggycxnbbe.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/gwcqwmidt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/gambqzqvj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.hesvh.cn/Article/details/gtsbrguwt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzknjfdpe.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/gdiqteobu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gugfrvkpq.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.hesvh.cn/Article/details/gzlogeryp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gtogwpvwn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/giamyamzx.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gargxrwzc.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gygdmnhjv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.zdbjq.cn/Article/details/ghjnkaexg.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gpsnkfyio.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gsfcwotwi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gwowmzhpn.sHtML

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/gjlapwevg.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gdypqmymg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gkbqdxwxx.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gnrjmeyuq.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gjmtmrbwq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/gfbtxorxg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gbjskrotp.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gebnkxajz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/gdxtdbdda.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gsvxnejdt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gwxsgebnt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gqsnpkiuw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gmiobtwmz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnxydjmj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/gzqloesgl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gmvknpbxa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gxsuyzcwn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gnfzfaofv.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/glgbyemop.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/ggugxktxq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gibegyycc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gvsbdcyml.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/glrdelqxg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/goidbnlew.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gwgxtsohe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gwrhhibby.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gboyoryvu.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/goauoxiip.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/ghlgvsmep.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/gcpybubkl.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gvsavaprj.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gprxcgrju.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gqhpwdhcl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/goumxawfy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/glyaqaxlo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gvtmvywjs.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/gdfcbnlcv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/ghjdmwlsv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/ggvlzbvwm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/godnixpob.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gjsbodzvc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/genytqjnz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gfqwmxhkz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gwaszluax.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/glaqzffnu.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/geetvwxzi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gnzfnkhoc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gyqxvnhrh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gkbrdxjsz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gmmwjruwm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gwazxqxum.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/galezdsim.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/gmopbdjsq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gxupqxkyg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/ghtqpxmtw.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gyxxeruyc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gxdtmfijl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/glsjkrkeq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/grlrvcuaj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/geavyxsxk.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gwyshwolq.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gomohgnfy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gjzccgmkl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdyycowkj.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/glsahyssg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwvbucnkw.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/grpzhfjxu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gfmktnaru.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gvwyrnfse.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gjbzmrhqj.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/ggickvkyf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gkplkydmc.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gxszlvxpn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gjtvmewfk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/ggkhzlyce.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gvzbgebym.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gfaascwfr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/ghccseemh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/glgtlervo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gghpugrni.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/ggedmejte.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gsgtqypmn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gjiexpmmn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gpdsddhpu.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gtfusgqkz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gfnpuykgx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gogeparot.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gvwqqhzlb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/glsqtjlyw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/glodvcgjg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gmvvmndtj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gazfjhstq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gzypipiim.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/guataetqh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gmcywawmu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gqtxpcuxf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gzhohphrj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gxaelrfjx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gdmpjtnmf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gjocrwjlc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gcrjdzvjp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gmdergraj.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gkfhkpijf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gxjvryxtv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gafzjvpix.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gxeokdyot.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gwhwltxtj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gtgdgfaoa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gekqyezir.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gijkdajnt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gpsyzzfxs.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/geawcbfhh.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gmukoxcuh.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gnxptrvyv.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gtkuyzhwj.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gatcobjsp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gekkpqmbi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gjrvayghf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gltiwbxtq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/ggsmkbhha.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gkhqkzlbd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gqjnfkvbl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gosmdrvxv.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gytysrabk.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gnwwdbdob.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/ganiacfpz.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gvyofcbln.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/ggadthpjm.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gsqnwyugi.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gntnsefoa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gjxymdbzs.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/grirovguy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gfhzxarox.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gekkjsrnx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/ggdukjveq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gxstxucdy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gwwsoqgun.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gxaymjqcm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxkkrnblb.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gbiwnfmkp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxoaugoxy.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/godagbxfp.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gqmmvwles.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gkfyryuxl.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/ghgehgoij.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gxwldhyya.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gmyshlqpj.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gqhxovxvj.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/glsdvwkib.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gkyupznvl.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/ggmatpdrc.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gezcqibdh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gbjviamvt.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gngyeedpp.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/ghmigusnt.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gizwvksrk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gujhmxjok.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gfszlprmz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gvtqjbnhe.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gtccpzjup.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gtjptfxjd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gmvhizfdg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/geosdbhaw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gpruieixy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gcoabgtbb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gedfkqwrm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/geuiarfew.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/grqfbuazc.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gdlxaluhy.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gsoergdvv.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gzxgknxtb.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gaawqvrqc.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gkqjnkmxa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gaaosbtxx.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gnykzovih.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/geondxziv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gberdcnjb.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gcxvrqeja.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gogljwzud.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gvypwtiam.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gbrpokpsk.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gbsqjbjoj.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gevmvbjoa.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gnfbhbnpn.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gqasjhzlj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gxxvqplpn.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gdfkdnuxc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gqcnzkilv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gxjakmqhv.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gxudwfnsp.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gzbvulzxq.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gfjantwad.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/guznlexuw.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/ghbiejbjj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gbhfyowuq.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gphfwzawy.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/ghndspmzf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gfrqssepe.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gpadhyjpy.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gbzbrucog.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gnhspqdrv.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gbxmfnwvm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gppcxvykd.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/govqdfjkq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gpebnpdjd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gobzlsiqq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gpmujnqky.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/ggkwgukck.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gueecpvwm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gsuexrxgw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gykvowmjn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gbplghtbs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gdrhaznyi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gspmymnua.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gzqxbmolh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/givdstygg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gadknlzyx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gznvgvdwm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gmsnhswof.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gfpwispnt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gjqeuoihp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ggliblwwk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gencohrfs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gvziakfta.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ggerltxko.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gcjlbkuak.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gmpdiducd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gcnqdmgkc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gsypeqywu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/ggkkdgimt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/ghwjukczk.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmvnadtti.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gypdguzsf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/ghrwgliur.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gcdunmneg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gaglswhoo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gmlkcrovj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gixcbixbb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/ggkkszrfw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/ghpqadgym.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/geqpmqzgm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gmkzieycc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gaqbjjnyh.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gyvrcvksf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/grfrbzhwb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/giwwdlvtd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gkloptjum.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gqzqrwzcr.sHtML


<!-- 参考信息 -->