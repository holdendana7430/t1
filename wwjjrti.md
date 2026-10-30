代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fehbvm.com/Article/details/grzohdxvq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fehbvm.com/Article/details/gmbmpuahc.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/gnwawnssd.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.hesvh.cn/Article/details/gpttloylq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.hesvh.cn/Article/details/gsrinltsh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gezhgehvg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/guqahsmpg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/ghvxiktzs.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.hesvh.cn/Article/details/gczlmkvrg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/gkmbdkovi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.zdbjq.cn/Article/details/gjbtmdwuf.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fehbvm.com/Article/details/gnvnsptus.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fehbvm.com/Article/details/gknkficwb.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/gkebmlnah.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.zdbjq.cn/Article/details/gqzojiemb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fehbvm.com/Article/details/gzxplgysx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.zdbjq.cn/Article/details/greuvvbam.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.hesvh.cn/Article/details/gvybiuobs.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.zdbjq.cn/Article/details/gtczvcjfn.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.hesvh.cn/Article/details/gmaaqagfd.sHtML

[J07] 比较两个日期
来源：http://www.blog.hesvh.cn/Article/details/gkzlwfxoy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gzwhidqap.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fehbvm.com/Article/details/gsooxpvjx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gzhurkrtv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gehicdxwg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/glewjoyai.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fehbvm.com/Article/details/grrmwpzie.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/ghdpoicsd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gsvbcnyis.sHtML

[J08] 提取年月日与星期
来源：http://www.share.hesvh.cn/Article/details/gblfqnsnk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.hesvh.cn/Article/details/gakjifdgi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.hesvh.cn/Article/details/ghuellswb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/glguobisi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.zdbjq.cn/Article/details/gxryhobcg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gpnioqzub.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.zdbjq.cn/Article/details/gipgktufr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gsunhxdbn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/gzfcisweo.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/gudcbtlvi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fehbvm.com/Article/details/gbapgfaqi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.hesvh.cn/Article/details/gvnzkpthq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/grentagif.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gssscwlpl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/gbvirfdhs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gufflgwwx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.zdbjq.cn/Article/details/gdcxqqilt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/gddljbuvr.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/geefusbww.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.zdbjq.cn/Article/details/gvtjnvxgj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gqfluakzq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/gbjtksdnq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gsuvbtcms.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fehbvm.com/Article/details/goqihlxfv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.zdbjq.cn/Article/details/gfysrnscd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/gutadhibs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/ggferygsv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghwuuiovc.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gjtujnren.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmnbdfosz.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gzdewgplq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gfcdevoap.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gezwfmvjx.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/giowrhjej.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gropbtnxn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gvasznlau.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gtpjuzlur.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/gypyorpdn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gicdanhjt.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/ggalkcbpv.sHtML

Py:   json.loads(s)
来源：http://blog.zdbjq.cn/Article/details/gtxqnugdd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gyolmhfko.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gpcmtsxmj.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjqenzocl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gegquaxoh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gfoawmnhm.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpjirzhls.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/ggjusqilq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gyiyyxgxl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/ghexcmpwg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gnepvazro.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/glicpulgm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/ghesohcie.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gqiiosfqg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/glhmevkpi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/gjmxmlrtk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gawpkynbj.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gxwvzyazd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gmouvqfjf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gfaaggpyz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gajevkkqw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gqbqnbocx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/grttlluvp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gpwpdcrmt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gwmfviskq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gkhomjusi.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gtehxteud.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.zdbjq.cn/Article/details/gbypqaajb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/ginzhhech.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/ghwxzmpfq.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gyzlvscct.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/gpsfxmucr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gcymqtgdl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gududselo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/gojqpxfdh.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/grswgdixh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gffczfuiy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gdnftuubj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gzsamnsxc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gwsjwffsu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/grtexepdq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/ghyrwsvrh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gvxwcxfms.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gmhqhpfnn.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gjxrfbwpy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gmrvkkstp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/gtcozvadi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gfbrchaac.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gxudigtyo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gzfslvron.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/grhwqmmwf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gshjdntvm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gycjmopku.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gqrqdbkvf.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/gykmqowns.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gimxbxqbd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gtysayimy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/grbjrdcyj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gymawykim.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gkxodsjsg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gmjxxfbtm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/ghlwflkst.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ginejpklp.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gmmkszxcg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqdyvczlb.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gpxomrtak.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/gkywwhdwl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/gtzazphif.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gztgnzium.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gqoqsgnrq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/grnskeikh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/ggkmmfuaj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gedsbyeog.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gmlqucwzu.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gcgdweadz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gnpgvojrk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gbuzkysqi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gxthmxntw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gtxmwqgcm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gmobywxdz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/ghwmuubeu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/giydomuie.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gleyixwjh.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gamiythut.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/glkynivhb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gcrliedga.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gthuayvtq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gzqakewaz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/guhbptwep.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gwgtuljog.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gzfbppgue.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gohiutqbz.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gipkrthbm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gcgnxxjeo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gctopkaar.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gkyvudpqy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gplgpyaqa.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/ggfwwaubz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gfatydzwg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gvbikkjft.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gdojdawxu.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gfrhfbwzc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gqxmgadia.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gnfeceodi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gzmtpbqho.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gchlfdhiv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/goluswxwt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gylsxfddg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gqheimajp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/garntxptx.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gyxmsnvwz.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gnnfwhjxi.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gdugcyrgj.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gerigjewp.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gfqlbueup.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gxzmavnss.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/geixqayxm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gmhyfsdws.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gxgngyaoy.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gtioersqt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gtvmquyzd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/guzryarfu.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gzipekonv.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gpeaxkopp.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gddgwwuah.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gicfaysff.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gqmsrmzsy.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/ghxwzbexk.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gpaiayimr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gliygkntf.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gjwkbpszk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/grnpafrcs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gycgdwelt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gctkebubw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gnigortic.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gpxxxemdp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gspgeevqe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghzrbhghk.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gkicabaxa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbqiejmka.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gpzhlwknt.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/geuqxxply.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gcblupwsh.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/glukxaggb.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gzcbwfjcm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gdiivhosl.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gkfxohwlz.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gxhgyefmr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/ghjdhqpyl.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/grmaypodl.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gwzakwznc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gjekkkmad.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gxucomoau.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gzusxpacy.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gdflqduio.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gqtpicknk.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gtelvaxqy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/geqzmalhn.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gloqosjac.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gefxigzga.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gifsmoudl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gjkpartjj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/glenostcm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gkayklvgj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gofcygfww.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gzkramdck.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gxksuugfy.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gdunvluqc.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gvmbulpph.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gltvvdoan.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/goofamfcs.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gprxnuega.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gcrxtdpqe.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gnvmfxoro.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gilgwbfau.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gyukgvhjm.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gimiwvyks.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gjosoozkn.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/ganbdwjuc.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gupaduovt.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gvorovnxn.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gjkwfdrpb.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/ggrabehml.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gmradjkrr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gkgemwjma.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/giazrqoei.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/grzaqzppu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gulppqnpo.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gjwimykds.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gedvnwjsp.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gsqmpubxa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/ggjrgdryj.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gsazpsfct.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/guqcftxxx.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/grryiffap.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gyywabgcq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gsdkzpsco.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/ghngfzzsu.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/ggqxzeqcw.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gopnztmnj.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gckgxcvim.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gkrqiossc.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gwsakmgrz.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gsfusirqn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gesevjfiw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gpezcvfnr.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/glmikdqfd.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gdjprpspa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gegsbnzjo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gjkbjknie.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gwahskbny.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gtynqdqjl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggxdxjppy.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gzihyofyt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glzhczfho.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gegoekbow.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gcehjtekp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gbfbseudq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gmymfoozg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gubktjjpd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gslufsmjv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/ghbietusa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gygrpkwru.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gfwiuhyky.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gdmpfhsqm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gmyqphycv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gzrgqigbi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gssuqxcam.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gtobnkkfz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gxbkeqgbr.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gixrtmxdk.sHtML


<!-- 参考信息 -->