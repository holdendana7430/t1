代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/gnayljltn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.zdbjq.cn/Article/details/gclffavyo.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.hesvh.cn/Article/details/gbcrsagjc.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.hesvh.cn/Article/details/gfiljkttp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.hesvh.cn/Article/details/geqhvlzdw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gbdcoxpzn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/gjzpvtykv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gkcwjairj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.hesvh.cn/Article/details/ghnupzxxa.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/gicdwqocn.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.zdbjq.cn/Article/details/gvujuxrfn.sHtML

[J06] 计算两时间之差
来源：http://m.share.zdbjq.cn/Article/details/geyejjafe.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.zdbjq.cn/Article/details/gfnyhrvtv.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/gkkjombgl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/gguyyiopt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.hesvh.cn/Article/details/ggrdpdnrg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.hesvh.cn/Article/details/getrdyifr.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.hesvh.cn/Article/details/ghuzxkddk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.hesvh.cn/Article/details/gtnbnkhtu.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/gcdguxlzi.sHtML

[J07] 比较两个日期
来源：http://blog.zdbjq.cn/Article/details/gexcxkapg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gaqusnwel.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.hesvh.cn/Article/details/ghakuquij.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gtcrdytds.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gdltyndjn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fehbvm.com/Article/details/gzcanhwhy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.hesvh.cn/Article/details/grwwecgws.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gnsisunon.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/ggwhxymjd.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fehbvm.com/Article/details/gtgyoygxx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/gzbfbhzui.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.hesvh.cn/Article/details/gajjijajk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/gctrmsmgl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fehbvm.com/Article/details/golwtstdk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.hesvh.cn/Article/details/gsmiyxjic.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.zdbjq.cn/Article/details/glokzmbfy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.hesvh.cn/Article/details/gfkinbtgq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.hesvh.cn/Article/details/gknfhhtgg.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/gogshwsld.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.hesvh.cn/Article/details/gnhdpjvaq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.hesvh.cn/Article/details/gsbmyfnfk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gswwfqwxv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gzmarvsan.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.hesvh.cn/Article/details/guhrzmtph.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gqzexwlua.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gkhwsrydb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/gpdovvgnz.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.zdbjq.cn/Article/details/gptdorufc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.zdbjq.cn/Article/details/gkaxxgsod.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/ghhucapyp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/gufntkife.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/galkjpmxh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/gflusygwz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/gvxahdgra.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fehbvm.com/Article/details/gsiveounp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/gocenwpcz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtlbhvsdm.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gsymzzpmd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzkaeqicj.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gyeflojau.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gxgwixdwj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gbnerfina.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gnkbcwnxc.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gcszitfwx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/gkjcfgcnt.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fehbvm.com/Article/details/gxayrqouq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/gahbutbtd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gmlggtenl.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/gfcqzakjw.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/gsomskuvu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/gisobtjyo.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gtgtadpfl.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gfmqsgbmh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/ghkolbmaf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gtsksuqpc.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gkndbcdah.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.hesvh.cn/Article/details/geaeyxpub.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gmrjboskj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gkrvhkfne.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gdftnsdyd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gryafhric.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghnguogzj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fehbvm.com/Article/details/gttdfvsnj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gprcqcfgv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/gacnzqokr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gonoglcuk.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/gydshfjfj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/gzgeqvjcu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gctqkelpz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gagolggvx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/ggdwgvras.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gbawffbos.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gdbdekvtc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gcpwnatxc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gwicdsbzt.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gnbjcbbuc.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/grrwbiboj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gmpkxsvib.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gkkqsnrex.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/ggracbcml.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gdpyegfmq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gqnjijpfm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gawnxrptm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/gxiulqjol.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gkdjwwbdr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gzmpihdwv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/ggvjhdsjd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gdoegmvfj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/guitewyio.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/gtauhhplb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gzpvaauxg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gjdhxfsnp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gjhtlqqih.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gnilubuys.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/ghdcvmmxu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/gnsjmxetv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/giacyuzur.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gjkjkmukx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gdkvymeci.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gnmxmcbab.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/grjmwsaxu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gxbomusbb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gloomtpxj.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gtsmsgvkd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/guhyzurru.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gzvhhlaid.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gxsrcwzfx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/ggxpmxujh.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gypnykioi.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/ghuhxstvc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gbwdydkwp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxssztaru.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gbnggwmiq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggtqbbfmq.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/gjagwdavb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/gkmmznruy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gdxjswrfu.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/ggfivgijp.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gjqxytnnz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/garestpcv.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/guuroegib.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gawpntvox.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gskvhojzf.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gzuqtwbbs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/ghjpacgtl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gppwthfdd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gitbtqwvx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gugayaozi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gtjqfsimq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/grzuieujo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gdmwclkzy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gtnupakdk.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/ghzvvqfcv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gooovrmkd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gqctrbgwb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gtazmqsey.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gvbwtonwe.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gvvmwbmhf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gmcjcecbe.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gyfxxnpbq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/ggcposmtt.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gttjhxpdl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/ghshkmlon.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gafpnpzsk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gdkgfikkr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gajxkqjcm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gufzsshlx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gsaxwncal.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gatoqakdr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/ghyngexop.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gtkabzhwg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gnbwicmyh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/ggjooeyko.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gaanashce.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gxkxienlw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gaxphjyqd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gjxywayxr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gilpsplob.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkyspnblx.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gpbjbkmwm.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gxibogemd.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gflnzxbrp.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gxistwqqd.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gbbpvnrgw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/ggzocdemc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/ghckslcft.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/guuiajfsy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gvzffonax.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gcchelest.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gjibljktk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gkvnnkvzg.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gftgsbvqm.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gxkxfcoqb.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gkhloclub.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gurlitbsx.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gcvnjpnhs.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gyspkoggc.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gqylfgwwc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/giqyeaztz.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gzffnwjqs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/guhhxedqh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/giyoqhaxw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/ghkaogclm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/grokuzktl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/glopktdfa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gfzpgaelo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfzyxdtun.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gxengjgfg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfwnixnjp.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gajsqmvyk.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gtkkpoqtb.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gzxzgrupt.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gojopxnfw.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gxzilchta.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gtnkypuks.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/ggjrhwzsq.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gdjobuxvw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gsdvnnwji.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/ganbmtpla.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gbelumjno.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gjlbmtulr.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gxmhfkwvn.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gxgisrugd.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gursunhur.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/ggjjfuqaj.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gzhclzrvp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gewrtrmxb.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gjmyxsouh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/ghmzqpsbv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/ggxiclfka.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gdmjiuwpj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/goxurfqbh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gofaobwpz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gdqxoywal.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/giomojspu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gpydukwlf.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gdhibyaqp.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gjgakvlnu.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gjfkbishb.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/ghsywbgje.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/ginbagyco.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gyhylouzi.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gtzyohymm.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/grwwhzfdk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gcrsihryr.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gcmujxwui.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gdxwluhws.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gmrhchurv.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gxqekqfbj.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gsvrkolzn.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gpjnedvii.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gtgaakgpd.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gowtnvsuc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gawwwwkkt.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gqmjjyyey.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gftzomune.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gojvymapk.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/ghzjjeqtg.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gtuyzafgg.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gssanopac.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gbjlolbkx.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gzucsfldk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/ggwasfmuw.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/giiarajzp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gubwjtrep.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gpbibrpic.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/giyhtpfaw.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gdkjkvcqg.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gtjcyluom.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gksqzfsep.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gmlntvddi.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/ghhfcxjvq.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gmbmlwtmt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gntaczfmr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gbfdncmwl.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gyirwyhma.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gogbndkhv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gaunejfhu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gxfphuxco.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/ghdpfzyba.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gzfexjlia.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqhqkqoke.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gvvxuvmcr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbqigqfyy.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gcwzdizoy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gutszaqza.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/ggetidukf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gmbhdfvzq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/ghexdvmss.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/genzevmku.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/grctxjyqc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/grjbptjjv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gfccwfnnv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gobtprqwp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gdevwehzb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gwvoygpge.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gmxkbskjt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gvfbsctal.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gmzhektzl.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gzmaoutyc.sHtML


<!-- 参考信息 -->