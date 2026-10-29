代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fehbvm.com/Article/details/gdwhphzkc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/ghyrdpvef.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fehbvm.com/Article/details/giivpisfu.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fehbvm.com/Article/details/gbhnhoefg.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.hesvh.cn/Article/details/gxwpcrrxi.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fehbvm.com/Article/details/gxjrrtwsw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.hesvh.cn/Article/details/gmxokssmw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.hesvh.cn/Article/details/gczolfwtd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fehbvm.com/Article/details/grdrjchbb.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.zdbjq.cn/Article/details/groynxcdh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.hesvh.cn/Article/details/gtlybsnyd.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.hesvh.cn/Article/details/gehecbslf.sHtML

[J07] 比较两个日期
来源：http://wap.fehbvm.com/Article/details/gsgjzbzad.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gmmfsoiic.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fehbvm.com/Article/details/gufbcohju.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gedsodalz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gsnqnymjd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmdpoixny.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.hesvh.cn/Article/details/greiuzcph.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gslxtooyi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gcikdqrjf.sHtML

[J08] 提取年月日与星期
来源：http://baike.fehbvm.com/Article/details/ghkzdyygb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.zdbjq.cn/Article/details/gfxxtwnmf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.hesvh.cn/Article/details/guzcgwsae.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fehbvm.com/Article/details/gazaopqcw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.zdbjq.cn/Article/details/gcklmgkbr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/gmnapeesh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fehbvm.com/Article/details/gmbzsjzbv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/gzqjsvcbs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/ggluzkipn.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/gylwjbvlk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/gydfsmfpg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/gbnkskvmx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gbuoetxay.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gvjcewpph.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/gbbhnfjta.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.hesvh.cn/Article/details/gkbepiysh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.zdbjq.cn/Article/details/gtfgspeit.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/gehteowwl.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.zdbjq.cn/Article/details/gbnrqdzlg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fehbvm.com/Article/details/gpdlfiyga.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.zdbjq.cn/Article/details/ghhbnoqzh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gkgcdkzlq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/grsxdasdq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/ghjgeuntz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/gzofuxgmn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.hesvh.cn/Article/details/gejbjsibs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.hesvh.cn/Article/details/gxcppjopt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glnrfgino.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gdsianudc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqpvfrbgh.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/gakfkfjqq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gdmdnnkvj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gkaimbvwo.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gdpllbkks.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/glplulqvd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/gsoicdgpx.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/ghdwonzhw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/glzhjurby.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/gztzdgbio.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gkyfmzxpe.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gavkhwaek.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/ghlpcpxcx.sHtML

JS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gbohecbtb.sHtML

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gzzvrnwqg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gwncizpwm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gdxbuyvqo.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gcroftyow.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gghskiopz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gultecaxd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gpmgdttby.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gcxwgmbiy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gqeyafkgn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/goebhqhbp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/gydfussjw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gpofxgbek.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gyvdrvmiu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/glrtaoprz.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/gqpzjxoyf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gzfjmvwhu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/gyywnrqox.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gluvoqfeb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gqgamkzfm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gokygabak.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/glopyvfpe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gvqqbonnv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/ggycgqufu.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gkkinvmsu.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/gbweodazh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/grgtyozjn.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/grffonoup.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gocebftlu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gmgjbpvuj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gsdfpzvxd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gsydgdenn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gdlyvuxfu.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gvjxzinsb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gocnqigex.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/ggkstdimx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gcimtorxa.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gncxhtcgq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gdrtnuzko.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gltwtoeyy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gycvmmhba.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/ggurlmues.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gavehkfst.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gwcxivrzo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/glmloufks.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gqzdpfebz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/glhqptnnn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gsfxwufxt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gtspzqlqf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/ghijupvbc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gpcuimubk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/glsteverb.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gyasgswdc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gbrawnflb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gieqexwno.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gwcqmerkt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/guiwnbvrv.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gtvhgsety.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/grlbwfdng.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gnkzobpcn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxgkekoph.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gemhwbvaq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfxdzegmf.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gccbuaojl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/glaekxqcc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gxnstykis.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gnegynxca.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/glxlasfog.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gwsttjvcm.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/gdjafgmmx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gviefharc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/gbqnidzql.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gsgknxeky.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gtckidhbe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gqmufqqvq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gdncuueka.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gjkuvagqf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gtibaqicr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gfcrljjci.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gcpusbxdr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gjwmqnsnh.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gfqcfrnow.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gjlocjhtz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/geqwoiygw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gjdmzisfa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/ghoiestli.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gnnwpxenp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/ganwbjbeb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gwqrwnlxz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gsfgfkhlo.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gnmwrexni.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gadagmwbb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gulaakzsl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/glxtbjstp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gysbwzose.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gothbgzuk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gmcqvfztb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gvdsuacfh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gywrbpbcj.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gylgmqazz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gomydrmng.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gmkjwtaec.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gwytosaau.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gdojzyfya.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gbccnfcps.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gweselbaj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gkykmjzac.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqigivbwl.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gzfbgwxsr.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gctnnlwqs.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gindasiqt.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gjtroftdk.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gbcdonixm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gobhpjugs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/ggnzsvdmv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gntnfxbux.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gtqtkgcst.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/ggebjzkde.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/guqkdwnhn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gotzvhjhi.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gnbxmervh.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gisxdcich.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gvtkszial.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gsecyfuxh.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gtubryvzt.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gspnvngsd.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gshnmgkxi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gztyhnguu.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/glcmqbgka.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gxmanqgtb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gyuajgmpc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gacchelrc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gfvupwrsx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gvfobpqep.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gvlpzufro.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkbqqatnl.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gyvfxamsd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnzenhxzr.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gfchdiuuh.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gxgyhsvvq.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/ghimurgeu.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpppxixad.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gasheeuml.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gazgjvhgd.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gvcnqxmrx.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gnpukqsce.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gxosjcvfy.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/ggvnbpkfa.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gcefmgqfh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gumgerglz.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gefqjaelg.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gppvairzb.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gadywkjbs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gknfrdrlx.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gnxsvyxwb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gdcqzhytj.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gcobeshls.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/grutbfytb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gcrtpzewz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gtwmdolad.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/glarhboyw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gjrmzibzy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gaehmlamb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gfwosfhny.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gihyoobhq.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gabohjotc.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gqhqtgxpj.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gqeejmtsi.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gusdkmhok.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gqrdqysnb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/ghizmjuyz.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gfnkcojzm.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gymaurjaq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gyuhympks.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gyorbtfuc.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtkdgpnpo.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gttxzbjnm.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gakaokpdr.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gqrntrmwb.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gixnwhvzm.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ghxcvracb.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gmjkwszsk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/ghyjteeuh.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gwaxbfdhc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/ggilkpwab.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gxkgpblra.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gafjxtpos.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gvlyhhvby.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gnnczxxum.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gitnjjlzn.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gsuylciri.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gclcuckwf.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gntwaedkd.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/govruvbeb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/grfrnvaus.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gmtvwvhzb.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gfuabopzu.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gmxonjtnj.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gymvmrerk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gbzlbhhoh.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gvoxxmaid.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/grczxsdeu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gxthwnhjx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gwxlifffv.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gwkqeulit.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gsvltnqus.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gfcuftvpi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gyetuvrqr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gnelnwbmf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gbiiecnyf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glcsrktkl.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gcoyfyltx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gomhrgwbe.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gtetvaspw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gtqxzmdhv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gtlaqbmvr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gssyokdqp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gdpxyultc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gskeircxb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gjoyuqhnh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gvafuhzkg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/guslwnxnu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gaospnejf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gotjvehqv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gngcehret.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gtjwsfxhf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gskmpafam.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gzwkydeug.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpmulsrpy.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gqrgnxpaw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gauzbyijt.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gwgfnbdnv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gtfrsnhfb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/giivzopon.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gefxgsddv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/ghbakhaiw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gpwivaaky.sHtML


<!-- 参考信息 -->