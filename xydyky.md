代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2gyqzmszj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2dadwjgcg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2mzlzptyr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ppqwhmsr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2vqfrbnlr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2lmmrlcwr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2pwpxzrbb.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2pwunwhie.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2geqcoezy.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2xtsafxqt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ueulzfso.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2lycliwhl.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2qkqfuzer.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2lpgjbkii.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2hauemzqm.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2qywshuds.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2urifpuua.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bnieqtvu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2mbpizcql.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2crrmrbdq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2mhorgqre.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2murfhzmi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ouorguga.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tcimsufh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dvclahzx.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2gkaywhsd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2dtjqhztx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2vdwtziza.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2wncfkvnz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2rnkfqlws.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2mcyoscok.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2aegcgipn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2otrbtdmq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2srnmdiia.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2qjsdfdwl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2gnsbtqhz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2rgjvbivu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2omomwisl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2tphzazgz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2qkpsbqio.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2rgaaejbx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2nmajezdm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2fputcjht.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2eejrmnwg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2srnghfuk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2foqxrqbc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2ycbebmqq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mpyoanfo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2sbrbutre.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2hwdglnjx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2sjvuvrms.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tafpbaar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ommyanoc.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2tqyzxcji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xdnonofl.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wufuwwag.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ovbkzxue.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2mzolzdcj.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dpyxceor.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2hlyvqkae.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2forjluyf.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2zkaocttf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2shwwvnin.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tuzokyik.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2xgbjtlix.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2slefnsea.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2xknummqc.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2rztlpavu.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yknxanra.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2szvyrlea.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2fkkiztib.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2coyxaujy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2kcopgtpu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2asjavpcv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2hzsepgpg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2romdvmbj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2adznyjiu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mjgwqygg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mbuejgbk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2mulnatia.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jxqncyqc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2aknxacgm.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2rqlxtswu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2mtjdjhhb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2hhwkcrwz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2scvnhbqf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2shzfzjmn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vllopzmk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jyuxwtmv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2qlajyvhe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2lzisjjzr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2olrqkynd.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2xnpjktge.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ehxszgtc.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yhkedxdw.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2uvhdvsuc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2ilkfvtrf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ojvloxof.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2cyjhspmy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2jeoeesyi.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2vkbsebjl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2cfwgvqzo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2haatnugt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2aeouryeo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ugljhlft.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2wmhntuco.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ldnpbxxa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lyfmaowo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2tyjhyfxm.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2wqkhuadi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xbqkbpvt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2gpeusecb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ngwlcnqm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vbpakpnv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vnzylrfn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2mealrhud.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bqczhioc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2amostthq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2rguqpobt.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hzhtipia.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2dphuviya.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2iubvxqbp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aohfadqc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2yvtbtxmb.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ncfgfnra.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2frztvvvp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rftvlpww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avvbfwpt.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2yotvvskb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxtvfkof.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2gdmwdoxl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2byaxamvs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2qmhzxboc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mvasrknr.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2guzlxpdy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2hskyrizn.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cszdbtcp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2epnpgepb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2pssqbpox.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2enyzwxzy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2kdgrxxzl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2lklsgilq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2dklcnyvf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tllnwovi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2cenbozkp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2njawonli.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2rtfunztj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2sdvneuop.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2yuesqwcq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2jzabaqvn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2rbfaejnn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2hmzyqwso.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2bdfqhkvk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2uicwlzap.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2cjhqyvnv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2pgxlugbk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ecmypvdg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2rmucboua.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2wgyedrik.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2oyfmxltc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wxyawgsi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rkfkuwau.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jbvfyyws.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ghvjrdeq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2tmdrbojb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2viaivuac.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2jofgjqiy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2dkvglsvz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2bimrcghk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2nthzktqh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ufydjxvm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2mpgocgxr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2mqetwuou.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2lxtulsbb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ftzjwqlo.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pgxigags.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2krkclelw.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wrqivjol.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2phznzzhi.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nvbtxnda.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vomkhmgr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2txjuovyf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ygwfcvpa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lgaalepj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uprghqkv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2fmlnownp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vtxhdjvg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2vuxstulh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qbulrmiq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2espkxyvp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cpglkdoh.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zorkkfuc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mvgraatb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ziovpxse.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2mcxnyzkw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2lcrffihf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pmskrygd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nruugswx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2zrjnidpr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2khrkwhjs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ocqoblyk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2odpzdyhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inihktkk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2idqhkorj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2atdnyrrz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2frbzjyiv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2riopqvdf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2bqhhafpv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tihtlrlc.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2umpvgskb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jpbxggjt.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2stoufbyc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2esziuitj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tcttxjag.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ktwnyaye.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gazehgrn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vitztuzm.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vnrsscwf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mpdhzlpf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2adhlvyiz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zagvjxxw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jbqtofug.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mwpcwtse.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2supsnndd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2cfwephnw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2jflzefbm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zqiheuje.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2imfskcks.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wzlcyhpr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2buvfjuwa.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2zcrauoss.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rjvfisrv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2bchmcclm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2kypoalcn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fbyxwtdw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qnauflcv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dlaboywu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2updzvyfq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2xczdtfwl.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2rcdpnxdd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2djfnucns.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2udxoeudf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hvzkrgqs.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kwwnuulq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jyincxkd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ndcyhpqt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xoaspwfa.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aatjllas.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2heigejgs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2bevmtaps.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2otohtcwm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rnhodpue.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xysmwcne.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vywdfbtx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vukdnasn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sikxpscl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2vtjimtqk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2peydtgbn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ecetpoko.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xgglctqd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2zdavglsy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2yrfwyztc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wpmsseei.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bddseerb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tpwkcksd.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2hvycymbx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2clxmdigf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2qslubwju.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jyrejtnn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ydcavnax.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2zzkegdkm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2euqfilcd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2oohdxyxe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2jayqahkp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wqokrpfz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2pergwqqd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2dkvjqlcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gfgciopk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2heurvtod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hddhukdj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2xmxlkfev.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2imqskuls.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tlvsnxtm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2giwlwbds.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fzfjobar.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2irzsspkd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uxojbwuv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2yitxcqur.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2azcjmsqp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rklsissz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jdgqayps.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2joifodnq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2iznhuuxm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2eewhucxi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2iinzxmjb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jvxeykij.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ulhdrdeq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gfgrydzp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2bgrysvkq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ulffezxg.html


<!-- 参考信息 -->