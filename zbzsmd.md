代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2zitjtbwi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2ubxgwcdh.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2fjqqiadz.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2tegfsylx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ltafhqka.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2jejhmhpd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2qyoqynja.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2pasvnyln.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2cymtcwli.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2tsxsgobr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2npjjjavb.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2fvsutadw.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2iohejvyc.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ubnsnqbr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2cvajkmdc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2xvslaybc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2cumxkqni.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2psomniyv.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2qwywolhw.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2resfkfdu.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2rgpvvdkn.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2bkhnydld.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2pkgqblkz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ihqlgofd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2fwmbannv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2dqthzdyx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2auuevyqi.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2bwhbtnkw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2iviyrenc.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2uujgfqvg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2pisircrt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2dpjzigro.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2aqkjmrfy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2jophpgpu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2zgmtocdo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2jenfgwte.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2eseeislp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2buqqcaha.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2lebaapkr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2oijckdio.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2putvclwz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2xolldvia.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ftvmhkdj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2bckllbun.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2apyvvwjq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2lgapckpy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2pdysdmca.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2lpyudvuq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2xlnuntgb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2jytgtjah.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2vpsxusnp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nylbydbf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2spqbbaez.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2rvpeitrn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2oqahfkdd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2ydqdoqkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2togkoytm.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ebkonxcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbttzseh.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2izyumkfk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2cnwinsqq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2lphtclxy.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vadhonns.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hqghuujv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2mmsxvsxp.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nprojivh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2jemidmuc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2oeijoksv.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2vrmizygi.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2mvkvmeyn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2bhqkphdb.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uqqiwufz.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2nekaeuok.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wutjohse.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2owjinhyv.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dmrusdal.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2fogzrpsw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2utaseckt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2osvpqspk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2aandoqxi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2skulboyy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2utccsqye.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rjngkasd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2oagfglxw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jmalnlfk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2rierygah.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2eukryxuj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ouofpzsq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2bmakqfxb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2mauctxbx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xuchgwdc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zpspygys.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2luxyvwcr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lkixfitk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ajgpteix.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2wxueuqgd.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2emkouxyu.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2emvmxybz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lhsapksp.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lfhjlhxh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2aqyfnees.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2misaxefs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2melmprma.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ccqwqyrw.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ayejxyrg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2phiwajsg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2kzctpbjv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2rgteqecz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2skdxjxqj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2cbxngljb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2sbhjzixa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rgrnlgks.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ruvxjufy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2chnthrvj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ztcnhkva.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2dsvuwpec.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gbkgwyaz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2axswqyzd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xbhisack.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2mlkzuzmb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2yvzoersj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xckpizbh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2txweezom.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lcgalqrl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ijhejjld.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ssjmfwrx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2skzomgmm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2rfwqhovh.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ftbvycoj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2mpsifamk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jtdckroz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chvmlrvx.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2chgbznqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2auxtbtxg.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2iiasbmda.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2pgnjtsba.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2aqukingb.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tjackbfg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gtykxful.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ukydhtkd.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2ztkxwkqv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2mvgnfhmb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2psnaslvq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2appupkoy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ayirwlui.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2psqeehmx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rbnawica.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2cxrnghwc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tqslhxau.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ytpwznzo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2cwkrmbvi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zxrfrekf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2mkizyuxz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2hxumyhtk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aqcatadv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2lenpzfnv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2yekssgle.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ioebnucg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2dnkgmawm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2lcnxyecj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2faokulth.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2asjdkgcn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2zxvmenom.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qrtsuykn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2akecddya.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2akeixndi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vrlglrgw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2hzxhffyj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2kfhnoulr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nvgzlfoi.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2buvhkzef.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ncftrvnv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2etatvvrw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2sgvzwoln.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2yxfvwraw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2jobowqkf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2frutumqu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2fdbkthvl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2flyltidu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2rmykvngz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tpmmttyp.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2grrlftcs.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yzsukxyw.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wzgcjfdf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2eopzuhox.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ijycmrog.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ijlttzqk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2kwiarvok.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2uvqbfmou.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ujvacodz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qehwwkqi.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jwclrgox.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2txhtznjo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2wfdspofc.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2koirhjxn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ugxsxrhy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qrtplmis.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ahfpbdof.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2tnzsqyrh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2kfhvjjqs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gkcacjkz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rnftdfno.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2bkvndgrp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2jmykdxmj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tkeeaztr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2endqqhbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2giowikrs.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2fyxnpatt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xcmruegg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qrphouhy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ipehvolu.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2vnslukrr.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2krqsnbap.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ldjmbyhl.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ghkffrjs.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qiohjqvs.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2fkvhumxl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2woeqqofe.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vepavtqi.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gajjzfvm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jigwufbd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2aknqkzdu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jxtoapcf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2sxpdcrzr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2sjbackjf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2hhlmnhpc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2iiqcjmxf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2bswmwrzh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2phrmaelr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zpwtwpop.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ribbyqqu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zkdeiuov.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2tlamqfoy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2lyhhdert.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ilhkcxja.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2asexrmzy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2fluhzpuc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2zqhnynkn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2mgbynhsa.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jpwziypf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rreziszv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2raokatbd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xcdxhooa.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jiraellz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2wxwkcthx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2mlktuzjd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfmbcnak.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fvboygld.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2achgpaxj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2idqwcvia.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2amqencwi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2flfbzlra.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2jflnairq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2lyhzkzst.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2makcrvfi.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2raloopam.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qzbtqzqz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2iepurvsp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ssblqllc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ptvjduzv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2kqstsaka.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2zknxbnkj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2meqyadih.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2phhljxaf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2mrcbkzxg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2kpuiygcf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rewlnans.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nncljmzf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lnbeetjf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2nrluqjof.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2beybrbfa.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cmlxbxfb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2tpmwmxui.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2fkvpjguj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2mkpqbiqk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ghxuugap.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ruxjimsg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2lsbwntzn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2yhxudnst.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2echisarb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2zuxzlqud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2buknmyyv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zrghbhlw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfoujcpy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kbwoyfwy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cqgpafrm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fhrzsnxl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wppnwhkq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2edujoscl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ctrmcejr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mbeafpgm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2lruieaxd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sjdbciop.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2qnbnslgi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rcjmczlm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2viuukzqr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mzywcsjt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gubakwvw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2anrjthfb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2necawtzq.html


<!-- 参考信息 -->