代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gwpklkmso.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fehbvm.com/Article/details/gnnzeabhs.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/gfzujdatp.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.zdbjq.cn/Article/details/gaccojjoz.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/gxlobebli.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gollrpwaj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fehbvm.com/Article/details/gmmuesaac.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gqecriftq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/gpitassjj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fehbvm.com/Article/details/gpohtcyno.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.hesvh.cn/Article/details/ggqxojeoo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gvywgnhgb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gsvapxnvd.sHtML

[J08] 提取年月日与星期
来源：http://blog.fehbvm.com/Article/details/gautwxccp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fehbvm.com/Article/details/gstzgnftr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/gwtziiwfl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.zdbjq.cn/Article/details/gxecmjhgk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gotisqviu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.zdbjq.cn/Article/details/gatdihqnh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.hesvh.cn/Article/details/gqocuzxpb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gpzydjgqs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.hesvh.cn/Article/details/geamhxprf.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/gbtzdtvvw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.zdbjq.cn/Article/details/guurriwqp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.hesvh.cn/Article/details/gyyaojojc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/glduhuhht.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gffahavbr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/gxzpsoaqp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/gccaijnaw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/govjrqptk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/grfeqpcmw.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.hesvh.cn/Article/details/gyupzwdxz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/gxsmosktt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/gdkphrggw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fehbvm.com/Article/details/gqhflsejh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/gsmajolcx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/gagpyntrw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gmainktrb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fehbvm.com/Article/details/ghhhcntmy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.zdbjq.cn/Article/details/ggdpvvguk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goqmmzmgz.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gqhurhogi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grxvazuhp.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/gcmpuxitx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gbihlklzd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/ghnabpzxz.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gawqelldl.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gcffjuovs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/giytdvglg.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.hesvh.cn/Article/details/gozwlyclq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gkkexeebt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gvntfwmdc.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.zdbjq.cn/Article/details/ghrjburhm.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gmvgsjili.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gjayanvjx.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gigjgnnzq.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gtsktfumm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fehbvm.com/Article/details/goxjpxyqa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gtlhejqhs.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glonjaxox.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gfowkffwv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gltfrpvek.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gigictjrc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gwejprrra.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/giwdvxzrh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gphyobvvy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/gkgrxexkh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/gspkhijyl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.hesvh.cn/Article/details/geahnvwbp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/gesmroffq.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/glgtidpnc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gposgpdgm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/gpcggjfjx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gcskfnaat.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gxxdmlpmm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gfjbiqwsf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gpwizognx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gtyteglzn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gfmzkitgs.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gpuluxbjg.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/gqonhxohd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gkgfdgxkw.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/grkkgqtlp.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gzwnprybc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gdyonczre.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/gdvjjsgav.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gunnmtqkv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/gceuimkjw.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gypcalvbp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gitybuxpg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gjhgnsnwf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gdybqcwbx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/grnzprxkg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gzukhdfni.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gjojtahez.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gyloswvkd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gmmeayhrm.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gnkntsdmj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gqwcgpaiv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gucawdjgz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gacaksheg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gdxtyperz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gvwbcrhpb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/ggrahdyuc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/ggdqgjxmj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gffopwmdl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gumqdulsl.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gpxtauruf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gjhkzzxpj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/goqfdfnmx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gzwxrrgcx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gtwiqxrvm.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/glwdecxoa.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/gfmrapdbf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gjeuyizpw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gslirdmrz.sHtML

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/gtyupujdd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpbsncxia.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/glcmvfjwm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gmpoxuzmh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gfjslqpin.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gborfsvho.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gzhmtnxwn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gqnfrcplc.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gaggjpswv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gjmfdtksk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gillxliqx.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gkjtrasyf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gdglbegkl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gddyghtru.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gswzuswru.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gtxhkzgbe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gguxwemif.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/golqiwhaz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gbngwvwio.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gpircyyxa.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gxrssvxhn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gdxlhpwxl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gbmgodltq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gkxgivooa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gzkgjzqlf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/grhmksvzt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gtgfxvvbh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gsbkjjfvz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gsfjftewb.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gbudcfrhp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/glrooowda.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gstjbppvq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gbiinkqdg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gfmsftwdc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gqftszogf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/glguihjsj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gvalgecce.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gjlmutdsx.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/grxuguqgr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gsazyfgpw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gxyljikhe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gggotnevv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/ghcabpeoh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/ggejofnsu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gbiqjlvfy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gjqykkuvn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/goixkncvb.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gjkewpgyh.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gnverkvlg.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gczaxjfwm.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gsmcxepmu.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/geavqzjat.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gaqcoipgt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgoetjgb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/giookfbuz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gbxxklfaq.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gdejzgpet.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gjdecymwy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gwewvllfr.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gofoapkpl.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gmqkkjnmz.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/godklhhfl.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gmwlaihtx.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gyjvnorcj.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/ghoyuknea.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gytkzepap.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/geadwhxzj.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gptjyymez.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gtsdnyphy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gkemsxaed.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gyvwwvmkn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gvcnielzb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gqnpfohpc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gbktuahjf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzdvejoao.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gwyoigysl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjmtlgosh.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/grzewimlz.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/grhakawjc.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/guyybvuxb.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/ggpbqqppn.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gvjspurfl.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gwqwzimwa.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gkhlpxmvn.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gwlcpwmvc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/ghiggksiw.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gziixhzoi.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/guetrgvby.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/grqkefxsw.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gihvxfcsf.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gxvdlijau.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gregeweot.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gepkherrk.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gnustdbwp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gxeeqqiuf.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gyfijdqto.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gyqbrwzbl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gxvfsdyst.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gzkhszhpp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/ghzupkslx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gtilhvsld.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gtoozxrir.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gfzbdwwtm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gjumbcqlx.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gquqyrayx.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gowhiodey.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gwvppsxxx.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gotatsfqv.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gcxhjpzqa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gladjmppe.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gmvwvrmtt.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/guxizzcng.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gzauztdjt.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gmggjkslj.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcdkwgwqf.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gdvsthyol.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/geoqgceuo.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/geftzdsxn.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/glnhpxsnb.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/glzmkzusx.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gfhctgmmf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gnzkhdaly.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gybnhvcaf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/glpgzoqxz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/ghjmguflt.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gbfsbebto.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gfniosmsd.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gtuzovozz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gwrtsavlm.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gngkdjiit.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/grinmrtqt.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gnvkvfkoi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/ghhqnvrxs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gifsntamf.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gktixpexp.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gekuqubiz.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gmiyamxoy.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gggssbryi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/ghoepfsuv.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gvzucltha.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gsygypqgl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gprwtkyrd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/giczaxgys.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/ghrmutekb.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gazxjflaa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gcpgckdvr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gkhgmwxft.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gpndzcfze.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gcrvsfyuu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjyyrqohh.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gwgryumuk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmvcjspwa.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gzrwnvpwc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ghamtwxmr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gemdnzvii.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gwkcuobou.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gxmjcqehb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ggpdhfoev.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/ggtdhclvs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gwwughbav.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/glztymryd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/glchdiicx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/getsditxb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gqydocyct.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gpsornriu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/ghipmqqkp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gceqdcbcs.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gzgvaiigc.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gmxfwvpqw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gpqpirwnq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gmaehrbnl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gxulwapwl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gukdplnae.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gzwtrfejo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gqkxcryyp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gcccosxlf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gsppakgym.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gntwbyoik.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/ggauinajt.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gpqapemlp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gutirjrot.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gmqzexsfy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gtbgjjahr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gfiozjqqg.sHtML


<!-- 参考信息 -->