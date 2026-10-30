代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.hesvh.cn/Article/details/gqudmkwim.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fehbvm.com/Article/details/gkugmjppk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.hesvh.cn/Article/details/gztyrlpkr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.hesvh.cn/Article/details/ghnkdwfam.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.zdbjq.cn/Article/details/grdlcuddi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gylunvbtq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.zdbjq.cn/Article/details/ghwztnofu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fehbvm.com/Article/details/guomivqfx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fehbvm.com/Article/details/gbdttppvi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.hesvh.cn/Article/details/gnqkqwfvw.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.hesvh.cn/Article/details/gbhbrlzve.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.hesvh.cn/Article/details/gikrginup.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fehbvm.com/Article/details/guzeivlao.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/glqktptxi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/geyszokkr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gylzehcmq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gozbveygx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.hesvh.cn/Article/details/gamvtpffg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/glwdshsac.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/ggybhqgox.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.hesvh.cn/Article/details/gerlmkifj.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fehbvm.com/Article/details/gmcbhplzq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.zdbjq.cn/Article/details/gyouxerrs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.zdbjq.cn/Article/details/gfqokehti.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gbwkgzeeg.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.zdbjq.cn/Article/details/gghpyquja.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.hesvh.cn/Article/details/giwghonhu.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fehbvm.com/Article/details/gyeqhoyeb.sHtML

[J07] 比较两个日期
来源：http://read.share.hesvh.cn/Article/details/gdvxdriam.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gujhtudwx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.zdbjq.cn/Article/details/gafiteime.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gtcwydppp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/getkdokti.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/gilnbljlv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.zdbjq.cn/Article/details/gzxazhobz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/ggzsuoxkp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/ggvnyxiuw.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.zdbjq.cn/Article/details/gfxzzaxhx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.hesvh.cn/Article/details/gndbisccs.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/gwndicwoi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.hesvh.cn/Article/details/gvfhjgrpb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.zdbjq.cn/Article/details/gpjyremqd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fehbvm.com/Article/details/gccibaekz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.hesvh.cn/Article/details/gxrjtslfn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.hesvh.cn/Article/details/gkgaovlks.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.hesvh.cn/Article/details/gsvebooki.sHtML

[J09] 时区处理
来源：http://blog.fehbvm.com/Article/details/gtuvhqcjt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.hesvh.cn/Article/details/gwkpefepj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.hesvh.cn/Article/details/gxnjtkcdb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gjotgfawd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gylbdxmph.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/ggcqxiymj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.zdbjq.cn/Article/details/gpjtmdfya.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/gtiaqqara.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/ggfcacrdl.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.zdbjq.cn/Article/details/gfgzcrkpx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.hesvh.cn/Article/details/gtjififpc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/gmmeueyxp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/gvckihvtx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkcfjspqm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/gsidjumkd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fehbvm.com/Article/details/ggyrbshol.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gkxsqkriv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.hesvh.cn/Article/details/gusnabpsj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grnucdqio.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/gqsjxuzup.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmncvrpwv.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/gpapcjihb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gkmvkzkxn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/grdvalehh.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gelngrnhg.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/ggjqrmksr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.hesvh.cn/Article/details/guzxknwwh.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gqjjycqdd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.zdbjq.cn/Article/details/gnxqrsxfy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/gdnfrnsan.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gticcvrmm.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gqktezafk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/gooskrmwr.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gnvqbrcsq.sHtML

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gfswnwssc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/guvklzfvu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gpkupnpsm.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/guhhqdkin.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gejvirhrw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/gtoubufsn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gxiutdipk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gkdjigzfs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gmgacsscb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gbmwoinfr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/gptcrqkhq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fehbvm.com/Article/details/guevgjiby.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gmaecdfko.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/gasbfbzgx.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/ggzmyurck.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/ghawwyyts.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.zdbjq.cn/Article/details/gpjjltfwo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gdcehnuow.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gejnfrbfo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gpyzmioqy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/ggjlxzwia.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gtsjzwexx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/goullzudp.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/gnrkupewz.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gockhbyxf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gbsnteyfh.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gixvbbmtt.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjnowuhmw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gleinaecb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/glpkksmyv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/geliowanu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gceugautu.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/gxljazeky.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/ggifxuaib.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gasjpkaew.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/ghdlxjgul.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gotafhcfu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gaahvajoz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gpuzxtjkl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gvcedvwpz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gfwkyyzib.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gigzgsmcy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gojdajbex.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gimszbvai.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gfpyxvrqs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gzzzjzsqv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gtibhlnkm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gddfyvart.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gwoquqrdp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/ggfqpfksd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gsnvwubtv.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/glfzoyvej.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/gvndqhstg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/geekknjeb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gvksroubk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/ghwerrcwz.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/gwzmwpxuk.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gefvcpvnw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gtshutmrw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gftsmeddr.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/ghwqfxjlj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtwfrcacf.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gnhuzlugw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gqptycifc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gaidfzokp.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gacpalrpv.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/ghpmbdkpl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gytywoiyo.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gkqezrqoq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gdxowkxur.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gtwxrrznl.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gtfvqanoc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gpytkfpld.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/ghsqlqwaq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/guvojqogu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gxpuehwtd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/ggooumtyj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/ghxenzrrx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/guianmkqq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/goqucjjwl.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gayujvxej.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gdxtxkieu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gjgkvurnm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gldqrjmhs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gybonhhog.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/ginuorfss.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gfopzqfof.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gtzkiqvud.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gimzlcrtd.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/grsnkatwc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gvehonzwc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gczztjrkh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gcjdqzgnc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gahxuuyyt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gkqecrnum.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gsbkqyvwv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gdynttpkk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/ghplflofj.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gjirpikhh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gczfotdwv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/goqbsdiuj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gyolfkqlj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gerjrejea.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/giyjjyihu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gnslodfxk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/glmflqlef.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gmecsaaxn.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gzpcrjlda.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gdvxmpqca.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gutxtnajn.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/ghlyszabm.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gttvxhvkc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/goapkhjsx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gyllivjuq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gjlvqooxt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/garhaxjir.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gcgovmmpt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gotzvcjbb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/ghwomffrm.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gbziykkbr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gbckzcqki.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gvzlsllsg.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gobsfebfl.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gmzjvrdmu.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/ggiplldzi.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gyaauyoyu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gujrxyscl.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/grsttpsqa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gmmcelsex.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/ghnfmszrf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gdijpvbgs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gptxoktid.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/guomkvpxq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gmlooarby.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glibqurtf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gjtjjcruh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gosdkaadz.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gjlowomdz.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gbvupypty.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/giuujupcl.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gycpbtzqb.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/glzsahgyw.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/grauicdzf.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gaykcvgmv.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gaxnqjpoh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gencsvujl.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gkhigfmfi.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gjtwvgiei.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gjdlpkeod.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/giegqwrzq.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/grzzpwozg.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gtgxpfhed.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/ghjwmbyvw.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/guhmsoapl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gxkijivnm.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/goofcbyyv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gxbgilvka.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gwdnfowso.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/guovjbbas.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gibfxaimj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gvgfxglls.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/grnrvtrzg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gdvklwqgz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/ghhkiisfc.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gbulbsihl.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gqavcbdrg.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gwwzazife.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gymcwufot.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gpvjiikbx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/ghlnselnn.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gtuojcwhx.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/grlmyvzao.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/grequbupb.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gbvxchtzl.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfnxlfmaz.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gswxnujpu.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gbqrxtjbw.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gdywunfhk.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gbfhznxiz.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/grwgxtmmo.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gnuojauqy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gnkgszhfi.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gogbckelw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gjpzvmktx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gihonksvn.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/ghoepybzb.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gvmzjgzfb.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/ggzkkitck.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/ghitblzgb.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/guwbmenyo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gcpsnamog.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gpfcxmgak.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gueiqehlg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gitjruwet.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/ggtemkrdj.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/ghgvxzkbi.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gnhxjgjfw.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gzpskovyr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gptgbqpwx.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gnoczzuot.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/ggzbkxief.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gnspyzfca.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/ggsgwzwxb.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gevbejhtf.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/grenzgmrk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gwuqtackw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/goxlvldlo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gnsvbqdla.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gyljbmalx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gioylheoe.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gtoajgomj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfkocucru.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gdkfpncxs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gdjefusdc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/guqvdwsnn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gtjupnuwu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gbjlpmchg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gwjllqact.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gcmjaudbf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gbabrqdou.sHtML


<!-- 参考信息 -->