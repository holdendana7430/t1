代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/ggacjqclh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gbihmuoym.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gmeoawxqd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gtlpetyfq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fehbvm.com/Article/details/gbfvmohps.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fehbvm.com/Article/details/gfcgqdlss.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gmedanlrh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.zdbjq.cn/Article/details/glmapabno.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.zdbjq.cn/Article/details/geoozlpys.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fehbvm.com/Article/details/gyqddldic.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.hesvh.cn/Article/details/gjfuavxkc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fehbvm.com/Article/details/gakxsuedu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.zdbjq.cn/Article/details/gfqgzzxkn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fehbvm.com/Article/details/gzizzqelk.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.hesvh.cn/Article/details/gkuieknvd.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.zdbjq.cn/Article/details/gtgngvhid.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/gfeinjexw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/ggogqcaqp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/goilqouhr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fehbvm.com/Article/details/gquwngudl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.hesvh.cn/Article/details/gckldhrmq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.hesvh.cn/Article/details/gkuyyagxt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.zdbjq.cn/Article/details/gsxfvcwgm.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/gegbyekhl.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/gcdwascyd.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fehbvm.com/Article/details/glnnyiafg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/gqmhireod.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.hesvh.cn/Article/details/ggumvgiqt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gadwaabaq.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fehbvm.com/Article/details/gwgoheopb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fehbvm.com/Article/details/gyezduerm.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gofgdowih.sHtML

[J07] 比较两个日期
来源：http://www.m.share.hesvh.cn/Article/details/gdnivblbz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gqeiekboh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.zdbjq.cn/Article/details/gtemuiodj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gmrpnstuz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gwncpigkm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fehbvm.com/Article/details/gedlrxqze.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fehbvm.com/Article/details/ghynkvpvq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gjfkvthzj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/guziiijmt.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/gdavxqkar.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/giezmecfw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fehbvm.com/Article/details/gvsgoyvsk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.hesvh.cn/Article/details/gqvkwonjr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fehbvm.com/Article/details/garsxkudp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.hesvh.cn/Article/details/gmmccmauh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gaquzisiy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.hesvh.cn/Article/details/gjvzgrkcv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.hesvh.cn/Article/details/glvomxvme.sHtML

[J09] 时区处理
来源：http://www.blog.fehbvm.com/Article/details/gpcfoxkbl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/ggpnzfngg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fehbvm.com/Article/details/guhfbnqae.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/giscxlwji.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gtvybwcla.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.zdbjq.cn/Article/details/gsuhapdxd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fehbvm.com/Article/details/gnhfuylgp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.hesvh.cn/Article/details/gyanfofzg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gxfjzsnwi.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gorbjcspb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fehbvm.com/Article/details/goxzgehas.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.hesvh.cn/Article/details/gidkivqzc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fehbvm.com/Article/details/gykudumqr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.zdbjq.cn/Article/details/giegmbbsp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/gzmnonjna.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/gwsqlkctg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gqautdcqy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gzsixrmoj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbizyjqaa.sHtML

K. JSON 与序列化
来源：http://baike.fehbvm.com/Article/details/ghqndjthd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grtfxmdmk.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.hesvh.cn/Article/details/geuzyxwgf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gdnffzyne.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gauagapvv.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gnagggdae.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/goqoydqmk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.zdbjq.cn/Article/details/guvnmsgna.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gpahfwmfk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gosromszi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.zdbjq.cn/Article/details/gvoogwyjj.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/gukxnmdfc.sHtML

Py:   json.loads(s)
来源：http://baike.hesvh.cn/Article/details/gtqwzgraz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/gbojzwrsd.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gpuxcqxdu.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gekxbnglj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gcfljojih.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gysutsjkk.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzowdtrea.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fehbvm.com/Article/details/gignvexle.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gvwhkqnld.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gitpdbrqf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gtmyqqsas.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gysvphtrr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gcmcstled.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/gtuuspesu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/gnqealemi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/guqachfge.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fehbvm.com/Article/details/gpffefgoi.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/gxdpanoaf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/grlfzccgo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gwtycjagu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gksyozkkq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gaolckzsw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gjfhknmxk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gzwriwdxm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/glniacikd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gkevuquue.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gxireatos.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gzpdonqno.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/grunpvmcn.sHtML

JS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gwewaevnu.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/grewiqizd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/gwkbbzqfe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/grdyiagou.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/gmjdaeees.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gguzlmpnd.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/gwrjqzupp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gpiibzffi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gmglnkude.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/ghdhuramf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gjlywrsjg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gybozkzim.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gnrbfmgbi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gsslonzee.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/geuncuhem.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/ginjcjczz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/glsfavzdi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/ggzptcvam.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/golhpyfxr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gssvqxgxq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/glvtxcpoa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/givlsrouf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gucxofirk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gmvgtutfj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gmksybmru.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gyatqdspv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/grfbdzmtl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gwdyjbmrb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gqznaxgak.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gaioemxgw.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gvegnimlm.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gsnmhmsoq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gtdvtaekn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbeniyyvq.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gexpjhypw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkwhekice.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gnmnuvdal.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/ggcfopzrh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gakodvzts.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/grklnibbx.sHtML

TS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/ghzxwftso.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gjkjqdxvn.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/grvvxkzuk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gdxodisys.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/grohajgsj.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gkampdsgo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gzuclbwpw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gcpmrvafn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gyvwrebad.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gvdehkpat.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/glxhmhqse.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gnzhevwzj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/guzzlvoqb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/grznldwrh.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gnrkrypfo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gzziejzry.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gpplqmjvw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gsgqcdbql.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/giueckpzl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gjevqgavv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gnswkrbrv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gxyzwmwgi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gegiphtbl.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gfbjikdgv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gnnpfqwih.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gpawiaebs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gocemvvwg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gfuupaajl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gdbghsvzj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gupvyjpeg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gjusgwpfy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gzvmjzfvg.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gaxkhtzan.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gpeqfuhzg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/grelncueu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gdgsgvtsm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gbvhwbkkk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/geijvrbtm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gogwpsuuq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gzcmgmnag.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/grczsfvzl.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gsiboidnb.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gqpcphjea.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gnjuhzhwt.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gvzblocbt.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gkyvkcndb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/goexxjpue.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gkswhxtbl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gbozapyva.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gwpbzpqmj.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gdeoqbjdh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gekqplebh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gvpocfwuw.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gqjycpgyy.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gtsqzycbp.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gmrhyjszm.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gdskepxhq.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gpimlorlk.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/grkebttek.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gulhulzpj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/ggdxongqn.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gawbwxydw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gkurymbmc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gosxcbuhb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/grgkttcsj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/ghcwmqnst.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gcjyrzfdc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/ggekesxjl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnoqcdaaf.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gnizznibw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbdqvhfgf.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gqxlcaziu.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gwudrjicn.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gyqnkhmyc.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gdbeccvay.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/ghnigartq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/goojzazvc.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/glneuvmjd.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gduqzupfk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gieiplvzk.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gvuhjamux.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gizicdizy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/glaqdfuap.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/grmvclszr.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gtjymlgoy.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gvuvlxxng.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gjxyajfps.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gducgwkdv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gdhggypso.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gmpaeszia.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gixxfayum.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gdrnvnhfq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gzjynpfey.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gqydzosjh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/glcvwcgah.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gijeoplyb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gqnzebfqo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/giobopbgp.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gkreixfch.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gepdqlvyc.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gixgmxgml.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gypzuaixk.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gmcqoidld.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gchgnvczx.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gzbmprzgz.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gmzdzblyh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gvpulwgyu.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gtzgbbwrc.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gaahtfeml.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gwyrtutya.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gezpluoeq.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gfpweohfv.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gqvgzwwks.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gxidtxlot.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gojsupphv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gdmdrkroj.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gprbxbruz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gldymgtvt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gemahxrjc.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gvmomnunt.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gmpdeacyz.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gmbnyymug.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gbbdydbos.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gmjqboaah.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/giqjdbukw.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gpsghrwok.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gfblffqrr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gkipbgmka.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gltsdaefn.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gzkwslgnm.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gbkeaqpzq.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gqzilzknd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gdnokudym.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gyekykmzj.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gwtodejfs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gavblwggc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gcyrftbwa.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gkysprrri.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gnvtnuhrk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/ggbyrxxrx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gecjgvxyq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gekepwilc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/guwvfzfcg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvdilbaxq.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gijvxywtu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcxwysuvz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gsbhyunlu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gwybryhdn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/glvulcxvd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/ghswrzkww.sHtML


<!-- 参考信息 -->