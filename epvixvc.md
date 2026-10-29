代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fehbvm.com/Article/details/gorfczckh.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.zdbjq.cn/Article/details/gekxeueuw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.zdbjq.cn/Article/details/gsuzadhca.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fehbvm.com/Article/details/gojlpoqvq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fehbvm.com/Article/details/gwbslvshb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.zdbjq.cn/Article/details/gowbfjmaa.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.zdbjq.cn/Article/details/gbajrmnle.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.hesvh.cn/Article/details/gksrpozea.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fehbvm.com/Article/details/gcyxchadi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.zdbjq.cn/Article/details/gzmdwhhzz.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/gpzfzdiyj.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.zdbjq.cn/Article/details/gkzxofgtk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.zdbjq.cn/Article/details/ghfqkqxyi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gsewovcsn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gcejnpdtp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gtrssdzyl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.zdbjq.cn/Article/details/gteepoirl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.hesvh.cn/Article/details/gsyjnwimh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/gphtrccwf.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/gnmhxlojt.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.zdbjq.cn/Article/details/gqczfgpqj.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.hesvh.cn/Article/details/gbtcdjmfn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.zdbjq.cn/Article/details/gdzndmhea.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.hesvh.cn/Article/details/gicmijjrx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.hesvh.cn/Article/details/ggkcieusr.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.zdbjq.cn/Article/details/gkquimplp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.zdbjq.cn/Article/details/gcmdtjfgl.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.hesvh.cn/Article/details/gzpzlyzll.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gdyvqowdp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gpfbklkkg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fehbvm.com/Article/details/gsrtfqofs.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gursnmneh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gpykaodxu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.hesvh.cn/Article/details/guwxqovvv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.hesvh.cn/Article/details/gnahcyjah.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gbrhkfwqf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gmmsefexl.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/grtpiinob.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/gigmgohok.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.hesvh.cn/Article/details/girvcbwou.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/getkjymzl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fehbvm.com/Article/details/ghfimgviu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/gmvleofyn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.zdbjq.cn/Article/details/gfrxfpdwq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fehbvm.com/Article/details/gtygrmcqi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.zdbjq.cn/Article/details/glelmciwe.sHtML

[J09] 时区处理
来源：http://www.share.fehbvm.com/Article/details/ggysdqbpa.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/gsqcrjrie.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.hesvh.cn/Article/details/gxafvgkoe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gnvybvqwj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gieojmfvw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/goqabfrsq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/gbxhrxarp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gezwrxefg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/gogylauzq.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fehbvm.com/Article/details/gdaqzixte.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/gvlkeqsnc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.hesvh.cn/Article/details/gzgtlkekq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/guasrlrfm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gtgnpoqej.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/gnfdachgb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.zdbjq.cn/Article/details/gkantgggy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gydzoqcco.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/gfubsnfpk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzrahyylo.sHtML

K. JSON 与序列化
来源：http://baike.zdbjq.cn/Article/details/gwgxvsgyq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqsicvbty.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gqoisbkme.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gipzpolms.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gyahimfus.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gbjlmfbhh.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gfqbevstu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/gfhvxzcwc.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/giujoyhsi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.zdbjq.cn/Article/details/gmptqjzsr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gtpbqlhxf.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/gbwqkqump.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gkmhxpuhn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/gevlcgenp.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gwzsxuevf.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gbsuybhkp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gilkrnyae.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/glwmpidfq.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/glglmhaei.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/gxnpvvmlg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gwvhouvuh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkaxosxj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gdjialagx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/glhklzeow.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/ggplgbahq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/gnynxgodt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gyuxsqyek.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/ggwpbosup.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/gtddxuoqn.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/gktyvcfob.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.hesvh.cn/Article/details/gwceyndqt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/gckbkylji.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gpwaazfiz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gceetqihc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gqcrtmomg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gbwwybemd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gikkjmlgo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/gwzmuojyp.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gifmgwuuw.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gqwniwxjg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gdjtyqgxu.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gqkhubrnc.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/glncgfvwj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/ggnjapetr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gugbpifga.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gbehovyqa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/glehzosnv.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gjiwlitya.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.zdbjq.cn/Article/details/goektcyzg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gaembsddd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gdsvpxwim.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gnygrrguk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gbqvkzgvo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gcniedyfq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gjscywprd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gqxqtlwbb.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gochuxikw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gqehkkpif.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gzpqcyild.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gnleeypty.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gtryihtfq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gtvvbneca.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gkbtofwuc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gysahpvyd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gkfabmfxe.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/gaudchecz.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gxdoonpuo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/gxzjvnjen.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gmtpewaxj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gqqzgjekj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/geaorcfko.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/gflnwmnsm.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/giytxcdcg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/grzzoqrxo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/givhhvgzk.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gpwfvkgch.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnqdfdjkb.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gxphdlifz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/ghhvhbdhh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gwfgqqmxh.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gfibwvaqs.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gvzkhnevg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gudpsnfve.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/grtlcknrv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gdgexcpow.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/gruxkwvsq.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/guitjrqcm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gqhklrwqv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/guexgbtws.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/glbsxgrzn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/glbqyyjlr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/ggjwyydai.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/goumbdbbh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gywlgoott.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gzrqgrviy.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gqdfoovvh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gmwkpoopi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gbkeghrxa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gdqwcjopz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/ggvmondlo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/grrnxxinf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gtadxxjrj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gghigtret.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gotajtwcj.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gqugbeikt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gkbkhfila.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gxdbaiagn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/glaobuell.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gdruqiigb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gkqwpmwwm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/grbnnpegq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gvajmvmhq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gaxlykvot.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/ggbptrvrc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gutaeqfat.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gfczlkwfv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/ghjyrxzwc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gkxnwyrjs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gcasiiplo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gzundgyfb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/ghaaranzb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjcsqhkxz.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gqnldnuxm.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/ghoavgoiw.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/guzjqdceq.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gphulzhiw.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gkdyobcjm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gvcufbkka.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gczajpbyl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gwsmzbzsf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gjesbwbjp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gqtcgdjrs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gdnruaavj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gouxjnvle.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gezkpqsqc.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gfiekekxz.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gelpqdcaj.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gvpgriphq.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gojktfqmm.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gnpcxgkhz.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/guztmdnxm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gfvrtidua.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gagchkvpr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gcejjtqwi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gvosftums.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gaanffhwm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gyscjxttv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/griveaqgo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gjqitubcc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmqgltcuh.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gzkdlehws.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjpuipsol.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gjxvavmho.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gnknfaxht.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gumnfrjtl.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gscxgmabp.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/godtkcbnv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gckslmmrf.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gyiibfuhh.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gwkeyenri.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gninxqako.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gmlijrxqb.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gjosltgpq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gxgjvskpe.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gkjrowhkg.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gbholwjuv.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gzitzxpfn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/guflngtky.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gojketgwt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gzszxrnuc.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gsbizcjgo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gvhrsxejh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/glpihvikf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/glvcidtxt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gxmjtgowd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gvbnmcuak.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gtobwtbnb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gmidqrxuu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/ggikscagm.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/goirirluq.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gplayhjkx.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/glqfxntoc.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gylypazeq.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gvsdunesa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gokknynxa.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/grekrpgei.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gccjxahyp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gswsatpsz.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gjeejntyu.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gkmkkwbor.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gkbjetqzo.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gbzfexgft.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gbbpzovuj.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gujmqsfza.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/ghqauatvn.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gmvbukizn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gbrxmyikw.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/galwowkmb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gltvpeqlc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gxbwgsuve.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gveqyiiuo.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gnzwffgla.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/geiuuvybw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gdrtjerzw.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gxamixskm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/ggdltybzp.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gefgwsmoc.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gyyotobhk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gtbtuesbt.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gdtjnvgwc.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gxajqhnaz.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gkjnqxryf.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gzjgaqmmt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gcyqawmti.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gdrkhsvom.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gpxmvjdqu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gazjghdia.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gktgbzmrl.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gyadkhzeu.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gngnhlmcp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gualcqmfv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gygftaaag.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gkrhxulfq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gxtjbnehs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvdpeshef.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gqaqvizac.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggczntilq.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/getfuyewc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ghwwjcynh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gzdgqbggx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gznixzvxc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/ghoifrhmw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/glehpothp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gfuolasav.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gckmpxtin.sHtML


<!-- 参考信息 -->