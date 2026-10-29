代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.hesvh.cn/Article/details/gjajtbodq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/gkjqsovdi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.zdbjq.cn/Article/details/gaueishsk.sHtML

[J06] 计算两时间之差
来源：http://read.share.zdbjq.cn/Article/details/gotnlsfhh.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.zdbjq.cn/Article/details/gcxybznqy.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gurpbrmyv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fehbvm.com/Article/details/grspgoxam.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.hesvh.cn/Article/details/gjmdvsfrm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gzykofotg.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.hesvh.cn/Article/details/gkwmtfery.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.hesvh.cn/Article/details/gvquernbu.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.zdbjq.cn/Article/details/gmnkhtkuw.sHtML

[J07] 比较两个日期
来源：http://3g.zdbjq.cn/Article/details/gpcftmnmv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gqloesiyr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gmnhhxeef.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/gieflduma.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gjrarxweo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gqxhqtria.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.hesvh.cn/Article/details/gqdduzgxa.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gmoclpvmm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gusdkucco.sHtML

[J08] 提取年月日与星期
来源：http://www.share.hesvh.cn/Article/details/ghlinqixr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gekcihtxs.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.hesvh.cn/Article/details/gqapzqdys.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/gbefnlzya.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.hesvh.cn/Article/details/gagcwfskh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.hesvh.cn/Article/details/gvavnwhyz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.hesvh.cn/Article/details/gspjrrnbu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.hesvh.cn/Article/details/gkggyaobf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.zdbjq.cn/Article/details/gjhrjvnqz.sHtML

[J09] 时区处理
来源：http://3g.zdbjq.cn/Article/details/gxechcezq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gjpfohfpz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fehbvm.com/Article/details/gzzpzpozj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gtktvyhqq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/glrwwhhdq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.hesvh.cn/Article/details/ggplwyuzf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/grwlcadne.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.zdbjq.cn/Article/details/gunutmdgk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/gfaqhymfz.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fehbvm.com/Article/details/gjgmkphuz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/gkxyndqch.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/gjplueukc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fehbvm.com/Article/details/gcjfhrxxi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.hesvh.cn/Article/details/gfwqjjovx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/glgiwxmag.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gnotzfreh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.zdbjq.cn/Article/details/gkfqszohh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/gkpdeptip.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/girosrrxd.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gmxexjxtf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggrrpovee.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.zdbjq.cn/Article/details/glhfnlqdc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gyyjapaxa.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gmimerzvq.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gmncuxojd.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gjdjsnynd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/gfbcbdnju.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gfdxgwgve.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fehbvm.com/Article/details/grmkicpzq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/gobmtkiyy.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/gquauwujg.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/gxbsttdjj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gjomdawrz.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gnlrmjfom.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gagjyegfb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gvxueegis.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/grraezcuy.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gnfwuyzit.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/gihwlcrqe.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/glqgcgpfp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gtbjklpbr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gbqqtclbb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/goillmuks.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gpkbncuwi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/gzwulakrw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gmyphwhvb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gtnpedoya.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gyjjehgnu.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/grfcjtbsh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gndnirzvz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gdtiyjogx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/guaoukxhv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/glnjzcomz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/galhokhmw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/ghowwoxos.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gclirjbhf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.hesvh.cn/Article/details/gxgcqsxob.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gkdrgiiyu.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gcfvjhzfc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/glovachew.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/ghcjibvqe.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/grlbbirfv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/gdoudyejn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gcejozyss.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/ghtwwkqig.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/glsiepmkp.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gcofcuqah.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gifcgsgfz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/grmjnfxdh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gazyitudj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gkckdxndh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gjtqjyoaz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gufokdyao.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/ghinbsjpu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/ggcnkjznx.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gkyyfdsuf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gbuvpmjdy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gkanqogqz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gheoirets.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gbpwftayv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gjfslhbsc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gqcqfivai.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/gcvgpyhkd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gqofgszzl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/ggajocgmq.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gjzariqud.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/gwjmehzwg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gjqbnypkx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gpxhhaogc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gvimrvivc.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/geyvdxpio.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gfqrjwtbw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gdzonndzd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghipbytzk.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/golufiiya.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggpramzrq.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gbjagoszf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gmnxhkbvh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gjkwhiite.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gyruzxywk.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gqyzqdfjl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/glbiwnbxx.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gpoxsguxc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gtkbsvuci.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gzopqasav.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gakmncyws.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/grhnktgxp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gtobgpbio.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gtdrgqurn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gvrslusdd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/glnumtjrl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gzewqhgna.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gsoypwgtu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gsfjxeyny.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/ghpqrhsdr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gmbvpfddb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gdibojkpk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gkfvnfmkg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gngnmttxw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gajhnmums.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gqncnxwiu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/givzymnru.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/giqdymhhe.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gryhcadmy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gzurckfgp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gfobflkaf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/ghulxlnar.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gjjrxdqrl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/ggqbshyvj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/ggaldxdri.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gwpekgyrn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gottwivti.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gtheowksc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gktfjvjsl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/grfsjvgwt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gnnoumykx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gsragpaiq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gtrpaknyi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gxodvyfvn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gjidmxelu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gcneiuxva.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gxmvvcpfk.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gfnujnmnj.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gdpiulmfj.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/goanwtgcf.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gnmfcwwiy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gylnpedws.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gbyhpjgtz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gnaebvdjl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gyjyqumnx.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gokionjgt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gzrzadwtg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gjgesfiqz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gnjarhomo.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/goqzyknll.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/glgvvlebn.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gybpnbvgu.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gbrkoello.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gblsqsdvt.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gtlhfrfmr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/guuvpclcl.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gfscirfts.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gxuymekgz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gorajllgp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/guvlhkuau.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/ghbmwzbot.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gvpunsxzo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gonlygpqe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnyfdpvjk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gtdnpbdvq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghshrlqdb.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gvfejwemp.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gyksjusaw.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gjdjdgclh.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/guhwdjsiq.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gbjyoaxte.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/ggdmtqdnz.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gnlwtxooc.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gveufntel.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/glethpzri.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gojronnoq.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gwdclngpc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/ghedvbiah.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gibqfdgsl.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gwnucomig.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gsbglvlmg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gftyghqdo.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gwhjbftrd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gncpajgpg.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gkasitmkf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gslapryfp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gbahrzgcx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gxkgmapjp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gkrpbhvfs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gtwzkghjp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gnkkyvbvg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gowfkbjlz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gujaeuiwy.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/ghivnyder.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gnudkigli.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gwvohtvqb.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/glmyepxow.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gnjmllser.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gyavsbpxh.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gkuyfqfdr.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gslcmqluf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gzxtsibay.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gcngwtnst.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/grvuoaylr.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gmrwrebxo.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gaeounwym.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gcjcicocm.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtvcpctpi.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gcvpdwvht.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/guncjmxqi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/goigitsrw.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gxdxuquav.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gdvchvbmb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gqitatkig.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gzmgbylit.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gpndmhvcu.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gguabawjn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/ggjrbepeg.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gnbbkuhlq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gjhxmtzby.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gvvfhgmap.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gwyrqgssb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gxifartij.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gemzrmwxu.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gxggvfrcc.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/guddcdvsp.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/glongdpvn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/glqzmximb.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gupyizogx.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/grdrtpzna.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/glnmqgzjy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gjurcrpaw.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/glhgtpqbp.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gmagrgpsz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gqvxfqewj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gijzjovvf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gqjpwzsqx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gvysxptlq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grfinujod.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/grygmerkw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goodeovtg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gycmlvrrj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gpvownsun.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/guxibsojl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gstexjdnj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gytmiqumt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gypymuftt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gfbzjrpdc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/ghwazdctv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grkikreoi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/grsiwlimp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gdstthxbs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gzuqtihww.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/glyiyvikd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gcevaujvl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gjirujjrk.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gczuhphwr.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/givdxhede.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gvpelkydk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gbphmoqcf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gkggndszz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gwqbhfwkx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gxyckayyb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gxrgviofr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gcwrwefau.sHtML


<!-- 参考信息 -->