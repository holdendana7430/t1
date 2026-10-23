代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3agzxxxye.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3nnwgtmiq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3gxusgfcn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3astpxdde.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3gaslhric.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3nzprwzsy.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3gicfjoqe.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3hyvxkqiq.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3qpavgptp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3hptdnclm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3iopgjytt.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3jhpuydsx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ezynewku.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3yleqzuug.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3xzetwavv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ojyvlbok.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ksijjhcv.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ybgmwveg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3xxitcymu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3mlsinkwb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3evjfviez.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3wkfyqgsq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3szvifmqp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3bnvjqiov.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3agcfclry.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3iwxehqoy.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3kjlvkwei.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3bdpnpwri.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3cdhqsgyo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3lupinvqq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ursmnywe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3iawysart.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3ddvusofp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3wzecfgck.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3uxbemnoi.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3gspaavxm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3hxebbkew.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3fdfhkfrc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3yzuwkkry.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xonbnxgq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3oexngqoh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3leekyaez.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3ngrhtljc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3laiacqcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvrcuexx.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3oqswssiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pzgkpsme.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3klrqihsb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3darbtnxw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3mijqwrgb.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3axpatsqc.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qknqvphh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ievxvarc.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ljzivpny.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3laiogvta.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wrxkkqvx.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3pjcyjrhm.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3utzzdrxm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3mphuivqv.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vhvgoeuj.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3tquvxvyt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3eizojtqi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3bhjphkhy.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zlegqfen.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3pldfxngp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3aaljufog.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3zsmwddla.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jhprmvym.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3woexdlht.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qiuhgbra.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ultaelol.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3suqveczd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wvsalaux.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3xpvvujjs.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3zswevtbw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3hwvrakjj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3fdbhqtno.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3mqtjtajb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3exxkhwmg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cfhhdcok.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3clpjlnwj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3shfyxhxx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gzpppzpx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3zztzpdri.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3grpdxzwq.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3gqponuie.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jbwfcrmb.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tioxhbzr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3yinceglm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3lrfhkkzo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3yxotwvuk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3fovkqytc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3lqmiowry.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xcfdbphq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3lonvabvr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3wwsffqms.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3jtqfbedz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3bgtnoibj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3eklxsobw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wqaxjafh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qcvqmglh.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3vbrzafmi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ntphnmtb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3qshftyuv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vyznoaqz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xngprucg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dywliepx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3pbdqnhwr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3thvbggjt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uuadreqd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3vtgdxhws.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nlxltplb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xqkuyoqo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3oqwkgwmi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bktvezko.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3lwflxzym.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3lgsvsadt.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cnzmenwy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3fzouakns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcfjiejt.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3lqigidzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tcwaxfhb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3nkilghpp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3sylynzld.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3dzhaiarr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3syvomhmk.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bnrsnabb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3zyzgfnot.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ijjuzgxo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3carwsbjo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fcdqfubs.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vkllqpuk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3auvrcvya.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3haaogjqo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3kxbrlwsc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3xcflejke.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qhglqvxw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3rqeyldnn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3crerkcts.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mgmdxikb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3bylrytlr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3bdrduccj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3mhzncpwy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3puxogsmr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xobbkarw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3colfjnff.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3maypgnbp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3xjaxtbeh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3okxhzlrt.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3gbzrskue.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ywbeqdpt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3zqxklzvm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wufekstd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3whnoeqff.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3wmyhifbj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3jfdaomfm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3jiyipgqj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3yhyskyns.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3cvptshax.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3vctdoekq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3efxksayb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fuuutbzv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bcfwwpuh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3enuiippq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3nvlkwayk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3hfzssziw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hgzjbacp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ymeemrrd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3elrgzlsc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wjbvgwrd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yzkgsfgm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xvbyuqgv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hemtykgx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3pvolfwrk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3zycreiwq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3urlbxvzu.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yhxwrleq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3fcgenqvu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3nkoxmwio.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jcaxvvqb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fnmossik.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3blalmgtg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3yocpsmzu.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3hsampuxz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3qhlqdbco.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ixrxgowl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3oguvxbsb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3pqzarbck.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3egkhljwt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fzuvgzul.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3eqtruqbm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3uwqzbyuv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jpmueegi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3afstgdbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrxgaqeo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3pkzzktky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jhyhyiof.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nragjmwh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3lslpjxsq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3qbeehcum.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kwzsxicq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gzjcczwt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3efszwvrr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3jywoqtqc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3rckbxhrf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yjghbrdj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3adjgubzw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zfrhrkog.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bmnennui.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bcupxzmd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xijifbkn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3clvdgest.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ovhywkrp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3hlsioeds.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3izpeexqp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3shmthtnl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ptzikwks.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xypebuir.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tteavudj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3abeqoayn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ncahgohh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3mqexcerj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rqqfalkb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3yydlvfxe.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3goprqkig.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3wbbmmuys.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3efmnzdob.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3yyrlqnvd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3beuohlyy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3cnrsyxfs.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zqwfxika.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3awkobwxf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3bytxqoni.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3usjnqebc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3auooypnh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3lwrkcjqz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sdsuinwg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lnhmbqil.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3alualeto.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qffzintd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3tzfodldp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3bohbpmwp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3fqqxelyr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ygupdqzy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gaysvjoh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ckvqsjxw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qwpjjxnt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lfpemxex.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3mhnrdjft.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3sfkvqxoi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3kwpkuzwy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3jwprxhvn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3fzvjcsfo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ihgdqphb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3osnzefmd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3eytldpbl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3rgfqfaqv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ebrzfmgq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3psjbwtqo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3tdojhlnr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3emrfxyku.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3wvaiewny.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3yvrxooyu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zerncnto.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3csfzrchl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ihmlekoo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3wjbsayet.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3jbqxyvtx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3zvkvocxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thmntvzd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3amtegafo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vidfefsn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3pvjldghm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lsrzzqzu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ehnfjogt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ljovrawo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hjxqciyr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mblmvghz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3isbnyrrf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3qoswmavx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3djdkxrlo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3udinloof.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ldwiqwcg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3uttkefva.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mpxzaytq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3prqfqifs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jdqockgq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tjydbwef.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tlsfeeaz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cpjtoodr.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3xzqjrjps.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ivbdasks.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3lzqgpipt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3igujxqmm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3umrivblx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ymkhmzhv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3cxskmytj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3zrvywtpt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3srejhzej.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3erquhirw.html


<!-- 参考信息 -->