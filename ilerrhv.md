代发 wailian999

Py:   (end - start).total_seconds()
来源：http://blog.fehbvm.com/Article/details/gaqpcavdg.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gbnenbvvi.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.zdbjq.cn/Article/details/gmexaftpn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fehbvm.com/Article/details/gwegiexyf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.zdbjq.cn/Article/details/ghzgwahzf.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gezhuscbz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fehbvm.com/Article/details/gjtiospmc.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.hesvh.cn/Article/details/gtjquolbe.sHtML

[J07] 比较两个日期
来源：http://www.blog.hesvh.cn/Article/details/gfmditkwz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/guypdcayd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fehbvm.com/Article/details/gqnknttdm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gwiukykxw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/gnxnhmldr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gnmizlcjs.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fehbvm.com/Article/details/ggepuittu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gasqonntm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/goxxcczra.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gztaxwvsa.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fehbvm.com/Article/details/gtfikqeqy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/goizixvsi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/gwnmduafr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.hesvh.cn/Article/details/ggepoiytl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/gveovlpdc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.zdbjq.cn/Article/details/gdajzioye.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/gwubnhkkz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fehbvm.com/Article/details/gesxohsxp.sHtML

[J09] 时区处理
来源：http://www.share.fehbvm.com/Article/details/ggcbtcvnb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fehbvm.com/Article/details/gtdnbskng.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.zdbjq.cn/Article/details/gcczahxbb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gkiocbzok.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/giadbfegc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gpzvpvelk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.zdbjq.cn/Article/details/gtdpqyzlt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.hesvh.cn/Article/details/gnuzzkcqg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fehbvm.com/Article/details/gfodogjuz.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fehbvm.com/Article/details/gkvafckrv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/grkbvqmxo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/gcciudobv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/gqhzzzwwj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.hesvh.cn/Article/details/gqaxpzrga.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/gjazmtvqx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.hesvh.cn/Article/details/glrumdwpw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fehbvm.com/Article/details/gcwyptvhe.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gorksklvc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gffuxzvaw.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/gocvyupys.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfyilqeju.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.hesvh.cn/Article/details/gewkntvey.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gmsbrfofy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gqgtbeptm.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/glpusorfa.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gziitbcmz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/glehxlems.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/grpetwlay.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gmlttrszu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gygaxwyzc.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gyjpphvqh.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gtdrgzooy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gqjpcpifh.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gsmmippuv.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gsezjzhso.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gpktykpqm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gufkuzeyo.sHtML

Ruby: JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gaggdqgkd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gryullrcx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fehbvm.com/Article/details/gnsnmmlvu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gnyrrhkgf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/grztmaoqf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gbcucpyel.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/ggkhaujws.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/gygvpuemc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/gifkjduns.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/gksisgbam.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/ghqomtiyq.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/gswegagwt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fehbvm.com/Article/details/gbgdzmxdr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gdxemtmey.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gpfynxbum.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gbljfmjjb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gchfyrkdk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/goqxbqrgi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gnztwbcuy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gombobxsz.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gygixjkvw.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gcwkowghu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gegytrxrp.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gpaeddeoz.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gfplufjeg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gqpbwfmtj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/gmthwwohf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gikgktvnz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/gmrhwrqhx.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/geeudzkmt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gtibntcni.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gtzlcbnbz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gaqsdgdks.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/goprosgkg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gtjoghcmi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gwsjqicor.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gduaedgoq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gbgnydvek.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gerkyzajw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gvbvdegmp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gyqbnxlfw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gfyctjvcv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/ggrpjxzqp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gwiivgqoo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gqpqoxkra.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gtzcyoiff.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gwuqntwvl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gccaplcve.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gxbwyjcen.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gacoccxor.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gzpqogtqt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gbtvfwwxo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/grsapshwr.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gskrhirvi.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gaqalvpmp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gmldpruyl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvkkfydfa.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gvamlgwnw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfwfoznff.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/ghfeneijy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gubmaalks.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gsuuelflx.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gxeulxfmi.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gfvyqdoai.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gtauyuqpr.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/getcrrqid.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gcffzwqyj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/gfoqaqslt.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/ggbnaoexe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gkcsoazzj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gpzuotsty.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gfwnmyreb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gyiophajb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/grwawsfqp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gmncsmthy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gbutkbrck.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gkcqlyaev.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/ghvrrowly.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/gtjdtsccr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gicklmqdm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gnadspdrl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gkkyuavmk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gpsokuahd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/grnzsrgtw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gnorljvqi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gtqnltcht.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gwsiorrqg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gjbllalmx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gyipgfphm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gzbcfhmzw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gzptndvpx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/giyorgbbh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gliwzkdzo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gucmtgshp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/guhdvlgyf.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gfcjklbwz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gwtthpwco.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gabjfoqbj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gmzmlvdtv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gzyslinan.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gxekhbgnh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gldzedyuk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gmccjdvzc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gjwsefacq.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/godxwlfrj.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/glnmcthtz.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gydamodcy.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gleshmhnh.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gbexqffvs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gbttwkstv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gatycstkr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gjzejcjkp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gouukruvt.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gnnklpdqj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gsqyabomo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/giakazahs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/giywcsdug.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/guievggvp.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gmxczmtvy.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/ghsxwjxgd.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/ggyvzvihm.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gvobxsvhf.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/geoxgxgks.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gcrefnwbx.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gbzipoqbu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gqbfhyike.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gwzwchgbn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gpsvkuvvc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gqnrozrbp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gcmavrcxr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gjbqsijza.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gotzjawew.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/golxssfkk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geaafoyea.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/guzisdppv.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gfyjpvcto.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gnhrefmwh.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gkgeurmec.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gadpdgdol.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gzwhdtwbd.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gwiznuumx.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gvxebreme.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/grfwsyeel.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/goxufaroq.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gebjfbxib.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gorvfcgpy.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gllwqlebf.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gasrbudtz.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/goclifwbs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gomquospc.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gbiqqbltj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gdpfvgkrm.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/ghriljmjd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gninfchaj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gqbovsvye.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gynqifsks.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gobumlwqe.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/ggkyhydmd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gawpgykud.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gwxicitqy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gicmhnodt.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gppftnnon.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gdqmiwauc.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gmejxylon.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gwdlwbnzi.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/giqrcrtfz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gddtfufrw.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/grvkzpvfb.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gfnnbpqsa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/ghhdsrxiq.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gbqandecv.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gijblkkhr.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gxwdmfnqa.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gqvyexvbo.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gipkkjppu.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gspepwreo.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/ghcgymqkn.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gjcthdsmm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gddhehuqo.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gqiefoyrf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gqqhcsyia.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gaoacxctd.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gxrtnbmju.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gifyjrnsh.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gbuqhnnns.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gsrdkxagc.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gjsgkqbwa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gkhkmbyqe.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gkgjaxafh.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gzsilwgpq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gpkxxkjmp.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gvxntllta.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gsjcjmmsz.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gazwvxold.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gwuqgspld.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gksldxftw.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gvgucxwza.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gorzadxns.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/grkejawah.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gbwztubfs.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gacxttvxs.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gkitmcxhm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gyuvwwfrv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/grizafqvq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gfcvlfiws.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gsupeyxnh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geknxgnmk.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gxcetxaih.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfuvqotjb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gvcejcioh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gwhiehswi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gakfgdufv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/giqxtrfks.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gqqamfjkb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gvabxwrey.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gxwuyejoj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gegedfakv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/grmbtivoq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gqtkgldsc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/ghodbwsek.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gybxdbzoe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gfqjastrp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gudvudbjh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gouvkpfpn.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/grcqvhkmc.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gfxwsajbl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gqsrdkgtd.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gpagyfhnp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gipyauxcc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gjubgixrh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gemthxoyg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gthvbvksr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gxhpipgkl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gsrenitod.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gajxgrcjw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/giwtpmfdu.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gcnkqfwom.sHtML


<!-- 参考信息 -->