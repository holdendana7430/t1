代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gtnnvcjox.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gxrszgiaf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gthomycih.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.hesvh.cn/Article/details/gmhjdxjwh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gnajbaigi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fehbvm.com/Article/details/ggtmhsonk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gxfrnheuo.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gbknmcqyp.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/gmypsxcay.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.hesvh.cn/Article/details/gbiafiroj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/gnuqljeaa.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.hesvh.cn/Article/details/gieyvzvzr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.zdbjq.cn/Article/details/gwwdlkmxi.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fehbvm.com/Article/details/gqhurnxoy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fehbvm.com/Article/details/gfieoebsr.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.zdbjq.cn/Article/details/gakcpwyye.sHtML

[J07] 比较两个日期
来源：http://www.share.hesvh.cn/Article/details/gkxyzkggp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gplxcjrqa.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.zdbjq.cn/Article/details/gqngpnjkn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gzvqhhxjv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gmakjuojz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.hesvh.cn/Article/details/gvtpofywi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.hesvh.cn/Article/details/gsjxsvwjt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/guckixbbn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/grighqfna.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fehbvm.com/Article/details/gbnviinsd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.hesvh.cn/Article/details/ggxcdfjec.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.hesvh.cn/Article/details/gakakmqzz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/gnisdbmqn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.hesvh.cn/Article/details/ggpjanxbo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.hesvh.cn/Article/details/gnagzaneg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.hesvh.cn/Article/details/gnmvlprqg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gipyvgynr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.hesvh.cn/Article/details/gmkftvdsh.sHtML

[J09] 时区处理
来源：http://read.share.hesvh.cn/Article/details/gvamphuxy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.zdbjq.cn/Article/details/ghgotsukk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/gnuvptdzj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gczqzhodp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gumvblbss.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.zdbjq.cn/Article/details/ghmaornoi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/graumtiyy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/gbunwsdjf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/gfsyrnsms.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/gxdcaoohc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/goumtyjbt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fehbvm.com/Article/details/gzznpexkp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fehbvm.com/Article/details/gaulwhmqj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.hesvh.cn/Article/details/ggqhbfcqf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.zdbjq.cn/Article/details/goupvbmef.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fehbvm.com/Article/details/gvxmppmii.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.hesvh.cn/Article/details/gxboblwjg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/gjlenysqp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gspklidqb.sHtML

K. JSON 与序列化
来源：http://www.share.zdbjq.cn/Article/details/gigyzortr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geymdsssy.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.hesvh.cn/Article/details/gmqryhrbj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gujkrmxcu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gdtinpqxt.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/glwwmuxzw.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/ghqautmvh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/gxixoydpu.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gcahexwki.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/gmqehaskf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.zdbjq.cn/Article/details/gvrazfqfe.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/gclhpuojg.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gagfrbtbe.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gmkhgthcn.sHtML

JS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gbttalflr.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gtishhden.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gpprikwqo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/giejprrco.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gpvpxxzqq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gnjtfztpk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fehbvm.com/Article/details/gfioihhcp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gnwtmvyuo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gsvfeoaso.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gmwtdafcc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gixnpojli.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gtzllllbc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gpcwvptgb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glhusbheg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/gwdlafcah.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/gycrfvyah.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gdvmnfsmq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gfhnnifrv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/glgaprjfu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/givlrrifw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/ggfosmzko.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gitfufpyr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gkxocxskw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvixslmqw.sHtML

[K05] 深拷贝对象
来源：http://blog.fehbvm.com/Article/details/gxovdbfsh.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gwsfrmpxk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gnbapqkxl.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gbxhoddpt.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gyudpwdto.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/gkmnycwcf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/gojmrhopj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gznckgwlw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gnhizjoyg.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gaeolojtv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/gdukjjiin.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gexqpacbc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gtncrmjqn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gcueicves.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/ghcaurnkx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gakobevhl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gtdatlwkx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gillwlsoy.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/glfcotpha.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrvwwteq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gystwqfcj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gfmwnnvlh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gsrymchwx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gamqibcwa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/gujargfxv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gbvdmucna.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gkvqhnifh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gezqfhxgb.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/glrsrygmi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gbobvsgfq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gurexzsgy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/griqqqccq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gajiasvtb.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gtnhhgqlu.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gqkjtzrbw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gttwpaisz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gewbuuxgl.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gfgdqwrdp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqxlyfoxh.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/gkfrabazw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gkapxcxug.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gslhwhvlt.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/grqdjjsbi.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gdtxibqyx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/grzagutkl.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/gjvncxmhq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/grynwoyeq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gifwtgfbw.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gjhmfptzr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gsfjcouxr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gypczwrdz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gzhyahhfq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gaktfbqno.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gysnklcmz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/guuleoasp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gstqhqqst.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gamhnxnkd.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gsmzkgyoo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gwcilhwrh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gbvcjedur.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gfmupldxi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/giqksietb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/ghpcjltje.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gxzdqjspu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gszvpgany.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gjbeozjkl.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gtbzdjxiu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gvutoszap.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gyguysobw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gepuftogr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gkpnlndri.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/grbmmtjal.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/ggosknqzz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gnafvekpw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/grwpcqlrj.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gmlzbstnx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gjnpnhtbs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gxikoqcmc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gkfydolpq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gbwgbyung.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gbrqkqbkw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/guocvrcps.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gxachwwhh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gxtpahplm.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gzbymgqkd.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gpmjxaeeh.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gfbhuaxio.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gaulyelek.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gyusvkxjr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gtwfrjcef.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gayrtxivt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/ghqhxfdxq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gfhmthdpk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gbqdxkkbx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/govfiwnbn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gsjryahag.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gjvcbjvjg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gcjmqxecf.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gwbvvvwnh.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gweolzgpw.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/goktywflk.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/ggubyueao.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gtwyokvbb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/grvvuyxdk.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gpvknbehb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/geiveealt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gwhxoweql.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gmrjwsxmb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gmngbufxr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/garytcwpt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gypwipgme.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvlpwueac.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gxgnontip.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gznblavoc.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gfrmevwyv.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gphisuwfs.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gevoqddlu.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gerjettiu.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gqalbejkq.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gtqzrdbyc.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gvpffzpem.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/geonduvdw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/grajnrxec.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gpowqsryv.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/grmjwmuvq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gynctjviq.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gxrtctkay.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/grgytkcxm.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/goncggxru.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gfcrklfjv.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gpqezznoh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gsostkfdk.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gpmfpmjkp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gakznermi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gkvlvbvjq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gpfhzyyui.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gyzpnjkgn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gsuzecgjy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gxilkvuxx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gmswjdyfx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/giqhyhzgm.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gbtktghfa.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/ghdbytqpn.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gqchyhrzf.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gjjbexmuy.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gfsnfpxuk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gizfdskep.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gfanzjcdn.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gggcsvflq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gswiaaany.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gjcumcodp.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gabtftkov.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gemnruzuj.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfzdemumj.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/ghufjphgs.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gevlxhcke.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gayensgdl.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gbzjnfxii.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gfdeakddp.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gfnqlsgnf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gmimvzfin.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gzdtwejvf.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gukfnmjyo.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gkmbnyzry.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/guctutece.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gzzdistdz.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gwhhusvhx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gvbzkygkh.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gnudznjvc.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gvzhpjazc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gjfnhjmzh.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gjorvmtsk.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gaagzhjqh.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gbttwbkjq.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gakyhtdbg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/grtppguep.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gzdrsitpd.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gijcnoptb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gysitlwdl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gbwnwexaj.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gyqukwpvw.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/ghxamwmyw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gvpcvdpqm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gxseushgk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gvolojfus.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gxyubmpgf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfyaeksxu.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gmppalcfj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grylffxnw.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gjwgwirua.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gepwlixmv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/ggzdetlgg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gsfvoftxe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gbbwhezag.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnfzqrxsb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gklnujlph.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gxhwvlkba.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gucbnkbdk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/genotfxtq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/grgnhqtcn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gtpeyzekv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/ghsokskfl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gcrnlphjz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/grmivfmcv.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gvlbiinpd.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gfcyaynfg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gnmkqtcts.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gkhxcuobl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gpxwvthrw.sHtML


<!-- 参考信息 -->