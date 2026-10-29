代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.hesvh.cn/Article/details/gwsfoerro.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gjuejudrt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gpaivekmg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/gpaixonnk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/gqzcgsolu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/giglymrrf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gvrtmtadr.sHtML

[J06] 计算两时间之差
来源：http://wap.hesvh.cn/Article/details/gdluykwwd.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fehbvm.com/Article/details/gmutgqvpd.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fehbvm.com/Article/details/gphkjinev.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.zdbjq.cn/Article/details/gxuyjaujx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.zdbjq.cn/Article/details/gfmmncahj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.zdbjq.cn/Article/details/gcerfbtyc.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fehbvm.com/Article/details/gicpfxepw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fehbvm.com/Article/details/gbjjbwfjd.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.zdbjq.cn/Article/details/gzcorvbzw.sHtML

[J07] 比较两个日期
来源：http://m.share.zdbjq.cn/Article/details/gtnmlsyjx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gvurudwue.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.zdbjq.cn/Article/details/gwqbstchd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gquedxxfp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gzufcwmjx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.hesvh.cn/Article/details/gksvepxdk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/gosuuiqch.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gftzandzk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gfvfvpmpi.sHtML

[J08] 提取年月日与星期
来源：http://wap.hesvh.cn/Article/details/gutfzdkcx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/grxvqoksy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.zdbjq.cn/Article/details/gkmwltihc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.zdbjq.cn/Article/details/gadewwrnt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.zdbjq.cn/Article/details/gvgitngdk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/grpxfyysc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fehbvm.com/Article/details/gxamkwepy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fehbvm.com/Article/details/gavxeaebf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/gjakybtgo.sHtML

[J09] 时区处理
来源：http://3g.zdbjq.cn/Article/details/gobyvjnjp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/gobyhymws.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gqlepflrv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gjhbqabaa.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/guwhkfiwp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fehbvm.com/Article/details/gtkbkvyrc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/gkfdvmmgw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/gaxcvfiek.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/genwrfztr.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.hesvh.cn/Article/details/gjcdjqfdt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/ggfitnihp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.hesvh.cn/Article/details/gkjogoixx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.hesvh.cn/Article/details/gaxafwaid.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/gehyvwnbp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.hesvh.cn/Article/details/gwxhpfzfb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/gtlovkiwp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gwqkbdxhh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fehbvm.com/Article/details/gnjblkqmg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqjnogkwg.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gxzjimkjq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gotyjssix.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/gnfzskyyb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gitmbfezn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gvvhynbou.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gqblncuxh.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gkndktdac.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gprhnarab.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gjqeyobhg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fehbvm.com/Article/details/gmivbegzh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gzjczkjdh.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.hesvh.cn/Article/details/gxjmvjjhs.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gjmeldbty.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/geitvoysa.sHtML

JS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gozljkufu.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/ghmouyoht.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gwglbgbdk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gihkebxhf.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdxypncdu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gbhtpjfhu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gmzthsvej.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gpxyecfxj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gnddwctci.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwskjirbk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gloofrklg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/gbgnipqum.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/genvjtcdy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gnqlvkyhx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/grzkekdub.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gifrziusd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/gabphceub.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gjujoidmt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gwkrpkwrm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gcryuqyqx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gewchqvbj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gdvhguhpz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gkyxgefdl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gqkhhklzg.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gdovyviua.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/gmcgajsfo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gfbbjmsuc.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gnyjmkfjc.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/glesonugc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gpdyffqih.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/gswritqiv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/glnctjkdd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fehbvm.com/Article/details/gopxkpoql.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/gegvckaht.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/gkytcwfuk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gwmyqfjvp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gmmsgzyug.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gziwjavlg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gengtbcae.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gfxxgeydj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gqhtdmwem.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gxmtkpkrb.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gqfaqefnl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/ghxndgrlf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gqujixvhc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gjyaldtci.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gneicoopn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gedlsuzrv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gyyagyiyw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gbokvmiwk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gckrsglsb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gawmnpuaf.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gqsdruwtt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/gxmzajkhx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gjgccklwo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gamvvytwn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gdwnrkgaa.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gufiibdnl.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/gwjuxxooq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gwnqituld.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gaqzgvmqb.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gcjscamys.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyijtqcgh.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gxodbdyfm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gepdnlbrb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gqozrdugg.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gbfjneald.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gefgieyvg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gthvjcjqg.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gpcfngwor.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.zdbjq.cn/Article/details/gjlowckoq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/guabnyyov.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gyuzhvghy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gpdfyfxoz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gyrbaqlyv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gbrtjgkel.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/ghyjzqzym.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/gkrprkrmx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gisayqvdn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gucicytef.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gyveeyuhu.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gfiyuzdkp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gikuxjolh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gmqosevuq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gbyniukcn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/grxzrblcj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gbybjmqvj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gnzpmmjbb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gzmeedpnj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gnpbnncve.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gnruhxycy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gsgymsvgu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gmgthflig.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/guksutibu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/grorqphij.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gpmuaavzf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gavaafavt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gzeixdrfz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/grrsmroco.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gmhqyqesu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gpkqfnqic.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gwsynhwty.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gdkemyoiz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gsqopxkjn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gywabywia.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gakturoac.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/grwbphnur.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gxgllhmpg.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gvjkgaxzy.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gqiwsiueu.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gwfmpgpdf.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gxidyiwiv.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gitgslfjh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gjhuumubw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gicrfuogw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtrnofot.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gldrmneis.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/glcokdlok.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/ghqjnqrnf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gbmdmjbsy.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gbqtmcxdo.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gxlzvwftf.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gmtixvpbb.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gsuewoekb.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/gnyldhjwb.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gfwlilmjk.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gostoffgw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/grinjarek.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/grhookrye.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gcmolkqoi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gsiwdwosk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gqudxqzew.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gqrrhzhio.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gebaejgve.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gnukzppzi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfwjctsgr.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gaddehrap.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnfbtwjqs.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/ggvuiypne.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gmqpjnreq.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gkzxvrock.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gjhmgqqcc.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gwylpvpoz.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/godplairz.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gmhgzxela.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gxwhxvezj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/glqemuekc.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gkzlgadxa.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/geosznuvj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gedxxpubc.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gwsalkeyr.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gvbjcqfhr.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gfxzpbdnp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gvnblnrnj.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gonyywott.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gqlarpskv.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gvsmezpgc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/guimaphcd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gzxhtqslc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gncsqfdpw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gfycqqryu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gbgtwkndz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gbvpotzkf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gfpqqzmfx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/glgmliukr.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gdjuqtrpj.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gknwgoxig.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/giegurbil.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gzcjibosx.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/goelzrxiv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/guhdkurnl.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gpeibaosa.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gyxllewdq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gpngsjziv.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gqoyhtwgu.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gpfsrroop.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gakzgaduj.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gtrzgzzzi.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gfyltgsvk.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gysajovhg.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gkpnfmdvn.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gxeazhlqd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/ghjrhinek.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gwmjnmrsk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/glnhjramb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gvhlgivpe.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gjxiinbvc.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/glfygysay.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gmrggrcpp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/grvfjuzbp.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gukgvchpo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/ghzrbwzpn.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gqgsfkcwf.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gsfubrmay.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gveytzelv.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gadoxdokw.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gvliaixet.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gphotizct.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gtdpcmozc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gclihxghd.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/guonkjsxt.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gdpttdywm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gfuhdcgew.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gthrizvfa.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gbtbfytup.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gonienmcv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gbjyirhov.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gzclslyuc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gplxmgjvf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/grdffczja.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gumtscadb.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gyrtnsrqx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gljcjgezq.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gjcdzkzol.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gjhdhrrdf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gcegcltke.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gmnookakp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/goclctoxo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gmrogotmd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gshuwpxoz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gjwsocoil.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/genkvtxwz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/glcmvcdxs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/giznwtkdj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gyrqpyjws.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gkbkcdesd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gpqzdwpss.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gyrgnousz.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/goreyhtwh.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gpjnecaeq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gegvnnfhj.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gixlmnjbb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gdsuwoher.sHtML


<!-- 参考信息 -->