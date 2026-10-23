代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3cwmupblr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3fuifixpn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3vdyzboty.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3mzlvrmrb.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3bcoygwbi.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3szalnfhz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3jslkefze.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3qixtsslr.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3bnzaoito.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3pofdluzu.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3ottsnhac.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3awrkapib.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3pzxtwnyv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3fezcmmyj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3ygplmsjf.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3hfokkcvu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ojjgriqw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3gkjfbmat.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3rduxyhsa.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3umrnvwsv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3dhrtexze.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3losuhqqg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3vnpykwsj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3kkbekxjm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3rswxtlry.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3fdpeurpw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3bypmijww.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3tuqrpgnn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3etcqrgns.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3lrhbeifi.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3qywamwpo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3goncgzkc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3mzocmjta.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3qzqwoyfc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3hwnqnirm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3zdvxsljm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3iftrmedb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ifkoeqzg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3adqjrbhc.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3nwscehcb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3wbioxbsu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3hqumfrsh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lwdommyl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mauilfag.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3zxaflads.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3ukghdyrw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3mrdknnka.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kxsgremu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efgmpvlg.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3kqktirni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oagxmgox.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yxoedhri.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3sdmncglb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gzpnpjmk.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rrlykvqx.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3kqkhkhso.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3zcakbfzs.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cmbsdrel.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3wmroaogd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3fggkhygl.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3axuheask.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3axwfmbqk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3fyzopzit.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pozfolme.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3whorulbc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qcdyzpga.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3bfzjseej.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dsqudwcz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3zwoumcge.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3mkxkcmhq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3kuhyafyv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3sbivhgky.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3nyieuggr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3spocmvok.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3jzwcouze.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3dbwtqyto.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3anxjphvg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3tuihsquc.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3yyzpfcrk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3uxmaeuav.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3chdupdom.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3pciovoth.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3kfuziipc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ofkhsirx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ecjiubii.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3sxuheeto.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3zhkwfpug.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3eitozgda.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yudgsfuq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3gpfjaaoq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3clzftawc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oawotqsu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3zbqjkrmw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3izaaasas.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3qzquakym.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3hfmwabay.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3vrxbognd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wehfmcsd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ugbphvnl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qxahqdst.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xnjxtfhy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3sugfcrzp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3leceqssv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3cmgnadsq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3biowhbqs.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3eqiayvkt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3stysbhhr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3azpvjiaz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iigmpikp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ohjdnlnq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ijbsorot.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3tsbttrum.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xobbirls.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3umsjppzp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3unvuyrqa.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3hveikjoi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3nwqwlhqh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3lzqpxhzc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zafsxbsw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3wdmxlesu.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3hlvboyqv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3poaebbgv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3grqabpon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3leyrujws.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3xmqismbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nazmtnqs.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3mixuclnj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3exzduplh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3aypybzii.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3djpppmvd.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vibfwole.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3lptabddo.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rqnlmfua.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3bcyczhfl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ugdmmgdd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hmdrzeiy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3trujthiw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3bpdfquay.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3mdsdhgbh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3beqdhnrj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3wmexfalb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3iciereey.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3tuearjpn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wmccpmep.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3dfnflqsu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3oyuxemeu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3nyejptxn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3zvadfnaz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tmcdizdd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3hhvqvlsl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ydhcesoa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3hxfdrcpj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3afthjqth.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3balfwooz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3fcjdwwkm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nyzfevnv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3juzorxdo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3agmbfusc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3rmwopwia.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3sbswsnpy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3qubytfsd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3bvsaagdp.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3xaqotfxw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3pwhicmcv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ooxzxcjo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lrtvudwv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jiybtcvc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3cneldscr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3nmypziup.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3nleuuitb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iqzsrtqp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wcibavet.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3grqzyiuu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nwyrxmtb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3utouywjn.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pvrfbbei.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3brodwmqh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3lwqhxfvh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3dwhrhzam.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3shukbdwm.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wmqarwbe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3mdopprey.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hqbfswep.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ocnnkbcm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ihlhbssb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ekxyuxlg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zuijpydt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3kzcsdiyc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ucwuarbd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3qygqcegv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3cshphgok.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3jumqhywa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kcluaexx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3imtbidqa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3xyebbsxc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3rsjdngyb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xiwlsxye.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3nfozzhrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqribeyo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ykrenwae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzgkvzkn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3pirdrkqm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yamvdqjp.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3fhonzyon.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3zifisnwp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eobstzpm.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ouatoprz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3uinfdzls.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3wwhhsdtm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cbdvpcep.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3iqklbpyg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zentjrhh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3amvrejug.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lsedplyn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mypdkbpk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dtekygfa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lnfcmqxt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3sfyhlegh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3phizrvlf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3adlwsitp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3dzapufju.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3bxwrdijr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gifsfsdt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xworijpj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3hzhxkyil.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3lpxbfqvm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3uaqqdljj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3jqjmaodo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3gababtnt.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ankutadr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3kmttkebb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3oyswsgtk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3odbtyuio.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3sssnamiv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3vqtqrvxm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hllnmyzt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3qaundjlc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3vigfodjv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kzxqepkl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3fhaoxyws.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gotkuvcw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wrakcmkv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gleovpsn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3roihxrsn.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3azlmagvp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3tvyghxtz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3rxcbhgha.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vwubzqev.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kzhsdxph.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ontoiost.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3crsacurc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3goipcwsz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3pcdenlko.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3pqlhvsis.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ystyqnaa.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3meewnbrf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3kzefawcc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3gkwkqahf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jfupadza.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wcdzpsrk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rdywmbkm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3uxljdxmr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3xzmzypvl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bhnocwsz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3nthydcvd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3joockbht.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3xulhwvsm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qylvdcmy.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dszimxsc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3fvgqscee.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3cjepaook.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3cyvwgxdd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3vvbwmbmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfrlhrtv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qvuvcjky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hziysrzm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fnqkzkox.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bewxmuok.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rhrfomdl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tkyicmos.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3usqieeju.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xnbjrlfj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jrubrrna.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3shthaxuo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pajrmidp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3nqaaybaq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pytujmjy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fnmsxdsz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fkczevme.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zzisdnkl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3gffpxgae.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wftixvty.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jqsfrlwm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qmgqchfc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ccjsblto.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xpqjnznq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3pzevkpny.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vsvxmntw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ehrqhuac.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3yvlolykx.html


<!-- 参考信息 -->