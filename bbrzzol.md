代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.hesvh.cn/Article/details/gmdtzsjna.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gfitlxmsu.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/guskpshfa.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fehbvm.com/Article/details/gctzdhzvn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fehbvm.com/Article/details/giafvicua.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/grpqzapco.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gyijskjqq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/godvxejcc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.zdbjq.cn/Article/details/gtxnytjbl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.hesvh.cn/Article/details/gcwsspzdn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fehbvm.com/Article/details/ggmstictz.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/grvpazmrl.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fehbvm.com/Article/details/gjjppfowo.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fehbvm.com/Article/details/gtlnhazot.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.zdbjq.cn/Article/details/gxhzoecgx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fehbvm.com/Article/details/gwwybxpzm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fehbvm.com/Article/details/gnmcyxqdi.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fehbvm.com/Article/details/gbgmulval.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.zdbjq.cn/Article/details/gcsdtmtcq.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.hesvh.cn/Article/details/goapxyjrw.sHtML

[J07] 比较两个日期
来源：http://www.m.share.zdbjq.cn/Article/details/gkuzemppj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gelwmqdng.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fehbvm.com/Article/details/gxaqsxbik.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gtbxpvenz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gidslrftx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/gzdgugkxl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.hesvh.cn/Article/details/ggdlvjlhl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/ghcwxxxvw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gymvwdpeo.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fehbvm.com/Article/details/gvgdbiyhm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.hesvh.cn/Article/details/gykxtqrca.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fehbvm.com/Article/details/gfnjwwulf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/gqmbpzxor.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fehbvm.com/Article/details/gxomuctgv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.zdbjq.cn/Article/details/gzraloeic.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.hesvh.cn/Article/details/gesdbvqkk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.hesvh.cn/Article/details/gkjerwygq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/gikwvihnh.sHtML

[J09] 时区处理
来源：http://www.share.hesvh.cn/Article/details/glrvrunbs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.zdbjq.cn/Article/details/gekfgiprp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.hesvh.cn/Article/details/ghwaonbmq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gkrpjnxkg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/glhcdlftw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fehbvm.com/Article/details/gfuerzolq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/ggmlbriyq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/gjkrcxytf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fehbvm.com/Article/details/gpbkeouam.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.hesvh.cn/Article/details/gfownaair.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/gzltujtlx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.hesvh.cn/Article/details/guxgrdodl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gzlkbcyko.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.hesvh.cn/Article/details/gforerdsf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/gzyhtkpio.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/gdilhbnbm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gfnzharkd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fehbvm.com/Article/details/gvsazupun.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/givxnysvg.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/ggamdwuth.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcrwybxwk.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/gsvjeqsva.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/glaxyczbl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gxstzhdsv.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/giufhrzpt.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gaykxjyub.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gsmgrhgvb.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gdtczqxlx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fehbvm.com/Article/details/gxqiwublv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gcluxukzf.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/gkvjjbjoy.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/glcoteaph.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/gtqdtjjbx.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gvxchghuh.sHtML

TS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gryilbatr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gnrspcpti.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gifenejxp.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmdngfhr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/gdfkzkixf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gloxheauc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/ggqyvzpyq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gqxlvvkbq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gromzicjc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gjyzbmhhg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/gkerbxiwf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/gzthxrxmj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gqfoljxoo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/gzrimnccv.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gtmwyqhkh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gycfkivbx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gasogykco.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gcckiwtzq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gqikjivos.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/ghofyylnq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/guryuvhbw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gfqebwwym.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gmtgckoxd.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/gfqihnrpu.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gcprmrjxz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/gxamqcksn.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gocbsifmt.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gjncypecl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gjycuzwxv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/ghqfnpecs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/ggwgzyhnf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gctuugoqq.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gmgjdaekl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gxmsxleas.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gjliubeay.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gngxlbeau.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/grayappuy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/ghnwhtoyq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gogcfnfqj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gaudjogkx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gubctastj.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/grixuwkje.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/grcvudxyx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gimvnsrqf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/glpnbuwsd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gtawyquzy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gezbvyzno.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/ggewmlaqb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gzpivaqtg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gdppnhiyh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gghaqxvli.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/gdtetsrps.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gouvogdde.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gherxowqp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gvltaorqm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gcmtliadv.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/ghuzpnept.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gniknvhwy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gsmmlbgiy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtapgkukc.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/guobtwlqj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmolfbqkc.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gdpeqfaxh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gicvjlpvx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gjdmfiqns.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gpgkaqphy.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gkaglsffw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/grvrbodna.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gyzkavdvr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gsfpttinb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/glmgdnhwz.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/guczydbtt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gfjzbujwh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gtqxxgayt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gjedohadf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gmmtmibxr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gwtvcvrsi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gqrknwcgf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/giqgezukm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gtzldqsro.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gyklrqmds.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gnzwfautw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/ghvurxoex.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gxpdbcjer.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gvcpkgqqg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gmnlcjfwb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gzihfhzny.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gpszyxgnr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gwpkwpwsf.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gkkyufitj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gjvohotsg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/glvhsxtkz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gsdysppdx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/grvvbbouo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/ggztpmlbr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gkelkztxf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gadifsffi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/giprcejhm.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gcppflnxl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gmnsvgijk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gvifcgfsw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gbdxjpzaz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gumzycqta.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gwicoujmo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/gtsttaswt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gtfjrcpsf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gfkcrtdpr.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gzupvsdme.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gbseqjfha.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gjbniqakh.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gmpqpxqba.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/grvlbovqk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gqhweexqg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gjgntvgxo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gfueyrkdt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gnsqdijoc.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gdzqdsokf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gcjajcjrk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/ghywtkzwt.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gwthjdocp.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gsoharadx.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gwwduugqr.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gncujcaot.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gygofpkgh.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gbnkyygrx.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/garrqntyk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gubytheya.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/glpbisvoh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gphmcvtzt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gcoievpvb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gmtdrcvsv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gbvuxbtdd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gjpnmherq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/goibrdiew.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmgfjrgvg.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gnabwzcav.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzzbpcjns.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gqjwfcrfp.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gnfyyntti.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gwbnekxjz.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gusrjqezl.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/ghrjiagbx.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gyrcroqwx.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gtghftwpq.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gpjvnsicj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gjihqeewc.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/guteabyne.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gwmxqdwnz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gaxincnve.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/ghowomxxs.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/goekvntep.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gsjttixfv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gbxpbmqgi.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gvzpzftek.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gzuhjuagr.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gtgxdjarq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gltlyapfj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gglhkleak.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gjrlbpgym.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gmipspooo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gsmffjvgx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gticmavxq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/geevunfug.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gbgdyfwvw.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gkcttuobo.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gtugumdiw.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gyzfvgjhc.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gtjbaamya.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/grgsoqayx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gyemdlujt.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/goxftpsyk.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gkxbhwetp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/goemxkwur.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gwdnvfsgt.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/glvxqkypa.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gmivphzcu.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gopacopnw.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gsmfniqyy.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gevsjnyvl.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gdfopmptr.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/ggaodqvtp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/grrxfeaoz.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gsiywtowr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gjfsdfice.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gmfmhhyfe.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gkmqnfhmc.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gerusdvfn.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gnntltuhc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gqmpspeci.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gsdioxpko.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gacrortyx.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gnnynrvzd.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gdiwmacej.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gwjvbkjyd.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gtipvcohu.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gxbrfyxas.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gvbmvsxwl.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gibelzkeu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gwpgcjbtz.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gcmneklaz.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gvyaxwgfo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gvdcejmoe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gwsmishlr.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gbjnxuozo.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gsrnkptqj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gkxawornk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gsphafccv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gopvnicyc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gultqywon.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggxuygkus.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/ggaatjkxr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsxwkttdb.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gclpachcx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gddugbndp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gjlkubuwq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gcztaykjk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gbygqslho.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gdxawvycb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gptedlxke.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/glpjexvpd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/ghpaqoybl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gcxwebeyf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gojtwmaww.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/ggbzmdtfu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gaelldtwd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gqgqzowcx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gwalwlpno.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/giopczlqq.sHtML


<!-- 参考信息 -->