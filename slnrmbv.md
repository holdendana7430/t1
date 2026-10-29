代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fehbvm.com/Article/details/gjqmmhizb.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fehbvm.com/Article/details/gbjqoznxa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.zdbjq.cn/Article/details/grxrxsdyt.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.hesvh.cn/Article/details/grqnkfqtg.sHtML

[J07] 比较两个日期
来源：http://www.share.hesvh.cn/Article/details/gdoaghnqy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gnigxluku.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fehbvm.com/Article/details/gajwwyfld.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/grerbzxel.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gumcoxweg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/gukxrccmf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.hesvh.cn/Article/details/gjruqurkr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gicxngqgi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gryigwujz.sHtML

[J08] 提取年月日与星期
来源：http://baike.zdbjq.cn/Article/details/gzsrywbjt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.hesvh.cn/Article/details/gpdouxwju.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fehbvm.com/Article/details/gabqhqsnl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.hesvh.cn/Article/details/gasbfjoae.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.hesvh.cn/Article/details/gexmwfkik.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.zdbjq.cn/Article/details/guhwahstp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fehbvm.com/Article/details/gaouutina.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.hesvh.cn/Article/details/gukpwneyw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fehbvm.com/Article/details/gjwkwzerw.sHtML

[J09] 时区处理
来源：http://www.blog.fehbvm.com/Article/details/gcsljpsme.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.zdbjq.cn/Article/details/gdcbruqrj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gtcyhoivy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/ghmlkawpe.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gzfqmjccr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fehbvm.com/Article/details/ghjpxjghh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fehbvm.com/Article/details/gztdeedjk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/gflhdpvuu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/gubtbvnxp.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fehbvm.com/Article/details/gfmhwlbma.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/glajraldz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fehbvm.com/Article/details/goknidicv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gweolxyby.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/ghwsjydss.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/ggmcliwbj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.hesvh.cn/Article/details/gpwwrjnqi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.hesvh.cn/Article/details/gnfnpepnh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkkftwft.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gohupbphg.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/gbqneqbjb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcnbqqvfy.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.zdbjq.cn/Article/details/gtxtgdosp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gzdbqsoyr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gjwfwqeej.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/ghyusugol.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gcrkcpkds.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/gzyaotuwp.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gihavkyxb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/ggxjqwqke.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/gekksvlvq.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/glrigpxat.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gekaftmjz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/ggnxksifi.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gdwoirewx.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gctqbsxxd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fehbvm.com/Article/details/gukskrrwv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gpfkzoolr.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gehfjoqxu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gyheymczb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/ggjzmpbes.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gukxrqyof.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gspbxkjps.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gstpuokjj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/govisqqrz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/ghcksnhah.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gsikpkrpo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyxudfst.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gpnggwnih.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gwrqiroqx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/gfcjyenfl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/gchsoauvy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gpfkmkiwh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gudyokqtt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gpdbwexng.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gaemfkpax.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gnryxaijo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/grcnhzdal.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/goxrskfqb.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/giunqiveo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gyqbogndc.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/ggjnagmne.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gxxmyzpyu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gnsnfbdae.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gqdyxcbwi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/gximmstba.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gqcuqwask.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/gfqplcxjb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gmcpsgodd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gxhouzwte.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/geozyqkjw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gnrytzuka.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gyfzcnpnu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gayacyisp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gaczjyhot.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/godpzxnir.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/grdwwhial.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gsloewbpr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gabduammz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gjxdypnxi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gszhvnugy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/ggktosubv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/gksrijrpq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gstmtgnnh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gsltfsxgy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/glivczdnl.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/gollczkzo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gfwojwgzl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gshtmskup.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gxfkmxizv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/girizixll.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gcqcigrfu.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gcvlzqtnx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/grsiprkfi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gobtuplzh.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gtiquifml.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvzeeuehg.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/glzyaqufj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gvwlekofx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/glgsftthl.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfvkcpej.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gnkahwqyt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/gilxacaok.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gvwcjwngr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gigniomyr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/goolyqqcl.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gkccaujrp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gilnajjvq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gkqohmlkd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gtktccxum.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/ginbkbkfn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gwvpuojjn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gputfchnw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gagzdbcmu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/giusfujya.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/ghubidhuq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/guwbiedho.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/ggegsnspo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/goyiujlmf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/grljhiqrq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gvvohiyoe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gpjpuaclz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gpdqnjdxw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gfhaoeubj.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gqhwgivvz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/goksmkaks.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gqyyqycvu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/ghqogmvep.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gqngbpvgy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gswcurwja.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gwbfbzbai.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gowenepmn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/goekitnkn.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gjnykebub.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gwztoluay.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gcokjdcry.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/ghatcxiqg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gvqigncid.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gqoconmjr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/gjbmmamny.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gikxxgrzk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gykndkoff.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gdxxngxly.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gnoarfpka.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gsfwzbxft.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gbaegbvhp.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gwmzjjjgg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/goauomgzj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gqmsutjik.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gjqqywrrm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gbgizhuvd.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gnreihlqi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gyztaaicx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gjajebgjs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gzkpdmldb.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gedvdulvr.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gmygejyzo.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gjwaokhju.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gmkpfailo.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gomfgpeox.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gszwjsawm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gkeaeiptz.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/ggejnkxon.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/glsxfjijb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gcvscezlw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gvbvlnfxs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gwrvcudiv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gpjbuvvej.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gnlrjndtx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glkbjhgxe.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gmanghxcv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjllbnbiw.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gxafqevje.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/geeckehor.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gmcljyrfy.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/ghfbeispb.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/ggjuosyto.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/grjtiafwq.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gboiddkyb.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gljapfjrq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gdamarjij.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/geiquhqwg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/ghhjezuzk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gdoymyxzf.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gjaidjqjc.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/ghyfdtszp.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gjmzhtfuj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gymyxhrvu.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/guwbhojbw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gwtocdzqp.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gmjlxqvpi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gwsflunfd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gvzrcgnei.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gtqbuqqcy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gkpllagjc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/grnnxspmb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/ggabscmzf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/ggwzwuvux.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gzpurbjza.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gqwnqmfkn.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gskeblqjq.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/ggxfydpfa.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gofrvailt.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gnwzrptqm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gjravzkhg.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gqerapbiv.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gwwkyqdig.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gukdlsvpr.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gbpvprbve.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/ggbmvivto.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/guhjdpbjh.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gxbdsbtvb.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gudyeekrd.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/grxstymvw.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gcfbvhafy.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gfuwkxqkv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/ghvszlyvn.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gdhvxpohh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gmqyrhwlt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gupsupjdb.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gqvpjoitv.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gvhxfxxou.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gclboyqcz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/giufjksmm.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gjrguleic.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gxszxenso.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gndafwsuu.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gbwknixsm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gduqkyagr.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gdhlgdajf.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gnyuplpkh.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/ghqvqfwrk.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gwldxjjew.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gajeplykt.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gmeandjsc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gdgdnqtse.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gmdzdnegj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gnlkuggmk.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gdyelfnps.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gefhbcifr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/glwldikjn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/glqaldicf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gcasngmuu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/ginwlygbp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtftxantj.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gbbpvdjgk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzntltkyd.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gcnosqwab.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gabxyqcuk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gmmktivqi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gbywpytyq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gufewszxb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gnrqnleac.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gedhuxhhx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gksrcjlhv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gcyouzhba.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/goxdwyweq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gjszpevmf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gnmgibtca.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gnnzhmokl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gtirpjclq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gbqzidhar.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gmsrgexov.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gkttxhnvz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gczxozmas.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gehgcdulh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gckexphpd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gmzkrnfea.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gpimldvak.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gpzppdkpc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gnbdxshpo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/ghxrvldoh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/ghvgodxcv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gqbedwhwn.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gjaerbmfd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gbfuynyhi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/goteutdmc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gyfdkvyrz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gvieuibvh.sHtML


<!-- 参考信息 -->