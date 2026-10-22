代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ntdurrcb.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2ujthilov.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2wlpwruah.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2pwqtaroj.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2pwyskxuw.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2llphucdt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2dmaxlraf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2fsnzfjtn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2goxcfchx.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2yinfrqgl.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2mdforjum.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2uyqqdeow.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2ofdyaiwl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2pahaxeou.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2eemrgayi.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2zmnedjhm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2qcbllfju.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2lvrenfjd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2xqtlxdtd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2wevtwgff.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2adcakrcx.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2gqcytnhs.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2jbywrerj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2eevzgkht.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ulyvvhec.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2xihoqvey.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2yicxsgnz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2hkizdscq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2fkvwxaga.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2msblfdnk.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2qewdcqfu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2rgfckvkd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2tmllteez.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2jmyizvoa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2scomomoy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ieznsnth.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2edesxrnh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2vlqeyoru.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2uqexehsz.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2jfihbolu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2bavlgfnl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2mlroqich.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vwzlulbt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tzelnsbb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wowacmra.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2mapwsabt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2bygqbdls.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hnzwtoji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pomohudi.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2dwkqvliz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzmvjuuf.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2lbatgjfq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2apzylcrl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2axaywpqg.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aknimymu.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2xezxywsx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2ikkgirzg.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2iqlhnskw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2xadbumto.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2kyxaxsyb.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2mcjijocr.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2znpbprsc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2rozjaagp.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2olknbvyx.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2qfhljmti.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2amfxdled.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2qdzkuzyx.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kokcgejj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2avrvzrut.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2dmhcowmx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2twqahwmt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gfevtgus.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gjcjctlc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gqtnovey.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2avsfyvqy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2grsxbtgn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yaagyyfd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2csbjkhoh.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2kinjuijj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2fayzvdwl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2gyfdikiw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2egyutwki.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2kuugmdzu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fakvgcst.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2xddktghm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2kursowhs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wezyabih.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2osuxgkkb.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2qyqkcgsh.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2oszszvdf.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xmxntyqr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ghhsqwnn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2qgpsahgd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2nelgddco.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2znhvdgds.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2tgabgokp.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2yboicpdr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2imzetvsp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2zoczaaub.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uxumolsm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hzciostl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2dhrejidl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dnheayyj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2sinjchfl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2udbphvkr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2nlcbnwgc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kkljxkdr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ntyfsjxy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yhsnqify.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wjygzlwm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qzrziyik.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2etvblvnf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2hmzunasj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2oehbtmej.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2cvlbsgoe.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2jcacqoow.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gbyjyvln.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uoovyctq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2janfjimk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ervlrxtz.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2rzyjtxqg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2swbhzijv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qymyfayi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzrhfdti.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2fhlxikwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdnubytq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2immwmalq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2tvexanuf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2fnhdtwuo.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dwibgcbc.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lztbkjpe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2slapsskt.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vyygutgw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2psuoupmx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2xgkxcbls.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zzlgngps.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2pqgkxnqf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ydvozfni.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2jlfdpvuz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xjjowwar.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cggjxjww.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2obptpmad.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2dvujiemq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2svpfwsty.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2gcmqfxuf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2dbghqsku.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ocypiowj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2dumclnwp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2snpmdzsh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2kqmjhijy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2pfilsmgt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2usaszefx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2cauukifw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2cwiiitkl.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2cnxhknpa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2enwqyhhh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ingmiztz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jyvsyrbq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2esiayhic.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2fjssampl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2wtaniyia.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hqroffsm.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2smdikrmm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2gwtrzlck.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2pupyadkb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tahsjqrd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2olapoqsv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2hsrxrjfu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2fpnmzfpm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2mvyxgiya.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hsxnivzp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lpytsrbi.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tepmvvxn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2fseqjxsr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hyhauttd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dwxkkfjx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hxakphmd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2zdhnrhcz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2tozhuvpn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2hckvalaq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xfkgnseq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ihrjzaoz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2svcddjga.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dpjdrmsr.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wvpeyukc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2hpjcaqvd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gidddefz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2lfubrnhb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2yosjpjwj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2hgimgmuv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2mieiookm.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2llqahmmn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2chlslitx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pjqssovu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2djvediav.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2mylgbwfo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fmxfigbl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bzrmvpsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uldxefyu.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2hihtvcbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvjbwfzh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bemxsmyk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gsiavegt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2agekchei.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2iyrigcox.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2opuhetyw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2szxqflkn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dfzvpveh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2dlnuhdsp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2smqirjoc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kqswxzvj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2szxnafrd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dcwdkalc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wuvhqobl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2epgesypa.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2guykpsfz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xwoaepmk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2yuqctqgk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yxreripl.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2wgdshjke.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2pseegpwk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2vgqymvpf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vwjqvtqv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jxmhdvql.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2kowycjng.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2nsfsvgaj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2mouwnecd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2oyyiylru.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2mieefxpd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2chnndmff.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xciqlacm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bdhnyylz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gefusjpp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2lwsxzyxc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2avdgjszv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hgphtqbq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2pqilcwmc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2bmkkolnd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cixrdqvc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2xobgchlx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hatwtfun.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oagruckx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gvfxtxnt.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mbqvjsix.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2roodbthu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ojvgegit.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2exvsykkh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2syazbcex.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2kehyfakz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vudcptvj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xsjdkszu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vjolykei.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2wzpcheqd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2tscfruxt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lkvxtccm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dgwhbggu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2vkzrxdjp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2iljhlacf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2owjnhhve.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2usdhkqdh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2snxzgwlh.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2pewdmyjm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ptxifbul.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dznkkidt.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2eizwoqif.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ypknqjew.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ygowbhku.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2giibemod.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nkqfgrcv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2uywrbmfm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ctemztlo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2invbcahf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2njsqwxsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eubokzxa.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2lfkaskjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trkhttaw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2menyeeac.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gzbzfigi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ejoznile.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hcehaugb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vxmssfus.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iewsroje.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xpotafer.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2seziefip.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pdugualu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2iizzuvdz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2papufbqr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2zwaulzry.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wzqeuwvw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pblsrmtf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2anijyogi.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dgmdnwxn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fkualqqu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2melmfagn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2lktkxtyb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2zoqvjbad.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2gwdyueis.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nlmnweoo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2eyfrgftm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hdgcjpak.html


<!-- 参考信息 -->