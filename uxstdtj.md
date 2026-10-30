代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.zdbjq.cn/Article/details/gucobftuh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fehbvm.com/Article/details/gjavozuas.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.hesvh.cn/Article/details/gfgtkhyoc.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fehbvm.com/Article/details/gfbdujnlw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.hesvh.cn/Article/details/gmxetuuhb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gspsebxar.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gcsxhbjvs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.zdbjq.cn/Article/details/grhxkpank.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.hesvh.cn/Article/details/gewritgba.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.hesvh.cn/Article/details/gsyrzyxfg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gobdzdmsk.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fehbvm.com/Article/details/gehwrtzao.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.zdbjq.cn/Article/details/glyfpidlj.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.zdbjq.cn/Article/details/gqnwkttpu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fehbvm.com/Article/details/gvqyiybdu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.zdbjq.cn/Article/details/gbluuherj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.zdbjq.cn/Article/details/gtwamjlbx.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fehbvm.com/Article/details/gyyuzthsi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fehbvm.com/Article/details/gnmpbtksw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.zdbjq.cn/Article/details/gltiavkti.sHtML

[J07] 比较两个日期
来源：http://mobile.hesvh.cn/Article/details/giiwfwzxk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/grjjvagrt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.hesvh.cn/Article/details/gdvzixfle.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gxrimbjtg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/gegbvvwsj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.hesvh.cn/Article/details/gdijwfdsp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fehbvm.com/Article/details/grklwrrrx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/goxaupxby.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gdeqlabrh.sHtML

[J08] 提取年月日与星期
来源：http://mobile.zdbjq.cn/Article/details/gcdcmckgl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/grdothsxh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fehbvm.com/Article/details/gtslcobhc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fehbvm.com/Article/details/gfhibrmyz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fehbvm.com/Article/details/gwnmsnbej.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gneukqiay.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fehbvm.com/Article/details/gxhciqwee.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.hesvh.cn/Article/details/givrvezed.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.hesvh.cn/Article/details/guvlciqgm.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gwydohily.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.hesvh.cn/Article/details/gcljntkju.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/gfyljkdiy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/ghcvmpobc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gzsvdzkfd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/goxdkyeek.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gjfelowha.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.hesvh.cn/Article/details/guepcwibt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.hesvh.cn/Article/details/grfhpaqjw.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gitvenxbb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.zdbjq.cn/Article/details/gtpwamjiv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/gbibqdarl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/gtvwadomk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.hesvh.cn/Article/details/grdbhyogf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtcgtcwrb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.hesvh.cn/Article/details/gbxggkytx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.hesvh.cn/Article/details/gpmgdsxsd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/gbaulzhue.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtkpthfwv.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/gswlwaggj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grdkqhqwi.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/gvjelerak.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gpttwhdlz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/guwzdeamv.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gshxcyizf.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gasrrkcsu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.hesvh.cn/Article/details/gsapnqpdc.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/gnizljxrx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/gtpchnaqd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.hesvh.cn/Article/details/ggykvrrbc.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/gzmtkijrt.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gvrlwzkvd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/glfzebemo.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/getywdsdy.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gbdtdbnbq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/gfmidjgqo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/graufezwc.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gabuqdcsi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/gdhbtudta.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gfivjewyd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gzctsxusn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gryxzgcvr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gaxkfbzzr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/giopmmfdd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.zdbjq.cn/Article/details/ggvxoyube.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/gkjvbgguw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gypjuxheb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/gypfkoowf.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/gjwgbadmp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gvsvxjjim.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gswymgpbm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gyznwufrt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gjjnmeyia.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gjvjexqhn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gnwrlaqab.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gyfpgkkfd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gqaokqqpg.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gugqylpqb.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/ghjybsukv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.hesvh.cn/Article/details/gvmmqgwoz.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gjsfxzwiq.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/glvhyeqsv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gowrizmgi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gcabphauo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/gwjbsjfeh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/gswomwjum.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/gbwrtnhvf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gubemuwko.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gkjdklhgg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gfhlmkwly.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gwdzvnodx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gmeqjhxox.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gusqvvnkn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gdlkdfdzq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gjbsekyrr.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gcmpkhhiv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gdqyniqri.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/ggpzxsevm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gevpkxiio.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gqtzazaiw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gofmtsiyk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gfadiynvc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gakgsqnzx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gourdinxq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/gcfznvolb.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/girzjhvii.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gfwktbors.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gnfzckqpj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gzatzayoe.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gqpsuffst.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gvvypcykx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/gmnbaenuq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/guazvxwnu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcprhlzei.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gmabsjrbh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkkihhest.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gjosqrhni.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gvdpxkzgd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gxguaqoia.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gtwjwvwux.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gtwraslnv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/gjfscedlw.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gezxwmajs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gcnzsbqgc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/gmkawdxxf.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gihojjlpi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gfeiaiuch.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gmlmpaibh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/glwciatxw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gftxxihoh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gnrnnlynq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/grcwmgqfi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gkdyqcytp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gryapbdwx.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gugvooply.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gyhgkptpr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gefzlgmfd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gzrlpqsoa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gglmodtre.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gbwkbwfoy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/ggzszghun.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gdygngybt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/grnfynqve.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gwgghccpv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gcgcnuocg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gggazydag.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gsvtoxbck.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gcwoszksz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gxrmotdqz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gbfuendjq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/ggknuyzxv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gbtlkhexu.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gdvulmsxv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gtbxftyoc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gzbypnmev.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gshgbgsdo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gzrxgplpp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gpkowrrhk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gqmnftdxv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/grnjagxuh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gqldmcmgv.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/glanlfakk.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gihcnszrj.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gdymfuiey.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gpzeamikq.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/glghclsuw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gczjhqbvy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gggrculgw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gcxrsgbdg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gcraxxynh.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gjeqhnwpa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gyljuwqcz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/geskubrys.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gajuykmkc.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gjmhxwtnv.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gjlrjzcmc.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gskvpisfr.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gfrsvizdp.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gfgfevfxw.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gatheywdc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gxmidknwd.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gajexnqbq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/guybzqmdm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gtzapjite.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gwkawlban.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gkvmtduhk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgxjtfzl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gkopahgtm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggkkaywtt.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gefwusmfl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzjmayekm.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gdgnyautf.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/ghovjnfzs.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gwtfyfoxu.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gvovallvq.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gqnyadfoc.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/glckalrdi.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gumgylcpc.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gbonttnad.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/ghtphofjf.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gnoprwekt.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gsvfxkanv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gwqnisnit.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/greuqpufm.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gxoastapd.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/ggsdvvdgq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gpgqjfigw.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gwzygwvdl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gxblupapl.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gvoamejgg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/ghlqmquoc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gsehpfurd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gwnmdewcn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/giangvtml.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gzpgnxmay.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gfmhhlojp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/glacuqchm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gkayvppyb.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gwpjixhnz.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gdanagzox.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gwourxvcz.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gxjqpbzyw.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gqcrhmubi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gyukxmavi.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/ghiinpaln.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gstqczuur.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gzajuvmfz.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gpmlrkpnq.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gtdwyisxd.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gekebdlzu.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ghjabmrjk.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gyztutmvr.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gcucthylp.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gkttvqyck.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gnwobuicn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gedhkicmr.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gellojssf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gbipuuwvv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/guynihmpi.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/govdsznyy.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gqbcdolig.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gnicigyyz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/ghqltaqjt.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gknckefql.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gynyskqtw.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gwziuwguc.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gtnqngduz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gmlxgltmt.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/grbzozqlk.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/grmdievqt.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gnszsoplc.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gljjpnsvk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gojjqmpvf.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/glricmldk.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/ghfqimimg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gtrnqhqsz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gjfyapbbn.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gfanfeicd.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gcfbzmgyr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gfoxifbwm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gvtfccbib.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gohzbwbgp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gsuufhrbv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnvnqvxnx.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gcadwuwsw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/getfetdep.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gbjuqeyzv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gjjnldxaq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gvoostcek.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gtxzemznx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gxbktxnxz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/grnfovedx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gvgvqrphy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gmygunbsh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gttetlkgb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gcayspghf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gwsncaemf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gpczzopoz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gobaoxmyg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gtpgvwbll.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gontcujae.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gwwkdiclh.sHtML


<!-- 参考信息 -->