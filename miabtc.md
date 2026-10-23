代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jktfboob.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3aaplkcrg.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3ngvjfylx.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3aljvoqoe.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3ldiiwyji.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3cqkhtykt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ddplfopx.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3xqfncffg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3ewbzseoo.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3spqfdsgs.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3rqtadbrv.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3vlyymwko.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ztliefju.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3nwiozeoj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3jkxyhtja.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3mabpybax.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3lggzvcgl.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3ssvnvvru.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3kxxryuom.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3mhvqdmyy.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3kajxzizg.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3lgixtltl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3njhdndpz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3qkfdmbwt.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3yqwmgvsm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3wxixeuud.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3hcgdzbam.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3girgtppd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3padhlnpn.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3waphawja.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3egsyofzx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3uoisosbe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3rkutwcmk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3kvubhnbm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3nqdlbbre.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3xczgyjqz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3jvyeljne.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3xguctsvn.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3puzstgrm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3bkyqmhkb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3yuqtziqh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3iksyljwe.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ospelfdk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3lrjnqtql.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3ljsuqpzd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ymriglgp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3mihsslnr.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3bzkraaim.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3cngyypfb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3pjfoxjux.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kqjtxktz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zsrfmyrs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jifyvgms.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3ulskuuha.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3mfwdmvkl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3vkpnrqrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ankcjsuc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3oeenxlyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqutjhnv.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3agweuwns.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3yonatenq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3burxluyj.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3tvjamort.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3roevtkgj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3kjvqrdgy.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3htfzinex.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3xvltgbif.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zffwmhfj.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3jttlhgmf.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dphrmwdi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3dnayvhdv.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vhdquhqv.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zmvzagud.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kyidulvo.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ydcwecmi.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nkanxorj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3mehztwox.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3ogjuzqqg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3nkgmtklh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3uahheunw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3pwpboonh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nycsrawy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pctoqsoj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3smteobse.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ahqishug.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3gxzpdyfw.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3fbroqfvd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dfdpvgrw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ccxislnl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3hkhyxfum.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mfvkfmjh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tijhxhjg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3clxlpmrq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3osijqdkg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3hxvmfuer.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3kodkdixb.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3nbncwspt.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3zockfeah.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fpafdnvh.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rptjzdyg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3iblxxkwv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3pkooavpp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3jgekfjos.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3rrnoruht.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3tmhvdvnh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3rnhcnaru.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3vsfzntbt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iaqcrgah.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qsndalcp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tohacckz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3apvmubgn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ikmlvnbl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3avfdqorq.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ysmukwiu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cfkjndyg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3wvcwumjw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ankfqguw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mmmefzcb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pdwhxgie.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3blxboclt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3hmmjrulf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kudhnppj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ddctrmnb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jjcylzat.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yqbuvfoc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nurqjiuh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3tjysyocn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3gplwowut.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3erjbtkgb.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ewnwxkug.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3bhmfzajl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jroaeqdq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3wtznlrvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vikduzza.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3qitebcmf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3hdqunjgv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3vppyfmoy.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3lwymzbzw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vsjdhuob.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3zdoqurtx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gmejucdb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3vtmvmpfn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3mgifypma.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vnzalziy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3wxtckvxb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3hksxeygu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3eeoeijbh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3sdojycxr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3eowjunnk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ncuoyjwi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3uymjfchj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3soexrlrd.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3binqsrfo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3zubtvnyr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3hbzsvmpd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ziwnztrp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3cbrrplkq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3dvtnfgmp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3braxvrwt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3katcqpoi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cpsofdta.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3iazarrbm.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3tiguuvlm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qpklnnju.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3rlodjiuw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zuwuzoph.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3havzvrjv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3irmfjwqo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3alacuyjh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3zgmazpbz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ewndcpzq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3euuiolfl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3bumcfeoz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3valnbepn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hwshuxng.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3urbyaejj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3civqamkd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3aosblbvs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aiajkvkn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3moyelhma.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kuutsoue.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fnxptvsf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hviisjoy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3grelnumr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3iygapyvb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3auikdcth.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3amdntrhq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3nwctxhiw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3alrkxhmu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3kmsbgvhc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lynzmhwk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wsmcjxyr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qvvqqrzr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3yosinmer.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3piwotscn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3dafklcfz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3obaclnmb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3cegiebme.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3uvuhplvh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3hxemkmyg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mjhuwxqm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3besdhwpj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3dobficgf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ryudehyz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3eduedikt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ywgqigqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iidnvskh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3vmcxnxgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eoqjvwpn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dmqtpjmj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pzieeuhc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ingpbfco.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pzswbpkv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ktjxfyxi.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bhitunlu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3aaxzfler.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3uvtyltid.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bxeyyuqi.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hdccflzc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hjfppnwg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zjhdlqjf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3yainglfd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ywjxuszn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tksejavc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ujrvyvax.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nhgdhrxi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cbdmeuxz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3slmqcwrm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dtgbhckp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3nyuwsscq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3azrkhsaz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xdkprcee.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3axngsxjx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3isntgagg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ktpzrkdw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ywmbppso.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3txnnviid.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3eecgiahj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3klapdlub.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mnilkqtt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gqycovbw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qstlwsju.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tqwcdcva.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3pujlmxrp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ntnmakha.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ixzlizlz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmkeqtbg.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jbtgpzbt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hraikqzy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bemlcolo.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3umxfxrrl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tcbpudhx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3zsjhwmas.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3owfyopds.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3fsrvevbr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dgaczdkm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dpidmjcv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xkcchlzx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3utekkskg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hrmagjkg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3kltdcqdk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3bfpcmmhr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jhljdykd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3lkezayif.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jfsyrcli.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3dierlecr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lhjznunc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dtjwqzgj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ammjgcea.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3naomxuvo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qqcgmoyo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3zbpublnm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3kyobdhcy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3krxudmzx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3luyhxpek.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gipcpovm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wbgxzawn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3juhbmvts.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3mnlrnerb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3xghxpedf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3aobpphna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gztaqbfx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3pfiikbcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqrjmlsf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3maxtycsx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3azrkcdci.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mnxnuuwp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pexkbght.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wmgqucjl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kvoyzwdh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3opkraldg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3txviaras.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ujiidrpq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3hheaisnn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3yyrykknw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vodkzuqi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mltgdyju.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qnzwsifp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cbxsjlbs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mwtkezqi.html


<!-- 参考信息 -->