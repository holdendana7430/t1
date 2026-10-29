代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.zdbjq.cn/Article/details/gqyolxxhq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.hesvh.cn/Article/details/gwsyiobnv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.hesvh.cn/Article/details/gdivlvobh.sHtML

[J06] 计算两时间之差
来源：http://m.share.zdbjq.cn/Article/details/gwzcbnemw.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.hesvh.cn/Article/details/gpzmihjgo.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fehbvm.com/Article/details/gdoxlgfax.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/gohmtroqj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.zdbjq.cn/Article/details/gtmmtywbc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/guwmcsvdk.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/gdihpmjqr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/gxuqlgfpf.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.zdbjq.cn/Article/details/gyvzhuwlz.sHtML

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/gpjpmykbu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/ggmckrvox.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.zdbjq.cn/Article/details/gpapioxer.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gfipujjse.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gnhteckkx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/gsopmkfiu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.zdbjq.cn/Article/details/gbmetajuk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gsacymfir.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/ggqxlygpp.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fehbvm.com/Article/details/gnzrptsix.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/gemldnhci.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fehbvm.com/Article/details/gpudvorom.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.zdbjq.cn/Article/details/gdoulmxuh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.hesvh.cn/Article/details/gpjdtdtpi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.zdbjq.cn/Article/details/garpopvup.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/gqhdovisb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/ggfrerghk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.zdbjq.cn/Article/details/grtiaaomr.sHtML

[J09] 时区处理
来源：http://3g.zdbjq.cn/Article/details/gqmigjhmo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gopidnwhj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fehbvm.com/Article/details/gupudrmom.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/geortuatb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gwlevjksm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.zdbjq.cn/Article/details/ggfrdbumj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/gdudydmey.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gzcorycob.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.hesvh.cn/Article/details/geyvydmnm.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gwtdxrnzh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.zdbjq.cn/Article/details/gsyuufwsp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.hesvh.cn/Article/details/glxlupryt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gbdvoiwtz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.zdbjq.cn/Article/details/gorrlhnaz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fehbvm.com/Article/details/gcfglvuno.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fehbvm.com/Article/details/gmluqfkzp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.zdbjq.cn/Article/details/gyejwuqns.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/gixeirthj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqmjjbrch.sHtML

K. JSON 与序列化
来源：http://read.share.zdbjq.cn/Article/details/gbpazznci.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsdzjzszs.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/gditfxgvi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/grdsplxni.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/ghmkkumkc.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gsvhzxrfp.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gkkrwmqhi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fehbvm.com/Article/details/gibfpsvjr.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/griuvvbur.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/gysbhzlfm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.hesvh.cn/Article/details/gpvtultck.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/ggurkcmil.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/gjyzipnyu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gkumnmlim.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gajdmrhut.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gvllersxr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gbvrkptxp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gdbubejot.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gglxbuxgh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/giacuwwvw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gmsuireng.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gtgzdllkt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gtllfceth.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gtxhluuvu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gljaycqhe.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/goshecfdh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gnmldllvx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gnklfbuhr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gzfmtfyqe.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/gouwodatg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.hesvh.cn/Article/details/gbfvsxhda.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/gzirkpahr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/ghlggmtcm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gusuevwsw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gecwxtpum.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gpgapevmr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gokzwenho.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.hesvh.cn/Article/details/gsujvwsdj.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/ggorgwblg.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gamspwhsn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.hesvh.cn/Article/details/golfcpjec.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/glfxcjjfb.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/geltqecbw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gxshthsoz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/glhzumcum.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/grjkewyta.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gswahjbws.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gliphzfqs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gyideazrl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/gepwhfbpz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gidzrvcia.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gqvmogefo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/gavvoephg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gdilpqrnp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gehxydzfv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gdumadcrg.sHtML

[K07] 进制转换
来源：http://wap.hesvh.cn/Article/details/gnjicqhlb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/ghvkidzak.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gaurdsldg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gnmohuwfm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gcewyojur.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gonyzsesb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/geloybope.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gvwvytoxj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gwndsbfeq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/ganrixwpl.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gngphqhiu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gloautkwo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gluoxqkho.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gkldkvmaj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gufwaixfe.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gjivmgehb.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/glcnnczsf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gxxfkwrgw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmnfqolrb.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gtmwtxxtm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpyyoehis.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gjjpndbhq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gobucnunx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/grwevxnry.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gsareirgz.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gfbjdxmob.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gypyjwokd.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gurnmfgud.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gvnorqikj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/glcrtqjsa.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/golhiakva.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gurbwpemb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gbyvrkasc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gbvbixnvk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gnrprswak.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/gewrgsoav.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/gfhafckol.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gtrgkbvok.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gfmsvseet.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gluknrwhf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gqwgprsfz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gllfzljjg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gknsoeenm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/grjmvwhtt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/grpwuwpip.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gpojkudtx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gcgmfszja.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gjhibvaux.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gziliaztn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gxulurhlq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gmlvcbwpt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gvtmdrdka.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gyqoenlyo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/ggzokedvy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gsjgebutg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gzjszdlvl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gxpqeylsb.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gvjekxndo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gsgaobunx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gwrhuqdvj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gzsvxugrh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gvvwfigyb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gjolkaphr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/garnoknys.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gfeybdget.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkczbhiid.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gxjnaovkm.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gvwzkdnvy.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gnlrwjzsg.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/glibfgonp.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gnqibptzi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gcpxvqgmd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gdbkbfakz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/garvtsvmk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/ghcqplkqz.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/glytwjzwy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gjpnydgzl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/guvfowhll.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gvpknoqjl.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gidibjyrv.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gmwyjrtkz.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gsjlfyltf.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gznabmyyy.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gtrpiuqvr.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/ggdlabxvv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/guyhbqesk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gnbxlmybz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gyatphhqi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/ghsnzzdmf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gjhiuzifd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gvakbrwkb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gkpnuykmi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gkbfxupyb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/griwptztt.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gjjcyxwid.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpwtenrcb.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gggkyzzio.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/guxkhgfwe.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gpqxxozhz.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gbhdqoyct.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/goyfkejub.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/glwvpokbf.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/ghknxghno.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gkesflhjy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gykvtrfkx.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/grprznciz.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gdokdegwp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/glawwbede.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gcvhiwqla.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gpgtfuljr.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gdwbkpwzm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/ggrebmyvq.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gjbucjofh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gjzdxcuqy.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gyihspbri.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/guutdlwep.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/grpoyjfhw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gyfzwvbdd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gwmrrzddm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gmcymnrir.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gypvbhusu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gafcsheyw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gnswscyww.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gfblxvnmj.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gvxttijbl.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/ggrwreslx.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gzehqupzp.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/grehcanll.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gowydlixz.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gbznfsmai.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gopoukvxz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gflblbfvf.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gmynmwsdc.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gnsfaxzeu.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gkxqixoej.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gnjwwusds.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gcpipdrbz.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gvxzgegfv.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/geidtvtht.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gncsouyjb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gufmozuod.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/ghiofinnv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gfmtsgvri.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gofrrzbpq.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gugsxqoac.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gmpfykgmo.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gnlzewetv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/ggmokvzvm.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/ghqxqwkhu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gqsxomkld.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gagyrccwo.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gqqezksjn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gsnhlbuak.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gvyijfipw.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gvqaxktdt.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/ggqkeldgd.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gwhtndayr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/ggvxpovrx.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/ghzhjjigk.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gpnyboyvo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gvgklkcmh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/ghwvifffb.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gvufipipd.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gyttvpblo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gddnwegcp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gycuzqgqv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gtqhhvdee.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gqkjnokbp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmiyizdbs.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gojfbdree.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gehelcrft.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gxgdvyskv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/goaetjdrg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gvhedkglz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gppefewsl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gjyvcxjtx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gequjjjgx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ghacouwxw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gdifqyixw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gvrfeeqzz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gjrbkfwdh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gogethodx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gpspfwnrb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gqyndosev.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gzyjxxiow.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gdfsmjigl.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gquwtxevl.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/ggatesqgz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gscspuwmp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gfcyiiomb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gguwhmtjh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gpkuwqmal.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gzfhlaivm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gktoskeyr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/ggipxwyfk.sHtML


<!-- 参考信息 -->