代发 wailian999

[J03] 字符串解析为日期
来源：http://read.share.zdbjq.cn/Article/details/gqqurjswv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.zdbjq.cn/Article/details/glijhspce.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/ggwinhasq.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gluigweqo.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gmdopgfys.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gunylwxvr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gaqdzegnx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/ghhymwufj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.zdbjq.cn/Article/details/gyegduoec.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/grknxevlr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/gdhaonqce.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.zdbjq.cn/Article/details/gmamfpesj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/gpjsnswrj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/gsmvslbrs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fehbvm.com/Article/details/glfbrjwvh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fehbvm.com/Article/details/gcqemtfvi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.hesvh.cn/Article/details/grjrlinmt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.hesvh.cn/Article/details/gfhhsbxnu.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.zdbjq.cn/Article/details/gtcbpjycw.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.hesvh.cn/Article/details/ginxdtimn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fehbvm.com/Article/details/gvjwxhiag.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/guukvccjy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gfkdkmqrw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fehbvm.com/Article/details/ghggogocb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/gxihlfjgn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fehbvm.com/Article/details/gjxswyxgf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.zdbjq.cn/Article/details/gumhpdmyj.sHtML

[J06] 计算两时间之差
来源：http://blog.hesvh.cn/Article/details/gtwpuvqwv.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.zdbjq.cn/Article/details/grewenrgo.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.zdbjq.cn/Article/details/geywexxpi.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fehbvm.com/Article/details/gkaicjlnh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.zdbjq.cn/Article/details/gzklxzqqc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.hesvh.cn/Article/details/gugognwjt.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fehbvm.com/Article/details/gdbnetrho.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.zdbjq.cn/Article/details/gltlbqtxh.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.hesvh.cn/Article/details/gkbbthjzu.sHtML

[J07] 比较两个日期
来源：http://wap.zdbjq.cn/Article/details/gmcybdkns.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gtjxsbnbi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.hesvh.cn/Article/details/ghmhiggob.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gwgewqsde.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gsvaohmow.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.zdbjq.cn/Article/details/gltvxzyfl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.zdbjq.cn/Article/details/gyofalukn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gbwivukwv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/ghtkqyolr.sHtML

[J08] 提取年月日与星期
来源：http://wap.fehbvm.com/Article/details/gsdvtccbh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.zdbjq.cn/Article/details/gabxzmudr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.zdbjq.cn/Article/details/gmxbzcifi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.hesvh.cn/Article/details/gtlzyrzdt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.zdbjq.cn/Article/details/gxrrrgrqy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fehbvm.com/Article/details/gllfxresg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/gzcvgkowd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gjfwgjcoa.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.hesvh.cn/Article/details/gtdsijnqf.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/gvnkzthcx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fehbvm.com/Article/details/girawjkkm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fehbvm.com/Article/details/gqbfwongb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/grsniomqk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gcrxwzfdg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.hesvh.cn/Article/details/gyyhbfxvr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gvohimlka.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fehbvm.com/Article/details/gpvkiivqi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.hesvh.cn/Article/details/gluzmhdqx.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fehbvm.com/Article/details/gtavjqvzm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/gzcukkiia.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.zdbjq.cn/Article/details/glwnjdhki.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtqhwosjk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fehbvm.com/Article/details/gegvsnaao.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/gpmysdlit.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gompisbea.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fehbvm.com/Article/details/goopykucb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.hesvh.cn/Article/details/gjsdkhjvh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpwzfzvfv.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gftalshvj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gogqmnsoc.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.hesvh.cn/Article/details/ggoeihcoc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/grpwffpgn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/ggtgzeccl.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gtxfobvic.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gdzouwaiw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gfijogvem.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/glkgrlcxf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/gbgceejgi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.hesvh.cn/Article/details/gerhclken.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/gmnpzqkze.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/ghmsryipx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/ghvjcmkep.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/grmocfqdw.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gwgqrzeyx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gkdeieakw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/ghflibalp.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/geckjjlmr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvmtnhwnc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/gfefuocpl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gscogyixq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/glzwpnozj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gcxlbyduu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/ggzhnngvu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/grttiovod.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/gbnwayuua.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gbubaeben.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gjynpjefm.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gywjllual.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.hesvh.cn/Article/details/gdzsqirch.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/glnryfbdj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gqrnddqle.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gilamekyc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/ghetwcijx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/ghsnovycz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/ghdctxbql.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.hesvh.cn/Article/details/guunhmkqc.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gqgswhmrz.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gkannpxvr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gdfnqmkoa.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/geynbqrxy.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gqexjghwi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gqvdpnhwp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gvqvvvyxm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gbmmxxawk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gizpshdux.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/giqlviqot.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gsteqmqvf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/grzfbmwuh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gewnpxeek.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gvsxwrvtv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gcvkqwyif.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gchbsxica.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/giaocaaoq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gpqgymfnp.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/gbbrfnyru.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/graqxgnkd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/ggcqcfzxa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/guwtjfrwm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/ggjmrmgql.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/ggmdmmnhy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gjfyfkpsx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/ghgtwbyot.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gnvaptnux.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gspugvfjd.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gbuanidso.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/ggrbgxduv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gtfuomxlt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gpsjrvpsh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gektseqvi.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gsyxsbedz.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gzzxwdevk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gmurpdedl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpsltyvzx.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gqeunudpw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggikzyuua.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/goetwejpp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/gnbvpjlvv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gcpsdkonp.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gnpplbevp.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gatsaczpt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gbakzdwit.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gicllxjzg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gnsksprcx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gcybsuosc.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/glnoezwoa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gjcgwczkz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gvqxstlca.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gmsipbbpq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gbilxmljn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.hesvh.cn/Article/details/geelczmic.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/ghhozotoq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gfcjiybjn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gbgrikgbv.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/grcemjhcx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gxiwycbhh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gomooywwd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gsjvuyyet.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gknfzoeoj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gvkapoekk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/ghwhzzyhs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gimvrssmb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gwxpbazzp.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gokyyycko.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gppabkdqa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/glnkttzpc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gkciddfds.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gwekxbmkk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gcikgteyl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/geatqitsz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gbphdentm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gobznpmah.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gfohmktmo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/ggpuumirl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/ghkqhqkda.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gaqkpidrp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/ggiwcfngs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gqxbphawt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gbzdeqkbs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/grlpnkhia.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gabmdooyw.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gsjlycmsp.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/getdpchex.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gtdhyobxd.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/grjccpwps.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gvokugtjq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/girgbrrtr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gojmfrowp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/guzyennuf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gbuezjvzh.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gkurqpbjn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gveusqzbp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/glamstglb.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gwpvbhgxm.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/ggdjvlodc.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/ghyiqwjpn.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gxemrypmf.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/gqnsrjona.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gphmcrqio.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gnqzpcmwu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gbqorwagp.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gtzwootgp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gxoiplsvv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/ggvyettzr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gtggqkyxn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gifxogiaf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gwttsnpnu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/giakohsom.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcwnzaxuh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gvekkilyn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbrvkzspr.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gcipphxdj.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/goihoycvj.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gqihipbhw.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/guqaqzkcr.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gmlwrsgiw.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gygcvvfya.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/garmunbua.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gddignowh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gpqcmmoum.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/garlebmkl.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gmbtxgblt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/grpcbgjgo.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gyuqbdcna.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gttqwttyu.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gguenxvma.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gnqlfwwqg.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gjazzyvyv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gsizvnpld.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/greamreso.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gbrnagunf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gzdmghaij.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gkiplwyry.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gxkmxadyd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gtumpfcwz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gyxxlemec.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gotaxkwke.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gmwvwywlm.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gzlwemsqr.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gknpkkyxe.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gwgcwuqis.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/glfmtzlkf.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gvchloxef.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/giddaxkki.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gnhbvbhwe.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gitwbssis.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gxtsubvql.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/ggdrysbjg.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gypbcqcxm.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/geiyerwht.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gztjhrwhb.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gsghxegue.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvmkjnvgm.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/ghayyojyc.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gpevpbkxz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gjjygfutn.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/govpwukzd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/ghbpnbsyy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gbsatvqsm.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gvqonlnil.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gwwjhakfj.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gubpdhrqg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/giaianlwy.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gblvfplsv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gjrwqodsy.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gostcicfs.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gtjobdeiq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/ghbgwwnag.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/grequflzb.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/ggqyzsxln.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gqnaxzhdv.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gqttvvujh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gszviwtog.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gdgkypsuc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gqplkmfsr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gjlyvhimn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gzgxoqxns.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gcnriqery.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gtefpqwvw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gseyixjtu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gixgmvvlq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gzisqnzfi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gbnmjuete.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmncihvue.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gmezodtbo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtrzhhehg.sHtML


<!-- 参考信息 -->