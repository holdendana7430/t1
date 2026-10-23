代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3wlsfgrgk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3lrarkvbg.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3xtlwrdpy.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3tirnalin.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3jwqkoxcy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3htqwhxaf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3kigdflob.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3mvcbzjjk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bidnszxr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3aslcxoyy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3rrvkbtoa.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3sgxzfhzw.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3numowhqo.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3inqpkrbf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3aybgdapz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3mudpbqag.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ohqvmkec.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3ectlfoap.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3xkmfdvhx.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3kzephvlx.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3lxpqunbp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ozknumfj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3dvhnkzpo.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3cramvzzt.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3zbupdszt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3qncuvvwu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3wpcfwfin.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ycwfejxp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3sgpauzcv.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3zgyqhgnu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3xpttoyqk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3fwxoqaxq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3grvrxkff.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3drisdcfb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3vpioegpx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3rbveoick.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3lrbsxpur.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3seujdtyr.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3dzgrnlfl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3juxjjged.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3uxtwzecu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3dovgupey.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3vzsrncwc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3nekpkpie.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3mrcterna.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3kpijmjdr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3odtzvtzr.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3dnmqjbbu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3worordxa.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3eofouxqd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ykcdlmaw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bvlfdsmo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nuittmuv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3rvstkyjt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3qaumzkvl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nmlawuyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htiygwjp.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3sdbjytns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3psjowwof.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rifvbmri.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3xnqnizse.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3clotxmgn.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3biybodlq.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bfgwamvz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3zadxrojk.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3suowgjua.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3gzrnxxem.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3qfmjfikt.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3rytmzxhz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bivamqzh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3hqrhyxel.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ossfvosb.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gdqiyfom.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mixpuyjp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3cvgflncy.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zakscjce.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3flxxwelx.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3frnawtjy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3vxafauil.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3lrswshvd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dvdfvlsc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ahfifhyb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3jpmcslat.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3nclzmfkr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dnsiiqiy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3hhdutsgo.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3lhijkmwq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fojpzmss.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3vacxwkfr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hndncnjl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3kprecltm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zhuoxmov.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3qbchobqy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3lywhxgzk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3zwptthdu.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3yvvfhgxu.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qhcxcvbj.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3tcbwiugk.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3cawgjzyy.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ythnqaef.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3vfnsktzy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3eyeigplm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qbrucpvk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3wvypslla.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3cywwzwnj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3inyuzyia.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3njdsdomt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xthrtsmi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3spkrotpt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3apnotmrl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nbfbodhj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3culfhprf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dvxmwuzo.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3wwtylqxo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gaviklxl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3abdgphgw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fpfqxxaf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rndtkdig.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ahppuisv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3updruhaf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3loawvfla.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fvyovspc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3wkskjdvn.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3adkjcztd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3twclocrl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3iyjwawyg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ulwcnpvx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3lpddvffz.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3oqmtttvl.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vwvrcxnw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jmwaesoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfkcvjwd.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3sqhmnckm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ctwxzhcx.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3jkfynyaf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3zdpkefjh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3xaicujtl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3njjmolkt.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ejdycree.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3hbckqwxg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nquahtqa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3puwsdkhm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rjhndizi.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3bcfgkvgi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3uwaauqnc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3hwozsnbs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3bensxopi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3zkrqiehq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3lamljmgs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3xcpfunct.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ievaabft.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gkvwyfxt.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3jhxewmbj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ylltbrvi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3apkwsrva.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xzrdcunw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bxyoicge.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ibquxzjr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3uarjtrki.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3fzelwkkv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3tvpubyoe.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3rjzausnn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3naxdkcdb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3hqquaxjl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3voxihpav.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3oobmpcfh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jjktbxui.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3hvplyuap.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3otlereva.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3gvwkrtld.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3kcuxkrhd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3rtjdepoe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3jcmpuqlt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3mpwxnxpk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dbevgvtu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3hruryocm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3zpvjkqnk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3lpjkiigs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wipjrjoh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3kysqihyj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wedkxbmy.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3nsgoikfj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tyayjakp.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wadqbuwd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wvfzcqjp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3rifmjipc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3oewhjpjp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3svbprhlk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vlbvzcvm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3piizzsgz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3cuikyudo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rifsievc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cepttrvb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3bzdayfjo.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dscwqhne.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3fmtjtlzt.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3dequmsqw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3icqqbfka.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mavqxuyp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3bxhrtiwp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3oxqafagd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ifisjkef.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3dfoicdph.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3dulzbgts.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3poupnrgj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3nyvkejbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tiosoirt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3lfcwjkfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azllshda.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3iqbudvpe.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xxyrvwwq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3nkbfosjq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tezztqpy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mfbpsbun.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wybaahqc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3kjglkhhh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3etcwbcba.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3sshzjlni.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yslolrrn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kqkgidai.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3otyhgpoj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mgrxibxx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zmeirrrf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vqlashvu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tspbjxil.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3wxqdttiv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pidrowfo.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xaxiirrk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wldsheyr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3nsaiwkww.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3utwfqzlo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cwfovsud.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3idpoketn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3hbzreyed.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ombhdygx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ayotapdp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3osaeopnh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xybkphqo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3glsdknmw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sxkcvfvo.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ldtzfjjl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wjzdqxpz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3lakvoyoo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3hcvfdikq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3bvwogiwe.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xijmtxed.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xamutfvc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3lshyydnk.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nyjaiszj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfxhkeoj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ojdwacbc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ntbdexcb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kgugouwz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3wwsgendg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ovacrhjh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3eknukrfc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cxbvhxfm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lwwfmegm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zyuhmzrl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vfbhsrxo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ldkdxcwx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3xjdckxbu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ukexxyik.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ktaggwvr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3bsnqxdsl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3nfzsdqli.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3naoopybo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dcqbjcum.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xcdgguna.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3feobivid.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3cvgiisvf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3cgvfgwec.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3maocrvtv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3vuimjwxe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3shpjscfs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qcrilgta.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3isigsfoa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3tbuxgdna.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3dtbnciyq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3hrnzvauv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ghntyzhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3snogamfh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ezhlkaoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxqgbndg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3julzyzws.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gxmmaxqk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3iqxcoxfi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3utyrpspg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wiivoake.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3opjsuzfb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fsjddutr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3mznyathx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vejrglou.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3wxsokhye.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rkjfjifl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nsqhvizn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vbazxeqm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dlybpktx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3bizbdcgd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fleaynvh.html


<!-- 参考信息 -->