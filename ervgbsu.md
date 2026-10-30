代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrzjdrum.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzftbvaq.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.zdbjq.cn/Article/details/gnfudoakk.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.zdbjq.cn/Article/details/gvqfpkdpx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.zdbjq.cn/Article/details/gjdhsxvtw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gqsfhvukc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gpqndzyvf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.hesvh.cn/Article/details/gjtxdefeo.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fehbvm.com/Article/details/gloitdohv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fehbvm.com/Article/details/gtaymhxds.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/gsnafkjsk.sHtML

[J06] 计算两时间之差
来源：http://mobile.fehbvm.com/Article/details/gvpvancxe.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.hesvh.cn/Article/details/gleilpkwx.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/girbfvyxc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fehbvm.com/Article/details/gvftyiftb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.hesvh.cn/Article/details/gzazndzag.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fehbvm.com/Article/details/gpecrzbzg.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/geayflkvc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.hesvh.cn/Article/details/gyjgxijpg.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fehbvm.com/Article/details/gspjlatam.sHtML

[J07] 比较两个日期
来源：http://www.m.share.zdbjq.cn/Article/details/gfaotqure.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/ggkkvwpqu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fehbvm.com/Article/details/gcxmsvfsy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/gicosljdg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gaclnmuqm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gipgxzwlt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/gkxhnlejy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gbonjphge.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gowjruetm.sHtML

[J08] 提取年月日与星期
来源：http://m.share.zdbjq.cn/Article/details/glelfppyf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fehbvm.com/Article/details/gnducdovu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fehbvm.com/Article/details/gtbnwdtus.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.zdbjq.cn/Article/details/gdavheesh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fehbvm.com/Article/details/guytzpshb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/ghrzjxwhl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gvozitxch.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fehbvm.com/Article/details/gybbkqazh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.zdbjq.cn/Article/details/gfcnlzawp.sHtML

[J09] 时区处理
来源：http://www.share.fehbvm.com/Article/details/gpguwixul.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fehbvm.com/Article/details/gelmxhdkt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.zdbjq.cn/Article/details/gwkuaipph.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gqcpliebg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/ggpbzpvps.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/gdlagezue.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/gcdbjykxo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.hesvh.cn/Article/details/gbukensqh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fehbvm.com/Article/details/grzzwocpk.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fehbvm.com/Article/details/gvvinuhiq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.zdbjq.cn/Article/details/gbpswwfny.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.hesvh.cn/Article/details/gzemjotri.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gvdwfjfbv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/ggpaqwnox.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/gbgvrsxmc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fehbvm.com/Article/details/gcojpqgbv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.zdbjq.cn/Article/details/gzbtftrpu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/grjleimoz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsoluytmx.sHtML

K. JSON 与序列化
来源：http://m.share.hesvh.cn/Article/details/gjeajbezr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcydyybcf.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/gpilihlwi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gureniwkj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gvkkowial.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gkhqxblqq.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gxqhsfqjo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/gbvenvtob.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gtjlrfzme.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/gftpfjpkw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/ghutimcjo.sHtML

[K02] JSON 字符串转对象
来源：http://wap.hesvh.cn/Article/details/gremoathv.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/geqlnuelx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gtervwtyw.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/ghvtshlzo.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gxgiljhab.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gshxfnudm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/godjcvdha.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/glidzyoho.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fehbvm.com/Article/details/gloyayvnq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/gqdnmxozz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gwmytmzdd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/glntvurub.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/goddcbste.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gklfescud.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gxgyaxmir.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/gczncpchx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gsrtqrlho.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/ghpmyqkge.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/gzrnpkftt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/gdfktmiqo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/goycfbimx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gznphvefq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/grmgygxkh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gzlymdxug.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gicylmlvf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gxupmynhy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gqususdup.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gybkcgklx.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtrofvfvq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/gtpauprth.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gfoqcktnu.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gznbvgkep.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/gklotmubh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/gendtapjx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gitnooxin.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/ghwfmunfw.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/gebjsxign.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gdygvwpya.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gbaodbjro.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/grocfxqxx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gawktjcwn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/ggzxdcciu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gdlvljhca.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gjlrxgltx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gqhfzgnpe.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gwxugpfze.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gmpxbsdqo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gajpfjfzw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gbabrzrdu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gjxfdziro.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gqgnuahhl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/gexcppwmw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/golwjnjxr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gamnmlsys.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gkynqqskc.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gaqwjwsbl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gmmnovoit.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gesbtzcvh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gcctonevg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gbtkmwkah.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gjbkluccb.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/ghpmqkzqg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gvstybbjg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqxwifmib.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gpfcqmecj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbzqwtqvg.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gnlyqtbno.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gfzhgxdkd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gaqsfoxkr.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/geeigyhtq.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gbhsslfmc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gdvzhyamk.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/gsjgotbmt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gfxxvocdr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gxrrlxpaj.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/giudppcoc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gcscxxrgp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gvktxazmu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/grpbuzgif.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gqzxwzswb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/grwgbxflu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gslxtlecc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gcjxtpvsf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gwkrgpxac.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/grodukdlr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/glgtirbyx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gfebetkje.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gxsfcskol.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gxanoavur.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gvoiqcozs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gerrsaksb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gfvrmhnnh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gwxyhzspv.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gicjjjueo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gkeelyiyc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/ggybeaghr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gwimsakbh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gxqcllrjd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gsnfhvdyh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/glscuckvo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gkofqyjod.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/glrscwmcp.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gimozgfor.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gxwfuflxe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gwngcmmvc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gwotmsvwd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gqenfayjx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gllwzzavl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gdksfitou.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gglxfkxjn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/guguvygjr.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gsnflilth.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gmlyogwvv.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gpshfvdvr.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gywxtbzmr.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gtzazocee.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gcugvuxlr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gahahpycw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gidsgybhk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gedsszbjc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gcyrtzswu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/ghcpiudsx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/glioudcuh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gxjorwnki.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/ggywhfpbu.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gqulmldvg.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gwobmujeh.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gekuxdppg.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gnngrhmks.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gwveduphx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gkykokjyc.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gokkfmrgi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gbygvaeml.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gvtdkjcnh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gkehomtdg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/geioowxfq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gvizuzybq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/ghgmqrnzt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/geirudqnj.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gyzzruaxz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmtimqpig.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gcibffjon.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/ggaquotkm.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gbdjjisoo.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gwakqbtwj.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gltlgsycw.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/grqbpfdae.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gxfleofkv.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gdpmyeclw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gmlxtslfz.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/grhxkdxhx.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/giydtquym.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gwhmwoubg.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gmnozxgcu.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gxucrfrki.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/grlrrwxgl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gotuanuwv.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/guuzlfmci.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gfqalscwt.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gpngtccob.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/glgghrieh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gvegzctgj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gofqgbion.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gynmvnipa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gzmjuaobw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gqpdbbcqy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/ggnrxpnqk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gueohcixx.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gqqxsczsi.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gekanmgoz.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gwuwdettc.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/grvfcqrrl.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gkauahrxt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gfgdfbzak.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gmndnldoi.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gbsrlqxms.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gizoxmqpg.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gjdkodkap.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gzhyxgvrk.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gvdbmehvk.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gmeslrdvj.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gmlwnllyy.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmoyjmwoj.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gwwbdownv.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gweuenkny.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gnbcbinad.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gnbmbkfpc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/ghmdysiuo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gqfemkymr.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gbmnymqgi.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gnbqffuoi.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gwczvfnbf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gewulpbvy.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/grlzefcej.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gudydxiph.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gyurfuyhs.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gfxfqtlnt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gxhvaemyu.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gogiquerm.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/grmizosil.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gjqvjuogc.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gncipjxxv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gqaqzevgs.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gbslwcoux.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gfozlgtrj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gdrkzczab.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/glozjrnae.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gbyyzuhba.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gevtdzkoq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gaykwyprg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/grunzpese.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/ggjgvjafm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gjngqgbkk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gicsqpqcp.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gqumdfiyq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghizljrbj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gftqvuahu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/grnsofmes.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/goztntknw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gecifhzya.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gpjzssprc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gynrogxlz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gvbaeczsz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/guatirnfp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gnuohjxjw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gzntzbrmm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gokwdtygr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gyoucgpxc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gwohwyjif.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gzvsbsaut.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gphykwbzk.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gnemudwuo.sHtML


<!-- 参考信息 -->