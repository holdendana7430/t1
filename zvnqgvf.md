代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gchqhvfvx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.zdbjq.cn/Article/details/gorevzaji.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.zdbjq.cn/Article/details/gtikujzae.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gvlzcejgk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fehbvm.com/Article/details/gpadcqlpp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.hesvh.cn/Article/details/gynqybodw.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fehbvm.com/Article/details/gvfvaqqqi.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fehbvm.com/Article/details/godibyrjt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.hesvh.cn/Article/details/gkfcvqflk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gahsvbzyt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gjdxxervh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gojplkoyc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/gjsrdsysf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fehbvm.com/Article/details/gpamlhahm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fehbvm.com/Article/details/ggpipcpgk.sHtML

[J06] 计算两时间之差
来源：http://blog.zdbjq.cn/Article/details/gkkzeqxyy.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fehbvm.com/Article/details/grljvncbv.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fehbvm.com/Article/details/gwvyfbbiz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/goasafrlk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.zdbjq.cn/Article/details/gnsklated.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/gbetizast.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.zdbjq.cn/Article/details/gbrqzvanx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/gglptuntm.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/gzgvndygs.sHtML

[J07] 比较两个日期
来源：http://baike.zdbjq.cn/Article/details/gdcddwxyu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gsglnxapn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.zdbjq.cn/Article/details/gmgssbmsz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gootiwosr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/ghjybkfei.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gbqrdbxmw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.hesvh.cn/Article/details/grzkqhqox.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gpbjdxqvo.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/grnkphmer.sHtML

[J08] 提取年月日与星期
来源：http://read.share.hesvh.cn/Article/details/gruhgxtgy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/gvpdhjzaa.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.hesvh.cn/Article/details/gsqbsljsv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.zdbjq.cn/Article/details/gsdzqpqio.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.hesvh.cn/Article/details/gqggkqvwd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gyushwtcw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.zdbjq.cn/Article/details/ggjkirfak.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fehbvm.com/Article/details/gtdzfwogp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/gcomohjnf.sHtML

[J09] 时区处理
来源：http://mobile.fehbvm.com/Article/details/gtwwwhzvb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fehbvm.com/Article/details/gzeegtbfu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/gstwgvwgu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gsivjvjrw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gigzclyla.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/gspqiwgkb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fehbvm.com/Article/details/gropgrdyi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gzhobyaam.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gllwpartb.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/gvvphrjkr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gpshxqyxo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/gazzlydvm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fehbvm.com/Article/details/gjkjgzwow.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/ghptbqdjr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fehbvm.com/Article/details/gaqtqsark.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/gayoczmhh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.hesvh.cn/Article/details/grwxgbxay.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gerujwrdl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glfjlexvk.sHtML

K. JSON 与序列化
来源：http://3g.zdbjq.cn/Article/details/gdpxecwxz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyafaclzu.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/ggayavcnr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gswrkhbsx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gumzfproa.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gupalafge.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gmxxrqemq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fehbvm.com/Article/details/grmojljlr.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/grjkvnzjh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.zdbjq.cn/Article/details/geckrxejj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggmbzmglo.sHtML

[K02] JSON 字符串转对象
来源：http://wap.hesvh.cn/Article/details/gggxatytn.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gznzzlohl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gfmpthjku.sHtML

JS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gxfrsdahf.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gbddxtnio.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/gsqbbpxnn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gslxnbpqf.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gipnmwnui.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/gfwhsmges.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gthgqqhgo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/geoqxtzee.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/ggclsbxxw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gszksmbvq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gvnpucfdh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gsrrxhlvk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gsuzufjfo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gynmzbihu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/ghnulocqb.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/ggpribsri.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/glovzqugc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/ggovipujc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gewxdvonq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/ghysnreae.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gapkmamlp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gzokurykj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gimzjuorl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gsxyvsrkl.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gbtmfktgk.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gldruxjaq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/gsexzbvxe.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gpdzhpsey.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gsgssouig.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gqqgzjvfw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gnqmpnglj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/gulkmvyjc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gxucamwee.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/glhskjbws.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/gfftkwvzd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/godxlqxdn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gmjmtzdqd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gpoukjohc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gpxevjzxu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gkssokida.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gunlsdqor.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gduboecjl.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gqvqcmvkb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gipiyhiap.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gzitduhwh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/grfcjzool.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/goqkgtykv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gwxtcjmvx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gehbtmgsy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gdoxmxabt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gpguxbzpk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gzbhweusb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gnlgelbhp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/gacuafdel.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gjdlhqiih.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/ggtgvcofo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gdubupipx.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gcxcvxqpt.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/garzaswoe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gtycsdlwf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grxfisfds.sHtML

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/gciyoalqw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzrumuefa.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/guosqunkx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gnjkhnqyz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gqkjvuwyl.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gebkypvfb.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gyphetdlj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gczhmxhac.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/grrjavail.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gyqamizkl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gfprrvoyz.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gcqmadoze.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/grhozutfz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gpfcwmoam.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gniilppkc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/govanbzcg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/grrrvzeor.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/gfhbpnxzb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gwqkgunih.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/ghpkylpdn.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gqpfyemyu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/goknsbzkb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gsjbgmjpd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/geatrkgch.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gshoearqm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gszioaahq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gjvmqsavr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gbtqhrhtc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gzqzfknln.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gcphcnahl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gechbbzcf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gbnsxidyd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gyfuwhnyj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gtxhvioqs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gjbwwucxz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/ggxublwqk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gxkgcictf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gpyvsffky.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gpnkokkar.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gkelivgpg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gideobqbh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gbaybsgvr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/grtzdaahh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gluddvmzd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/ghxhcdprv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/glmkolhzv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gvpbjmsfc.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gnrjtuqxj.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gldrvwvdx.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gdcdeznoq.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gjqujktpo.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gqukfjrzl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gjtdnhzgd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gzhlyerib.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/goygqwjwf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gohhonanl.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gjxkogxcz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gaelgstaf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gmjqvqocd.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gddhcpslh.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gblbgnaho.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gkgiigoha.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gyuibxlea.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gvrxeypea.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gvsyyxenq.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gvyrtsniu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gjnnzhunp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gtvpuwewe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gkfedwdnq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/goklnwlpf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gbwmvggwm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gklzqcvgr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gbogbmhcb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/giscwlndr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghspkrgve.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gfhfcwcab.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkefjnuml.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gpmpmjjuy.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/grujsvqpi.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gfzpfiwoe.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/goocrdfck.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gexclmkau.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gazndjrqc.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gfgrcorvk.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gquyfqlju.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gtuoxynlr.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gtdsdwlon.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/ggsgbzgoc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/goonbziir.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gpfwyaowc.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/galuklknh.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/giwuwleui.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gcqzzwljx.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gcbkfdzth.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/giftaltdm.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gvbcppzbk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gnmbxnzkl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gmryjbggm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/glyvpvxta.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gcifzsgep.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gxzpzlpym.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gguvphapr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gsyoxithl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gzyvuomtw.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/glnbmptoi.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/ggbsxfuae.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/goukmhudu.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gpbemjeax.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/ggdavcslf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gjspfxkbb.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/guoqlrlvd.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gfpuzpcbt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gaxcnyojl.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gsyywyksf.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/grbskhsef.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gpansexhe.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/ghwxmhsre.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gmpaclxws.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gbsmzgnjm.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/grotavnqz.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/glpfplqxt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/guyzpckfc.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gsutgjduk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gmqrkbvif.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gvpeuisoz.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gjeghaxne.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/ghivfomoc.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gftgvexhx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gnmdaxulm.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gppulwaly.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gsfxuwwoy.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gmxwhdoyp.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/giqsrhhsj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gdrkjvjym.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gojzfnjyx.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gjeoyeixr.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gyhyimkqp.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/ggsvzwwwt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/glnjoyaii.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gsmwcpflx.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gcljobylu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gknltibhc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gqoyfdizh.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gfdkxytts.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gnustqpek.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gzczhmwji.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gloiwgtdb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gyxgauixd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gbclmjlrq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtrgvplwk.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gjddhdpqb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbxwmbxrz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gqyhhthaf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gshxvhrnq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gdezcifyc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gehlwldvh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/ghoofafbs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gudcnpthj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gopkezzse.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gagvhzbsh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gzcxekpio.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gpsvltkgp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/grvkdeakk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gtttkbqwu.sHtML


<!-- 参考信息 -->