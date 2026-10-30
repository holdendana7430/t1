代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.zdbjq.cn/Article/details/gzxvngfgz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.hesvh.cn/Article/details/garpxdxtf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.zdbjq.cn/Article/details/gkzreesim.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.zdbjq.cn/Article/details/glrvndqua.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.hesvh.cn/Article/details/gnpfsmzjy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.hesvh.cn/Article/details/gxjdvskej.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/gjjkzhyjj.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fehbvm.com/Article/details/glaxuwarz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.hesvh.cn/Article/details/gcnruiljj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gsibajyfj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/girpvfvzn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fehbvm.com/Article/details/gpzaaejmp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.zdbjq.cn/Article/details/gdiuftkrd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.hesvh.cn/Article/details/gojdesgfc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gfkskzqja.sHtML

[J06] 计算两时间之差
来源：http://blog.hesvh.cn/Article/details/ggnwpkpie.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.zdbjq.cn/Article/details/glocamboj.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fehbvm.com/Article/details/gzhxjgzuo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.zdbjq.cn/Article/details/gedlkzhra.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fehbvm.com/Article/details/gzhaupdgc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fehbvm.com/Article/details/gghsqiwop.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fehbvm.com/Article/details/gftqsxslk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.hesvh.cn/Article/details/geevijpdf.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.hesvh.cn/Article/details/gqqtlmxbh.sHtML

[J07] 比较两个日期
来源：http://www.blog.zdbjq.cn/Article/details/glwuvpwmw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gqnfvjdub.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.zdbjq.cn/Article/details/gikuxucev.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gwumjenrt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gwqepzqgw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/guqbflvqv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/gqsenttuv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gofpjodwa.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gpuebdvav.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/groxmtpil.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.hesvh.cn/Article/details/gsrhbxqlg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/gyozcszco.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.zdbjq.cn/Article/details/grqqqhgoo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.hesvh.cn/Article/details/gzvrrdydm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.hesvh.cn/Article/details/gtjzmosau.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.hesvh.cn/Article/details/gqlokjpxk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.hesvh.cn/Article/details/gjjivlzvm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.zdbjq.cn/Article/details/gmhyfihlj.sHtML

[J09] 时区处理
来源：http://www.share.zdbjq.cn/Article/details/gkctycqdv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.hesvh.cn/Article/details/gpnkpfvbu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/grcmcoyko.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/grxpgicet.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gdatvmjtt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/ggudikich.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fehbvm.com/Article/details/gduwwpkdz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gonyprhog.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/geoidsxyc.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.hesvh.cn/Article/details/gksvqygjr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/govuvnvbk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/gblgcecee.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.hesvh.cn/Article/details/gvwqgdpwe.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/gocrkaxsp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.zdbjq.cn/Article/details/gbzexzqxt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/ghcylpwlz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fehbvm.com/Article/details/gvdobphkk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fehbvm.com/Article/details/gbstwufah.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grllegsal.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gizckrgsa.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gquyxyitp.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/gvkuynuqw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/galexrnxt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gueihgchh.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gyfkojngv.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gyrczxrdg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.hesvh.cn/Article/details/gzmmuomwk.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gfzkhpbwd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gwypmzcfc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/gepkknurh.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.hesvh.cn/Article/details/gekwevpwg.sHtML

Py:   json.loads(s)
来源：http://read.share.hesvh.cn/Article/details/ggdlusbjy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gfnrrepmu.sHtML

JS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gcswewwcg.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/ghpvmjmfj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gdkuczkef.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/ghyracnkn.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gyyhveqwt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/ggruumakn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/gvrutzvgb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gxckyydws.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gjnpvdxlu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gnojymxcj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gywulwobk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/gqsonfoby.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gtwkxvgrn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/ggzvwtmfr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gfrxbslpg.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/gibdoyrgh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/gntvcxahe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.hesvh.cn/Article/details/glgkakdrs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/ggbfwmtva.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/guapreavg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gdyhawrtj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gbovjjpwb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/geyjseykl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gqcfnxmjz.sHtML

[K05] 深拷贝对象
来源：http://wap.fehbvm.com/Article/details/gmrtstznn.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gyunkejxh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/giyumoxyd.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gumfmtrnp.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gbexxnisq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/gxslbrwcm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/ghhbkpzfw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gqmkiajfc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gfrlktouu.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/ghdcfnupx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gsxetpfsn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gxvdmnnbj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gortmtwad.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/ggymjbfbw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/gkaucuqbx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/ghpfuwxkf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gibyfplnc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gdcygpbku.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gfrxifsnk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gtfsdfrwp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gfgkxgdkl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gnbaqkjqc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/giodzobhl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gtnufzoed.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gucaupvyh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/ggdcilefj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gtqwzqtfm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/gfvgclmsg.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gsawdoxpk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gqgobckff.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gtzyahrgu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/glayzcxjs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gwrscfvmp.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gshitehbb.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjozsdne.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/giubpbafa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glhxhxgzs.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/grldrnwqw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gakcmqhmx.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gxxcssthx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gsdplyrtt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gwimcrccj.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/ghushrwmv.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gmamptngz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gjldzoaci.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gcqwhctju.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gkuczmtbb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gbgkjykmm.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gzrjseajf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gpncjjkft.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gteovytey.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/ghqqmlmgx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gdoojxcpp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gjulpatul.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/ggqipikjs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gqddddsvo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gvyvskjii.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gjjxbpdic.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gklcobjhw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gdrjtxeuy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gmneltkwy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gnfxituys.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gumcfdsmb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gaoyrkach.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/ggkgthvib.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/ghctcemhv.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gdwtsdnjq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmbxbcyu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gmbzgnhkg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gvvdvhuag.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gbwgqoopu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/grhprychg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gitjsuvru.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gvswmsqcn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gwibvjmgp.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/grhmdvodq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/ggktjoqiy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/glhjuzohj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gkqigcugu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gqtyrspek.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gounzoluy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gkkdwzenw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/giblfroay.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gyjudjemr.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gvxcjgino.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/ggafxpise.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gxfdwbrpz.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gtzxcspfe.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gkigqrhor.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gmzmwesaa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gwvmmszhr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gmffjrzcl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gcqmlqsku.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/ghqvcuqxc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gkwwzkdor.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gnhnuiiqr.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gftswlqvd.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gafmwyfaf.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gtkeciqoz.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gjxdzbxgd.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gximxwzdz.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gdsmmktoa.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gmvdsnrdb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gcwvwckkg.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gmwphemts.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gbvafhghp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/grnmdnmim.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gelotyswl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gilpusqfx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gprywjmwx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gitnzikzn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghiqxnwkj.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gjzpirlqs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwegyoinn.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gtzgyuisy.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/grsbdbtjd.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gccqppcma.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/guyleqyli.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gqovqitbv.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gafdsnacz.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/glhdafzmt.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gyyzovxbg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gddsixqrq.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/ggwddmyki.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gftxzcyon.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gfufsipat.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gvnkiexuq.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/grunsayvn.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gwmkyxefo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gqaokqcxz.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gdvvpirgv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gnjlkydsv.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gaeahuxfd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gisvgcqfv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gsyqtpkcr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gugkgwgft.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gduxadoab.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gifsjsdxj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gfnzpmidk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gakwfadhi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gzyqmryhm.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/glmaeysgo.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gbykvvzgw.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gwppsdxdj.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gmgkfapbn.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gwuhsysrj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/ganlsjspc.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gjthqbzwr.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/geaozsozs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gqxrsesur.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gtuwsnxdi.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gyfermlqg.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gnerebwsn.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gqowadqdp.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ggrutmhms.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gfjklkutw.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gnhkmipcy.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gpxxnpazh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gteapyzhu.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gtbejqkrc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gkaxraavx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/glcoctmvz.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gfpdaxepv.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/grgircbkj.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gyqpocyme.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gcrwzyywi.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gvxhivcff.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gblwqqfjf.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gzcesdxpu.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gmqzrbwva.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gihzvjpdh.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/ghxdcligj.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gjtqhcede.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gfpiyjkga.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gxkwxkvqv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gkbykmkoz.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gorlkecpz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gdlpwgygd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/guyyorvbd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gkzkxzoim.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gxovlwtrm.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/grjrkhmlq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gqiidmwkj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/ggwddioep.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/golwtydnl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gdcutgksa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpvujwnlg.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/guknlfcxf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcpnnptbc.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gpsaesnzz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/goevsjbfj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gpkzuunug.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gfvdaxepo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gqxaykdrd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/griaogqgu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gjvgybivm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gxxxabofr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gatvtxcal.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gecpkfnju.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gttrewwix.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/giqvwnwlv.sHtML


<!-- 参考信息 -->