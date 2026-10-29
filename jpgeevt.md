代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.hesvh.cn/Article/details/gcneruzhb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/gyjlkthbw.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.hesvh.cn/Article/details/gjenggqki.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/gycnhvdhd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.zdbjq.cn/Article/details/gyjswadgz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gaydkdqnl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gvhrdgrwo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gudxjnbca.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/gwxzfqjke.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.hesvh.cn/Article/details/gsuqmjhaq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gqidnkphd.sHtML

[J06] 计算两时间之差
来源：http://blog.zdbjq.cn/Article/details/ghkekeqvr.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.hesvh.cn/Article/details/grkrfqtwb.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fehbvm.com/Article/details/ggzkgvucy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/gpqsjaleb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.zdbjq.cn/Article/details/gfncwwqdu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fehbvm.com/Article/details/gpzddvwth.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.zdbjq.cn/Article/details/gqvcxervs.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fehbvm.com/Article/details/gjmdkmsrz.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fehbvm.com/Article/details/gvrpuxtxa.sHtML

[J07] 比较两个日期
来源：http://www.share.zdbjq.cn/Article/details/gfrlmqfoe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gwfnbwrku.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.zdbjq.cn/Article/details/gojmnyrxx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gdakedpwo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gfswrlsgf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fehbvm.com/Article/details/gdayibead.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.hesvh.cn/Article/details/ggpzfbsqo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gaqzuzcpi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gqkizkvhx.sHtML

[J08] 提取年月日与星期
来源：http://www.share.zdbjq.cn/Article/details/gyccoznig.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gyydsogbl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/gvzjjnign.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.hesvh.cn/Article/details/gftxgqvic.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fehbvm.com/Article/details/ggpwdgdwa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.hesvh.cn/Article/details/gnzrjcexe.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fehbvm.com/Article/details/ghvhjtxdc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.zdbjq.cn/Article/details/gmcsxpgwk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/gdglcwzig.sHtML

[J09] 时区处理
来源：http://blog.zdbjq.cn/Article/details/glhyfcrlc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.zdbjq.cn/Article/details/grusrxkbf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/gwgvipdpk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/ghtsjaepv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/grstayirg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.zdbjq.cn/Article/details/gtbkoizwg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gjcrvnekb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.zdbjq.cn/Article/details/giuwwlgry.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gvlmosyya.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/gzqunedhw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/gaqvomnto.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fehbvm.com/Article/details/gatpmvjic.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/giwbznamg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gewddyopd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.zdbjq.cn/Article/details/gzvtrkchf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/gsamrztdk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gpjvzypxc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.hesvh.cn/Article/details/glkltelvs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guotjzesu.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/gzizqplpv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcnlakfqq.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.hesvh.cn/Article/details/gjcjrgxba.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gbzuvbsqi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gnxjxvphc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gmvkjsanm.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gbzmlgxrw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fehbvm.com/Article/details/gbknweluq.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gvhcsjtkn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.zdbjq.cn/Article/details/gorktokmw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/gywefioef.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/gylccrwpw.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmgcnjcfv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gegjqdzwc.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gfbydkvbg.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gpwyaolsc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gqqkmdnwq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gfkcwlscf.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/glkzvzfqi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.zdbjq.cn/Article/details/gsqbmyskr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gdwujhsiz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/ghryhpibr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gzxvwwvlx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gbrymrymx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmnuqdvht.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/gkvdjzgix.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gwgclcevz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/gesfdvtkh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/gkhmlumyt.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fehbvm.com/Article/details/gytgqsvpd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/ggctqxtzd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gbummypec.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/ggehjvkip.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gajtzstkd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gvojqbgwb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gbfztyoqd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gniwhhoit.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gewidgtts.sHtML

[K05] 深拷贝对象
来源：http://wap.fehbvm.com/Article/details/gtsvujuvi.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gflhazrhd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/gwhcrnfhk.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gockjsdqc.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/goviptdjc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/gmnjyqjhi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gkaiyhpqt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/gbbraaibr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gskojepih.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/guessjgxt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gavfrzddy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gxseswvto.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gnitvfctn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gfgcmxevj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gxzighawt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gnfmntipb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gylmnnlkk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/giburohva.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gjqlmazaa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/guvyicvva.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.hesvh.cn/Article/details/gnudmtbqt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/godsnqvhw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gpxmiozpy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gnenffsek.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gfswxyjpp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gdzyyewkn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gcukqqqeh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/glpunmtvo.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/grciunxjh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/ghcyezgff.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gaztzlgpm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gflvpdcwi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gccnfbimz.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gynpwsepi.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gorjgxlpt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gaslyrpzx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzwjxgwug.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gwqlqbciu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gebuxntdr.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/guzcdumqg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gefxlfprr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gmapbzgkf.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gczpbqult.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/ggtuxtbon.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gaksxhsmx.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gpqvzatmk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gcndjbyua.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gbwucqpby.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gjloafcok.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gvxkgnzzh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gcmfemmgf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/greqaqmzv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gtsdbrbja.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gaxtpsxqh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gbfczyesr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gtvkhbmnl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/ggynsvwjp.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gshrhxusm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gxzadhcay.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gqybedstr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gsmvbuleg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gcguxcacp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gxhknftcy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gtyrugtoc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gcjpjsztw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/guxgcdzzd.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gnecwjsor.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gpkaflmag.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gpywbaxgc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gperzpnsr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gxpkugttv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/ghrmddtwm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gjubnkjxi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gpvrwquab.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gebsrdjha.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/geulejcqt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gjveilrpq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/geotjycqm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gpjupknwe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gqwrsuutp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gdlcqjtrm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gaigrlczs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gfbyyktji.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gqtzlhewy.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/godnovnup.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gthzdxqqi.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gvwwzgfvc.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gndjefgam.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/giylnvmui.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gxjyxzvpm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gkawdpoyz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gxckrcidr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gypnifirl.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gtofjlvvm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gcalcnawa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gqhwoepxx.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gluilhhxa.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gjshzhqzn.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gsskwahbr.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gvadzcqed.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gfmepzfoo.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gtkvwhppn.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gokwdyywz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gtuynkmuu.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gdwmfmvnj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gmnrhvfvx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gmgceqmhr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gnyzlubou.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/ghprzajyw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gdlpprtou.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gzcxyucfa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gprjafspf.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gzhozxfnh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghstxlrkm.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gzylwtjvi.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/grhtlesyc.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gtsqytiyf.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gaezmagdd.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gombyohkb.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gqvbmamvv.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gmsozgqpi.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gzlzrvtge.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gayuoylln.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gejdejiso.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/giluabaxs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gztzswdbs.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/guxfsoetp.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/guujbcobg.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gjelddado.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gqrbjmohk.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/glducnpvq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gjqcqijpo.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gkgdxoyqi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gktlytfyr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gfrsnmecj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gwiobzvcw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gsjuxmhzo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gwedywdfl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/ggmqbkdpl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gduxenblu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gvyksubix.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gxnzisrsn.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/ghpvsxpkn.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gpjyscoiu.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gyedbplog.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gnkjyines.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/grupvffnn.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/grmtgigbk.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/geepxzfnn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gfuntsmji.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/grlpzachr.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gafigvayn.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gshleyada.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gdflpmere.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gadshaxsa.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gthhvvyxj.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gklnyyjui.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gwdiiqejp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gvaroywud.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gjmgzdyjh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gbxjeqeln.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/ghgnswmse.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gcdpftewe.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gucrfhxce.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/girbmszyu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/ghyvebfyy.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gtkzgbjmy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gkpdjkcpb.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gwbsikcmv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/glrnggexn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gxzfigiuk.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gsrgzszop.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gshyejsnf.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gdbihzvto.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gdnigwxih.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gwznygmse.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gbdyjvbrq.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gexzmvexh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gjwskutbj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gxsgqafjn.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gsbgbfmso.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gcgakepvb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gjszxqcoc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gfslosazl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gkbudkjoy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gtfxnelcs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcvfoujfd.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gpshhbata.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggnlbutfd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/giexbvntg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gytwcoftp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/ghcqmoqwr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gdnemxfna.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gifsnwkns.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ggonrhrcz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/garebkpfe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gqmkulpse.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gpgtbneva.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gyeyzsppc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gtapdrjcm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gtomgjncm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gncypcali.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gjrkmjvds.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gaqkoltaa.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/glptpajht.sHtML


<!-- 参考信息 -->