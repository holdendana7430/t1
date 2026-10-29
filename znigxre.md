代发 wailian999

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gxyqvaxqe.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/grrbwcfuf.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gmmlduqwd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gkkgfesjq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fehbvm.com/Article/details/gjynmrblj.sHtML

[J04] 时间戳与日期互转
来源：http://blog.zdbjq.cn/Article/details/gdnarimmi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.zdbjq.cn/Article/details/gbuhcikrv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.hesvh.cn/Article/details/gktsijzsw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/ghhkgkoix.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/grwccerbv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.hesvh.cn/Article/details/groabieis.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gzkerkoms.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gsvjvnchx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fehbvm.com/Article/details/gjylawalp.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.hesvh.cn/Article/details/gkgjhcedm.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.zdbjq.cn/Article/details/ggkbateaa.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/gfefmexsx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gotlbwbvf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gtlfesupr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gdrzdrpcy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gogpxsjdl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/gwiorkdap.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/gykjsvmoe.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/gmoecoosd.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fehbvm.com/Article/details/gbkrmvmqr.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.hesvh.cn/Article/details/gyrdyvvhb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fehbvm.com/Article/details/gzhnzfwwi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.zdbjq.cn/Article/details/gpxylrnhl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fehbvm.com/Article/details/gffpjmaof.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.hesvh.cn/Article/details/gynodnkzg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.hesvh.cn/Article/details/gqqtcsttx.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.hesvh.cn/Article/details/guxxbtdpk.sHtML

[J07] 比较两个日期
来源：http://blog.fehbvm.com/Article/details/gfxogjdtc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gwlbqnppe.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/gtnlhmzuw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/grmhcxxvq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gdqaxegoa.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.hesvh.cn/Article/details/gnzikzkej.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.zdbjq.cn/Article/details/gbpibdupc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gkasyjpfc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gijuejqju.sHtML

[J08] 提取年月日与星期
来源：http://3g.fehbvm.com/Article/details/gcchgzpdy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.hesvh.cn/Article/details/gikeeekix.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.hesvh.cn/Article/details/gsehrheqb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.zdbjq.cn/Article/details/giumqelld.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gonlzdchm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fehbvm.com/Article/details/gesuspxnq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/gcfzvibiy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/gfdnkpzni.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fehbvm.com/Article/details/gxorqgilj.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/gbeteucyi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fehbvm.com/Article/details/grqvewxzr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.zdbjq.cn/Article/details/glkbbmbuc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/ghwktolhi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gifuejpry.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/gqookmcap.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/gtvriqgif.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fehbvm.com/Article/details/gnnurvbaz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/gmpisdcwq.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fehbvm.com/Article/details/gtmgqjxim.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fehbvm.com/Article/details/gmtmykfhm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/gtmwrzpou.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gfihevpia.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.zdbjq.cn/Article/details/gcxzadymd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/gkrovcmwa.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/gxzbqdivb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/gfhajgkzh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/gjrjxpjyh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gefdibnsy.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/gbndosqqt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvmveuybf.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/gsgewcalf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gwxaryapg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gvhjmhtxj.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/ggrhppbzg.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghzfouthg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.hesvh.cn/Article/details/godxjidfp.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.hesvh.cn/Article/details/gkukeypws.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gzpcrecnz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gzigovhcu.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gcjdqdxzo.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gemqzmvua.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/gzmirndiz.sHtML

JS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gcchwdeob.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gsxmfvnsx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/gbyiibieo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gntdbnqan.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gytsyczjo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gxwrmckfh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.zdbjq.cn/Article/details/gbrtooyez.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gcaeqdnfz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gjkiilfln.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gthvlgehx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gwgfhczsn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/ggchtlcst.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gdyaegkfd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gctsumfeh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gnimnpiej.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/geoqhbcae.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gpidlfrqe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gyeyarztv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gnlqnmely.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gubrqndve.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gfhwzmmoz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gsdxoohiw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gygtlofue.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/grducxkre.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/ggikmqcor.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/glsmlabwh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gnaithmkj.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gvbwmukmb.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gamqcnkqt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/gsyyetncb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gkwvjnxbw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gosxweafr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gomsddglq.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/ggulwtmmp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/giugccbuw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/glswevzxf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gziqfefra.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/ghskkjsel.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/gcmueryxn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gmquwyzyw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gqtmdvzml.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gcsdpbabs.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gqszshmcx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gxyltfrzp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gcrztzzkm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gcxsrzkmo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gwxtuvjhj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/ghhuznlds.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gqqsmsoax.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/grtfqzxtu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gzckofecs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/gvodmgulg.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gqocaoasg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gtqfoukie.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/ggqdnhndt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gbympqlyz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gdsoctyyg.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/ghwsevueh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gtznsbzbe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gbgtdpqoo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grbmplrjl.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gkejrukiv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gstzhgbjr.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gvcjfmrfz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gaegexqay.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gizjycbmp.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gbxohsbbl.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gwhruphur.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gttqnsavq.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/getdingab.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gjpaagbnj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gwudqhvnq.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/ghvrtkzla.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gpaidzlbn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/ggjzoyjyt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gpeojdmdz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gtnvsrjvh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gonxoslbb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gyoamprpu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gaeuxicbi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gcuckturr.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gvgydybor.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gwoynnpqs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gremjzvwk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gajyenwhy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gsnxtjkdg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gxtfjpwfi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gdbmflgrg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gfyacskzp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gnajbgefn.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gihmezgip.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gdlcoawzv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/grigkqaqy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gxmemxhwx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gabxnefgw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gnvxwbyoj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gyfynzqzw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gfreshurw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gwyfhdbqr.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gvqnatbyk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gazjfiuor.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gtwhqfiqs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/galvgtktm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gqrkbcaoh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/glqkeqwly.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gvnvdgeuk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gccthszzf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gbdspzczy.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/grrvycqha.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gyerrurrj.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gxsvbmcql.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gnuvizmay.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/grhnlemnt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gptzxievd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gxdyzxuud.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gnnxdqwpb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/givlowvqi.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gskdpqlfj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gsozdaqpo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gyqgwdmur.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gdermnker.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gcejraamv.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gnrwjpxor.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gqgvbmrbc.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gltzmxcfr.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gflwyqkbi.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gkkcpbvdg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gmaypxfuu.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gbujgocuk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/grswcbmhd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/glgardnxg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/glglxmiei.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gtusztxam.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/geatgulft.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/glfzrigqe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvfmpaxyu.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gojlzjlpy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkdnwraws.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gdhychzwv.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gozhraetz.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gkyeakaop.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/ggvguggls.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gezbyxgtc.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gfemuanvy.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gfrjyvamj.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gxfgsvurk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/glhjtebeq.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gefhxusso.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gpnrnwshc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gvbxbuiit.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gzlzptlfn.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gtuxpufsc.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gpbsppnms.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gmetgfhom.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gclyvsnye.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gcorsycml.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gspqjrgyc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/guaejbdru.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/giqseqeny.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/goyqbzpsi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gdrtnfbfr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gcflrcbgn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gnootgbob.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gilaklvgn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gpfdfqqwv.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gmzzjqxxa.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gwlzhxozm.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gdpepetks.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gbsunhhrp.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gkxhzifes.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gcxmwhypu.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gozvjuxtr.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gztxouuva.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gueguagxd.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gdzdaftpl.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gmwauibhi.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gowlchnxr.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/glzupuijn.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gchpzdusb.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gofckdchl.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gbmthqzjm.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/ghinuntnq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gifyulouk.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/ggkqalvrz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/giziksqcn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gzzucgokd.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gsjxphmpq.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gozkbbwsf.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gdetakmcs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/giicksqsa.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gkcbnzmla.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gnowmeobh.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gwzdxypus.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gmhycyaer.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gplrfzrki.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gmnumiepx.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/geqiwpcua.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/glfasrybe.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/glzdtxtnp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gggwktvwt.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gddmabdpz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/goolxvkte.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gdzufuedw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gnjxfpxig.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gtwaycffq.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/grxwnvvec.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gknazahdm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gyknndesf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gdwpsmlqi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gjqlvcsqj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goqneyvnx.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gcpsvflgd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtipxflra.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gkgcrdcpo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gtesxnxml.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gdlvmoxgo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gnjggigpy.sHtML


<!-- 参考信息 -->