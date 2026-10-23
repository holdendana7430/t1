代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3nmddcyaz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3yeufgebm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3iwurfpps.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3hbuhtakg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3jjdgkjnd.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3qgjqovsz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3gvpzrbxa.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3gjyjiovd.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3qfrspocu.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3zvjchqlq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3jdncswhd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3mxcrjzyh.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3olmiychz.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3nmsvhwor.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3fedyerhj.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3bfbprogj.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3dhdnxalb.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ouwjydki.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3payzaqyc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3kxyuebfg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3urnemmws.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3tkvvhuzg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3netzscxr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ioxpkwol.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3bkckhhyp.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ttodzzhm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3czwaggey.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3xpbmylnf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3gaalbrel.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3ikjfvozu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3lhbeifgg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3plhxldok.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3vszwixnt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3tznozquh.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3aryjyntv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3zqssvvfr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3ehecackq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3kfmwiizm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3nerqqwiu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3glulytrw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3dwxvadzh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3gfljzkhl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3yteapwff.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3nroizfud.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3fzmrhyba.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3birxpwmy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3csjjbcdb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3iypryexg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zecoqtkf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3dnqjfkqb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3kssndiix.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3wauxyxmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vutrpuek.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3cryvmuhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wyjmzuzp.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aaluixzi.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3qzcjidsd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3atifkgfh.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3drbspkvu.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ilvfalbt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3hkyjbrrp.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sgyesuoj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3dbfclsdh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yctwkbai.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3dzqwytog.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3jmnihhjp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3jzmgaljw.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jsjhlozh.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oapyqhaa.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3moibvaxn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3doyrkmty.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3lmznyzjy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pbeckgau.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3peppxlcd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3omkctvfx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3codlxxoo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3pilndqlc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zhtlmuca.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3joyxvglt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3vynuehwf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yfdbzchh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3raqstnha.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3vbwncysi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3abhvwlgt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ivyxddkc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hvwtownu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3nqfjmxum.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rowvjbdi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ugvjmzxk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3aeelvtbk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ycalknbc.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3detnkukp.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cvtflqxt.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3lnxnpdsb.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3idhjggyt.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zutltwpd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3bkrvluif.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3wxfzpkol.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3nomqhanm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3jnpjqvjr.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3meruubhs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3kjwadywn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3diveqqkg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3gsbzgbig.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mkquxmwa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3hoqghwbx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ukbklqtj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3akywsqiv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qaybzglp.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3kfahwlgs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hhpexgyb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3enhtuymn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tzyjalyf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ygzhigmt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mfedtjxh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3xrgohals.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3njabnllr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fwlujtai.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3icubacjz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3htuyrgxw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3mupjxclk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3efqdflcz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xitqxlna.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3hsfozywo.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3fiuhunri.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ljvuykye.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3sppoddwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrvwdnhl.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3mybwbqxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ogmeheap.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3yrcljnyl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3jxokxikw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3slyuwtfn.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zobitvae.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3imliyozw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3eddjkiet.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ywhyhzmj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3nixzhczt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zrytprua.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zmllomsw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3rzoygqpa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3iwwjozxv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3lixefmdd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3zfzvkwiv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3disganzx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3uuvvobaw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3fbouzocy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3nouwumpb.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3yrhnjrmh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3xxeujuji.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qkcjliqx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rhgowrzl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3pjpjxxwh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3zpzcbrlm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bcvzkffq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3fwmjfzju.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lsfmeehr.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3lojzmvic.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3jtxzztwa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3uakifhyb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3egqwrerc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3unahmlwh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3akvjwqmx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3jbzvkukt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3yxcliwfq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3hagsinou.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3hlrbrhem.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3rvqewisf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3tonhesni.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ikzuppha.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yvoxvgxk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3msslqsol.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3jndyraze.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3bfrragty.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3otjmbnmj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fhivlvjd.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sjxcaraw.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wnpqerrb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dauqlhja.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wjeydsqy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bwpttsap.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3bobeuxav.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3lxnkjxwq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hfqkfnka.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3syuivytj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3meouewov.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3sxyuytxq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qbrqvvff.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qfriygpn.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3yhqkhude.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3sjavddoe.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vqradohm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3aeojjknh.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3xptgtxqr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3pwcsafqk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hcwsgmll.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jytimzdi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3budkdvvn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3qhvkwzpi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3oxfwiatu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ubiwhegj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3bbymjwsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mqooobqs.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3nvwqpwoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqobetbj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3thiwsenm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3fllorvho.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3eubcyvux.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rrwgfuno.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3upgwpcdy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cslasodm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3omwbzkng.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3kqhtsmhc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wvxeopdp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3puoapgyh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lybugkzv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ddmsvrlj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zqcbifnf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xvriorpq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3btpfpjuv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iebaxbpf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3oqaqildb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bjrwogkw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3dwzlyfsk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hjijssul.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3dwritngc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jojpuesu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ddjnlxrn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3pwebevzy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3emckalql.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ivkhhdck.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3xpsfflfm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3aojalqqa.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zoecmohg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3uxnqrvqy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rnkiyllo.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bnzihmtr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3bkuxrizq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3tfllvejk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3mtisdgrr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3umcomxem.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3gwcdjuuz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgjptrhx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3vixuxbcp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ntbofctp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3evqizmms.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qvhyjloj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xaelguzc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ulkzvzej.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3bqadqtig.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3hyzmfsil.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dhqjvxlc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gkfnomnx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gokujihn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lquqmcwq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dkrnbxtb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3uuihtwiw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3nhqpljfq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qdbogxyd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3stthrwfg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qekosliv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3zcnkozvk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qzdlymsn.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lujunlxa.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3cwzsgkyf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3vekncwpv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ntmwqqmd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3yemccxdv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3bswdsqlc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fhdkhbuz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wisockjs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mlzjdysj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ftcaahmw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3yngytixm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3vwemqjee.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3sdderinu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3flxodgwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afyrzxmr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3cxwzbcdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jcquuzud.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3uwbgoosv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vtfntgmd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tttjvowt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3keeoiruk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kksjhehk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dgvbbmiu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xchzubow.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3tfdtaqdx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jithgxbz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3kyytfrxk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jljmsrqu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3wjhmiwpt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sskdlizf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sadwsmit.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hexvnjly.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3awvurnmi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gnracrwe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3bovqyfwl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3bcawtnbx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3fwhmjdgj.html


<!-- 参考信息 -->