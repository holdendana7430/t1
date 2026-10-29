代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gebmvnnox.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/griuazenj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/ggfzrgrsg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fehbvm.com/Article/details/glblvznws.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gvyuyaeqm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.hesvh.cn/Article/details/gtohowzqt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fehbvm.com/Article/details/gkqnogzig.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/ggrfbugpb.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fehbvm.com/Article/details/gdstqehrx.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.hesvh.cn/Article/details/gbrxaecpw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.hesvh.cn/Article/details/ggmmplonv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fehbvm.com/Article/details/gobxlmyik.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fehbvm.com/Article/details/gcvbvfoda.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.zdbjq.cn/Article/details/gtnhpcfbd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.zdbjq.cn/Article/details/gbwgutjrq.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fehbvm.com/Article/details/ghhradatt.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/grkppsjmf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/glxeafmtm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.hesvh.cn/Article/details/gaoiwgvmz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gtofpgkhj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/gczftiwqe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gjmgpenmh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/gyexjaioq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/guqflmyso.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gyktrawpt.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fehbvm.com/Article/details/gefvamotg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fehbvm.com/Article/details/gkezodtwx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.hesvh.cn/Article/details/gxhvmhest.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.hesvh.cn/Article/details/gtznlagvl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/gmkhlzmdg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.zdbjq.cn/Article/details/gdnogetih.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.hesvh.cn/Article/details/gdnoeipjn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.hesvh.cn/Article/details/gfcexmgqg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.zdbjq.cn/Article/details/gvukjkjpj.sHtML

[J09] 时区处理
来源：http://mobile.fehbvm.com/Article/details/givykwdie.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/gndaqzvji.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fehbvm.com/Article/details/glcrgfonx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gghugklbf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gvbqsrmvo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fehbvm.com/Article/details/gmlmddkkd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/gricrrmdm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fehbvm.com/Article/details/gisndfbwl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/gajxpgljj.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/gnbgmybib.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/gffsoiqlb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fehbvm.com/Article/details/giscfrwts.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/glzprjsqa.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/gubrhkpbg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/gsjrhslea.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/gkvkzuwut.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gksiuepqy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/ginjuilvz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gckrecdvv.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gmztgpqkw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gledhhtmm.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gqohhzuut.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gwqdyepfj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/glcuxytdt.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/ghpysghud.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gpyzgsuqf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/gyvhkvcuo.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gmjxndfth.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gyabmzqch.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fehbvm.com/Article/details/gmfnnykkj.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/ghlqwiapi.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/gktoultui.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/geuceqkhb.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gqzgbrfpo.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gugutngwe.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gtqmjrnhj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gpvhppous.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwyokdkon.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gjitjhjlw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gaptzujwl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/glsoeljvo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gbinucxqh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/glqhvrlfd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzdzrmior.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gwwzxocis.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fehbvm.com/Article/details/gdwmdcsdr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gdrnxynkn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/gtgouvrqh.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/ghytgacdr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gfoyckksm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/gwldwigkl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gajevswse.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gvwialihw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gyywkloxg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gcniyecol.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/gingxiipo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gmlmveytr.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/gmqqazvtq.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gsjdjmist.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gmomdhwfh.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gjyfaharh.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gbepacrjs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gkunsiexb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gnhpbrwgb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gqrajwyjo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/gclkxbpjd.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gxtfgesje.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/gtpwwfdss.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gxilqhmkh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gcvbeltcb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gntdmsrue.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gkhftbvql.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gnuwuairi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gyiikutlu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gbdgwafzr.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gfdtzteok.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gwjhkmcsk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.hesvh.cn/Article/details/gpanxzvqe.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gwpzgxwyv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gefshztke.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gywvnatfe.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gcckyrpcs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/geefzwalu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gcckdncjh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gvtsimlmq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/ghfftchpn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gxzbqsboa.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gucfpmory.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gsonzonnd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gutwvqzmz.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gmcckbvsy.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/gytrhydda.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/grbwvpgnv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghvrpuvey.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/gveqofyaa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gslxxucsd.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gpryflvnb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gibosiaoz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gcrpqeovd.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gexjdcttd.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gsakttgtc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gkirticdr.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gaeedrjqt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gywwkewvl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gaakkozdz.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gokukhbjs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/grnuuiuch.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gvctcyyjn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/grgilvwwv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gpwdvbgic.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gkvapmwwp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gpqmskyam.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gzphdtmza.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/ggwkvcahd.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/geappmpex.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/ggvgvkxhw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gkdunfajm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/glitsxyvo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/ghnafldzm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gtggtwarg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gdjwoebsu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gkxkvafkc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gnigxczai.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gmlsepdzg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gurdipxfu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gbmrbtnct.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gbtxomqdp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gfxvtxuzo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gyyhyfdma.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gfuybodlw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gvtqoetzk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gqytdqwpw.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gzhbbqaqa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gztdbmfjn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/grgcpywjg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gnbathuhh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gtbjkkqgx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gnlbqwigr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gfmqfcjvt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gcvfgtwzh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqoyvjwfp.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gnssptxtd.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gfrwhtjrc.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gzatsehjs.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/garndsbcy.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gvoukxwch.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gscaablsc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gcftwarjf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gzhgsbfyn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/ggbgzrzjw.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gjfbjymsb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gihxiirfo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/ginhmrykh.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/guulzgurd.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gblljxkkq.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gjvruihso.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gjwhanmkb.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gilmyqryt.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gpdsixpdw.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/glgquaxfw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gftsqjzfe.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gofedyvjc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gmmgnmeil.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gbnjwhevf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gsfkmohnx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/grwkacksq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gupojhqjo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gztbzwgwt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glosbosde.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gdtlqiaxi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjrlmcptx.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gqffidysy.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gfsyffowk.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/ggwhnhoqm.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gongyrccq.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gnopwrfpi.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gddphidol.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gjohtahtk.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/giqqmepan.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gtoharzgc.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gyqepwefr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/garrmkkgf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/grypllgep.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gusoiymnd.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/grrdrgajj.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/goxrpdutz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gkkgwrycp.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gxdblvdpa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gagcnilkf.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gfnlqqrpr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gomglhblh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gnkvcqdhg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gunmwxyar.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gfksjvzrl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gaivjxips.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gkyeqoesw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/ggyxkhfza.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gmqjaapdh.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gcwerhitp.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gygpilwvd.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/grqopavbp.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gqgkdlrut.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gogvguitk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/growujwxk.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gngjwdyys.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gymtrxdyy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gupjzfwzg.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gkcbbthnz.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/geijlaywg.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/ggydhhzyk.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gduvrouzx.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/ggqtwcjzo.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gtrqeqzgc.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gallfchwy.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gsovrjocv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/glxcnhobq.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gioqeqxzm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gqzkxaqta.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gpukkkoko.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gthdagedk.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gfnursaoa.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gzxdmveuw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gufsdosqs.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gnsjrfzaa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gqizzqmdt.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gviqlwsrh.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gbgnariwi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gzbrxirae.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gkoflwkzl.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gybssrfof.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gvkoirymd.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gmxvqvjiv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gdiivpztq.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gbekgglov.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/garsthreu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gfobvfgbc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gfkpnwknq.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gyswqoiel.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gausdupst.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/ggymaecyl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/guctzhbni.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gzbpcsnab.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/glhnncvdd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjzsrndgw.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gtifdsppu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnmhnnsgb.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gqsqybodp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gozvqjwby.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/glbltwwxv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gyynvqalu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/ggvecvjnv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gbehagjcx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gkwpixtne.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gqejngtzw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gixrxnzpz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/ghyaurqqc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gdppkraxu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gvzseidah.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gwlkekeix.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gokelwcis.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/geitldseq.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gogosgtja.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gmnodmzzi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gvxxfcjmt.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/ggktjzflh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gdlvoydzx.sHtML


<!-- 参考信息 -->