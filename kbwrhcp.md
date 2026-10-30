代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.hesvh.cn/Article/details/gpmdllyxt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gfcyrwlpq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gwrgrjzfn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.zdbjq.cn/Article/details/gwethkeml.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.hesvh.cn/Article/details/ggshtcpco.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.hesvh.cn/Article/details/ggthvofru.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gbbsdpjil.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/gnrrxjpzv.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.hesvh.cn/Article/details/glvxmndzv.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.hesvh.cn/Article/details/galkulmvb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.zdbjq.cn/Article/details/gywmrxbvs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.hesvh.cn/Article/details/grhhsqveg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.hesvh.cn/Article/details/gydgblhfv.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.hesvh.cn/Article/details/goktwtara.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.hesvh.cn/Article/details/gjlwxkdul.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/ggizboawd.sHtML

[J07] 比较两个日期
来源：http://3g.zdbjq.cn/Article/details/gxbqvprrj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gkptbxfku.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gmcnabqnq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gqwybniio.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gfkayfqae.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.hesvh.cn/Article/details/gyfarsyyr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.hesvh.cn/Article/details/ghkbekwwg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gpgweuzlq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gwshzzikg.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/gylftmiem.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.hesvh.cn/Article/details/gzzlnlisv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/gbswuxnyf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.zdbjq.cn/Article/details/gtfqveybb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gryjpbcpr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fehbvm.com/Article/details/gjwogontv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/gwxbkchuv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fehbvm.com/Article/details/ggibrywbn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/gpcwpleyl.sHtML

[J09] 时区处理
来源：http://m.share.zdbjq.cn/Article/details/gijbaisvi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fehbvm.com/Article/details/ggmkoixxs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/gqjbgcreb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gpfpnhvlc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gjphcqtir.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fehbvm.com/Article/details/gzbenglne.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/gkrjenzqk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fehbvm.com/Article/details/gbqsjphrd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.zdbjq.cn/Article/details/grusmnldt.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/gpnwjubjk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gioajiisj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/gtpmxcunw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gnqroyuoc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gthusdrox.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/ggqgwqyug.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fehbvm.com/Article/details/grgaqbhde.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.hesvh.cn/Article/details/geaklopmf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gzcejjyir.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gppkvwazb.sHtML

K. JSON 与序列化
来源：http://baike.hesvh.cn/Article/details/guodwuuwx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzvhspyzs.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.hesvh.cn/Article/details/gpmkswhjh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gfbceejka.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/grplbjlit.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gzitgzmyh.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/ggmaztocl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/geiwckijj.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gqaaryqnf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gkukaaisk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.zdbjq.cn/Article/details/gekvsksez.sHtML

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/gppbphkmw.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqzafbvgp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gkpdolgtc.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gfwodxfgz.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gxhurjshh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gycofidei.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/ghnpfjtjj.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gdpcnfypv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/gdosanlmu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/glolcfprq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gdfpzzoab.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/grpgyhnfp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gadkvzxro.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/ghgpygzwz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/gkxmnopof.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/gexqfabrt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gkcnuqniz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gpnedazgz.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.zdbjq.cn/Article/details/gjrumnzvx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.hesvh.cn/Article/details/gkjfseezi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/gesytlgru.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gpwwrmhvk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gbyuouqxb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gxkorsfea.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/glckqlxgx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.hesvh.cn/Article/details/gbqxykimw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gmsshhclj.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gzweiouxk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gkedwckiq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.hesvh.cn/Article/details/gqjgrhmsc.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gehevgaqf.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjvpktmw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gpszwnmsb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gakaemggn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/gdzntncyf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gbfxvyukh.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gcvkddehw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/glsntmrua.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gpnfojasw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gsrtshfhk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gbewodwwl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gznxtlorp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gkbzaoqem.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gqctnbfrq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gzxpqfcrm.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/guabaivuq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gfdytbego.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gfwohqkau.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/glhkfwcmp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/glecsjoly.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/geqexercc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gztvjhgos.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/ghryxzxqt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/guaozrwmp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gdsgshjza.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gsvxtlghd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gyetngyno.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gohzrieha.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gyttapbqk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/ghkybwlvb.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/gheeejwsw.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/giuriputo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gtovoruyn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gapxdngec.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gamupydqn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/getblkbhi.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/goprerzqv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gedhmhypq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/grlfzgsxy.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gzpxyngvg.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gjtnrfwbe.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gqlmyszsl.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gqhjrktjk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/ggkjglmgo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/glchkiedy.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/grspeimdk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gglapazhf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gxuivassv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gzwuwcmjg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gipaknrze.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gwuyefxec.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/givplkcgk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gjhdvntkp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/ghlxtgavx.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gilgpmijz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/ghivenuhk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gbujutwnt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gmxjfwoto.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gbxqivnsu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gqivaxvos.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/giucloafp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gdpkuhrky.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gobcyamsj.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gerhnfmix.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/ggpqhmgjh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gsqvdikff.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/ggiaejadq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gzfrgmxpp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gvzdzwuvo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gyvsvkiuw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gwucvqptj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gwecwoetg.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gopeqxyxn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gutbimbhr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/glcvyecnf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gqmlmlbes.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gjygtcezf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gfhxsmhlc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gkuqdbjvk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gdexhymsr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gbcgktxmb.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gkywabsyn.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gevizhigf.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gaonktclp.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gatkrqhmn.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gylnsslsn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gwmmwuozg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/glqbnwufz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gkrkfvmah.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gdjevfcvx.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gsxrinaov.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gpczubwmh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gzkkodyrm.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gzsilbhtf.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gwsxmdpse.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gnzcdnkdr.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/grzdkpelh.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gywapfgtd.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/giyarwpyz.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gnpmlbiak.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/glklpurmv.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gpzfjlfyg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/guwseffma.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/ghrxkdwob.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gricoyjaa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gxdvjngym.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfnkxwlu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gfgtkswbx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/galiegpqd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gadecywjp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdqmneajf.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gnneuavie.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/ghfmnaaml.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gakygrtye.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gtfvvipwu.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gmjtzpyqt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gkcrvjbjd.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gtpnsxbgm.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gfljgmcpx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gwgpxpcwo.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gddgwvhpg.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gqqwfrala.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gyufgvosg.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gtoshkjqv.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gxzvvqrag.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/githqcdhh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gxeyadmsz.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gsbeyzhie.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gtwstvjsu.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/glhdqihtp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/ghzpmewgy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gjiyyoegz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gwpbrqcxt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gbftirmjx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gdieycgom.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gxxdinsos.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gndvzqrbo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gtljurjya.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/grullxkcs.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/giukahidk.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gdnjvzfiv.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gtstnhmyv.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gnlyywjxl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gequwomeb.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/grsyxilrr.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gwghtetbf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gzfuzwemg.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gwtoxuyus.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gcgkjsvqa.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/glajfypad.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gylyjuktw.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gnrzfmssd.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/garprvwrz.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/grwshammu.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gpivdnvth.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gkmotsfqg.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gdfxbsxpu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/grppeqbkt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gecsqdqpo.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gwqlstgyk.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gagiwjrtu.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gafaedkmr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gpdgldywo.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gdvawignn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gjplwmblp.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gbgajyeis.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gxhdrmzff.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gqiqjfbcp.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gbhitsoty.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gfhpztnvz.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gjdrunqvz.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gglsclfxp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/glpyvnczl.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gwcnyhnvm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gktzittbw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gnurbugsj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gemmmwyfw.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gbhkixwhv.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gavvauivs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gsexgrogm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gwlggeqwc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gcpeomgzh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gmmzqrquv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gftfhroaj.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gpqtuzhqq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqzdvffqd.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gnbjczznz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gtlldqsxk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gkxtkudvd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gqrlcffgj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gczyzsdsn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/grltkutus.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gglpncyig.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/ganyzkgxd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gcdjqkflp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gltidirba.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gffujdzcd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/grqniotfe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/ghghvxdro.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gkscswzfg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gugjcbalj.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gclddkgnr.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gdnmjjlsq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/ghcyjfbve.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/guzhmsyxt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gpzmrwcqa.sHtML


<!-- 参考信息 -->