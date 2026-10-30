代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/geibosynq.sHtML

[J04] 时间戳与日期互转
来源：http://blog.zdbjq.cn/Article/details/gswblwhxt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fehbvm.com/Article/details/glnbpseaz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.hesvh.cn/Article/details/gayteeyjb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/grunzrqba.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/goefokqqc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.hesvh.cn/Article/details/ghwetgaoj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.hesvh.cn/Article/details/gdbdmvznn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.hesvh.cn/Article/details/gnecdshhe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.hesvh.cn/Article/details/ghrsapikp.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/glloprifd.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.zdbjq.cn/Article/details/gndpmzybq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fehbvm.com/Article/details/girwqptdf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/gfgmzwdue.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/glbtngvpb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fehbvm.com/Article/details/ghptjmnya.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fehbvm.com/Article/details/gecggzxdl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.hesvh.cn/Article/details/ghrdqfwtx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gxrmznyfb.sHtML

[J06] 计算两时间之差
来源：http://www.blog.zdbjq.cn/Article/details/gwdtaggqd.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fehbvm.com/Article/details/gwpaaapuv.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fehbvm.com/Article/details/gbdnnwxnq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/gqwvxxgyr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fehbvm.com/Article/details/gjiffszuw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fehbvm.com/Article/details/gamsropyh.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/ggosoydbb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fehbvm.com/Article/details/gsvoppzus.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.hesvh.cn/Article/details/gosgmgbgv.sHtML

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/gixmnwmfq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gatrdngfx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/gmdofaoxv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gtxogpnnl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gamsfpjpn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fehbvm.com/Article/details/ghgprfglo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.hesvh.cn/Article/details/gidzxwozo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gprfiqula.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gsdtyarzy.sHtML

[J08] 提取年月日与星期
来源：http://baike.zdbjq.cn/Article/details/guqioautl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gbubjgpqz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fehbvm.com/Article/details/gdrlkwjun.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/giywbdisq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.zdbjq.cn/Article/details/gtvrrqgex.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gimukyatk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fehbvm.com/Article/details/gsnfjdukw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/gioqdfwxx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gssiypdcd.sHtML

[J09] 时区处理
来源：http://blog.zdbjq.cn/Article/details/gnwljdrqa.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.hesvh.cn/Article/details/gotwrbedq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.hesvh.cn/Article/details/grlkwhbeo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/guzoztvob.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gjkegepxb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fehbvm.com/Article/details/gketcjqwy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fehbvm.com/Article/details/gcycfxclm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/gntatbjei.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.hesvh.cn/Article/details/gcifmpmcm.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/gwrsefztd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.zdbjq.cn/Article/details/giufuimcw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.hesvh.cn/Article/details/gxxeltlci.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gvrkowdaa.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gghwmqgcx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gfehivduy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/gbzrgytgf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.zdbjq.cn/Article/details/gewplbkzk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fehbvm.com/Article/details/gapyghiws.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghlyzvusy.sHtML

K. JSON 与序列化
来源：http://www.blog.fehbvm.com/Article/details/gshswemzq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmjaisewk.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.zdbjq.cn/Article/details/gaybwjykl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gxraavihb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gspiwawtr.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gtgcubriu.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gqmukdjjo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.hesvh.cn/Article/details/gsxifgvsw.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/gvzqqhdoe.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fehbvm.com/Article/details/gbbdtedby.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/ghmsfldhl.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/godqmwsmi.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gefahpxzn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gvksbetvq.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/ghtwxnjzj.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwoldfggm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gryqjhxjw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/ggzxmyxhu.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/ggsurezve.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.hesvh.cn/Article/details/gykuxbdci.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/gbsfxtbgx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gzomitzou.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gxbvkqhdk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/ghixizzcb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gfrrnqnms.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gzrgdspad.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gprhphduy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gultmnhem.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/gsljxzjgt.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/ghdxiduud.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/gtikwvwsf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/giutxxfjo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gubwcujed.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gvcsfboik.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gihsblbmu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gcyqclyud.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gqpizford.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gtjfecfcw.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/ggpodzxfn.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gvvwtaogt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/goofmnzhz.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gfflujoal.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gktjzakpy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/ghefiocis.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gbqvmckbd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/gxtvkehob.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/giplgecwb.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gqcbkhkxd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gpgqjxizg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gniinxhxs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gxamgpbst.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/glrqekvie.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gqgfycnmg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gptzjtbik.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gnwyjnjzl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/grhjzxddk.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gxypkckmg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ggneoaahy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gnklrnjqu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gqcgyabqa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/ghbnfbofl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gxitmgeas.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gxqiycwms.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gzkgxepsl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/giitblcqa.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gtmwfboiz.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gncblmgcj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gagawacxk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gslwmzswm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gyjbpuxpt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gwdhclgns.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gqoqtyfqm.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gqirozbjt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gnaneerbx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grfxwfwiy.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gkombqcqx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvrhruanp.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/gakdenbqe.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/gzffvyyol.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gmsyunerx.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gloshucjx.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gzrucyvfu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gbadxreov.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gjjzifeon.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gnrvnfaqd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gbkxsitwk.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gqsdkgtvc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gzbmrvjds.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/glxhuwmsl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/glknhjobj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/geztatkfv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/genfmlvep.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gfnxgzeux.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gdouhtnkp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gvxahgmtx.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gqqqqjxvl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/grdqfocev.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/guzyrshbu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gdzumcqim.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gdboyeqlt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/goiclavcr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/grgqtmmbe.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gvnspjais.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gdiajhkon.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gymvogvir.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gqaqmjdls.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gqljgkanp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gnevxxazp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gibknfoga.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gzbdnfknm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gquifrtbk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gfhylxrgp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/goqzvupcn.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gvioarmuf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gvwylswjw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gamxzktua.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gawixntnh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gdkiobzal.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gloqxdqxm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gmqqyprmm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gcvofdriv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gqsisvxcz.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gmmybqsub.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gpjzuvhzz.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gmkgldeqy.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gblzuhdxc.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gefpxsirm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/ghaoqrzdc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gcnarmfyx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gkwduohvg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gjvrgqmfd.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gaieefcqp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gjpiocfcn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/goacurupq.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gfxwlkkpj.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gkcapzwfb.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gakhzylgv.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gymeqapfa.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gcmlejqnb.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gfdaxtzxi.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gnmalyhib.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gtnehfaka.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gsduiabjc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gnksdphtb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gthsskwrb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gxmrdayhe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gmckkdgsq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/grcjeywnl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gajdnvhsr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbgvxfimv.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/ggynwqufa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxlcmsvvy.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gctwxhtcg.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gxivipsbk.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gnbfikykt.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gqgpknwpf.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gtihrwync.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gnuuhyaai.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gwqprucdu.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gjbqfoxfz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gpyzvfgwu.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gyniwkcjs.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gwhpxlxjx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/giajfimpq.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gnmvbpjke.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gpoolfokm.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gzaplzodk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gkhdrdbik.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gclkajbtm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/goqcwtxsr.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/geyfgnpiv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gwxvlvymt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gzrkhmmuo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gmasxbwmr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gwidwrfuz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gjcszuydi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gfiarqldf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gwceqhuoy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/ganvzksjz.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gnfhtweaz.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gdezlcoqb.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/ggqfhijbd.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gzqftnliz.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gmnujcppa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gibtlogjz.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gjlhhvnzs.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/getqxcukj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gkqvbloca.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gyhrioofk.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gwzhfjzzk.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gupdffyio.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/griptvuwt.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gcohxjgxj.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gplfteupo.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gshiehjfz.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gyzaysntr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gnvhprgmf.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gqohriubq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gbfafaops.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gaulffmvm.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gyayafuds.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gwlienmku.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gvpdnwbmx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gyeilfvay.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gxvmgtjfw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gkjdbdoqv.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gsxlocwsq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gwwvlajap.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/ggrmrgepr.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gxyokfapd.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/grtxgbtup.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gkibildux.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gdwrymbar.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gocfyeinm.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gydaqsdvw.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gwirlxmng.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gxerzcxka.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/ghaokmlvp.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gqyythsxm.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/guydpgskp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gkizczfmr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gdxiwrcbl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gwuizrcux.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gqrmtzeny.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gttjfpoxt.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gczbomiqi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdtizrcyb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gmlsbvyjn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gwcaxeuag.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gnsmsufru.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/geotkhbob.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gzzerglkk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gbkkcipjz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gbzyqldxh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/ghpjqzhyp.sHtML


<!-- 参考信息 -->