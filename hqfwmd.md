代发 wailian999

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2petbsaox.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2vbhhkeam.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2pbjqxlbh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2vrwurjua.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2khrewyqz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2kznosreq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2uqmdwcsq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qjxtgbrq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2oithrpdp.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2aemdijjt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2qcuumpvn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2urvdcwee.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ewdbxetg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2xofipccz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2xlkzyfmz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2zcbiofgq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2aqwhgxrp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2lidihkih.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2tvuxnzhd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2fumohpjz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2nzkppate.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2skkqtmiu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2nxckxuut.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2axjxsptz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2rxgdhbdg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2phpufhnq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2qlwwopwk.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ryekijbs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2piqywlvk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2gwjuzjxa.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lyfheull.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ojpqoapz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mhsevvyc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2vjznhfnj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2qpskyzhw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2geainqrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nacmlzke.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2dlrdyuej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivlazwgm.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ebhfpryw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2nndzgkkm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2absyrqex.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kjdenuiu.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2esxdpbdu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2egvuolyg.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fmveckdn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2imkwvflg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mqjvlnet.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2cbuweqxo.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ueaayfmb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2pqihdxgo.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dnshlipw.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xqmiedbn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xsxssvlc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2sybpmyal.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2oblunlml.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2qrcpgzhp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2jnedxmtq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2uhpenlgq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2chejwiza.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oxklbyoh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2krouacpz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aruyiyiu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2hrfjvkrb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2bmkbwpok.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2dtzfpalt.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2wesegdwc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2bshuvxdb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2cylbxtlm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2usparajk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qcfgrfqj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2blywvycw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2sksjkiwm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2erhawvqb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vjuatrym.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2bgslbvsf.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2hjourigy.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2rwwchnim.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zurakhok.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ifwbqsrv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2oyzsvuyb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2tdwxddor.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2tbubpnzp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ohonktdz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ymiofrls.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2aczaaxbv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2kdmevjqz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2oeivqvay.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2iifgobuo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2dbtvovzu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2czpbxzil.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rhtjbrev.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mqklmnkf.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2xfkromge.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fryuvltr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2nqwvdrgr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jfsbwaqp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zamudmai.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qxdusqhh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2onyqdzgi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2kwabpkik.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kcmbqfgc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2pricdsui.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2oclbdzlf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2xwrvutnl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2usjbavgx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aibubaec.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2qamyrteb.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2hnmvpapm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zmynmqxs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vbiquxoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nyzudrmg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2qyfmnxnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtdblntm.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jgfmjwpg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2fyufmagf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2fnihvyuz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vnnxirkf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wzrnklyr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2hnvuwsin.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2qmuxgqvz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2cyxyvtwh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vbeizqqj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2scgeymnv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ppxjcnir.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ynbohltr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ghmjtlcf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nybkifhc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2gxvdkvya.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2kwrcjhvv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2plwhhvvc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bwhldaue.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2vexssudk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2wszrffwv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ojboqzmy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gmjegqwf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2tlvjuinc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xvbowwjs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2onmjsaqs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2trjdjiar.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wbvuhvxy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ufegvads.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2eovpucoa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2xuvwjvpu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2iprsdhsf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ccjbvhde.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ahgegfus.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2gnjhojrw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2mgzjgpnh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2yzktaphw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2zgacljdp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2aavcjhnf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2wwbxnrjq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wdymkxmx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rqelvyyc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2apyvlsnb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbwytpwp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2betfbydw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2avsumzwr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2vkizqngy.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rjyqbhuc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2nnudccza.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lwntgsik.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gwtrjacw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hjaiwzgf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2uysvgmmx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ngiuwcbz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2fefjzdbi.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gksshbgm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2gajhngmi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2sxpnaewm.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2gkvvrscj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wtpluplt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2xvbhjyqv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xnswhuto.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2zunvzrdj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2amujtswv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2xvqtmzxr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2drrkqchy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2pbopagdi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kmbetjiu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2olgxclos.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2gcwqwfcw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2zfmwaqma.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2aaszpfja.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tiuwnwss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2occbikro.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2pmmapxxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2arqamimr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2sfvywfup.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2fbrmmhnu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2fnowhryl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2paevkwkc.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uovejkdt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2veoxeuff.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yzhmryck.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2zuzelvma.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fiutwukn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uxpyraiq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wttiambo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dhhkgcgl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2irhdlkdi.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2muicyxmm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pryipdyn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2olhlqoty.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ykgyhpul.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rhaaiwfg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2wyixgjdo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2aioheqau.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2mjzqafxo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ciwcuimk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xgvkiikl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2vgcwfdvm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2krgryuer.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2citvfkqr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2itofekfc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2rydkgvhm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2usxddllg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2mwfsjapm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hjbkmvlc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rebtywca.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cttwjgpz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ytrljjfn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2dmjrbkip.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2sjsfqyxv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2kacbuxsb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ebjdubzv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2hqngumbn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2snsideop.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vtmzawcz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hjhkhual.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uzbohtbp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2wujsbgyb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2sqpauuig.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2mlwsobhp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gwogpkef.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2iwughcmw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ifojuggc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mxgttpwg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2pekabrjd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wfvorvwa.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2iqwneihz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2dqrkodfw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2jesmnsmy.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2xrqokydc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2gjpyeaat.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tnnalrpg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tppmikuz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2oyhxtfrw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xkcbxstv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2lyjywztt.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cwfcsnem.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2srxvmujt.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2tdzhfolt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2nodthblp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kfrqekrw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rmsboegb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2jgzbqxrt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2oxqnnsjj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2mdnpmeox.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2nmstpezv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgndzpab.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2sylgmqrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2siopilml.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2fucaikjx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2byealgqc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ehvdxpzg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nexragcv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vgefmpuw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2plfjkmza.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nwojompk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2cmypxwuo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aewmoiby.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2zmpmbemu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mrjumunq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2eemrmjgj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ubncpfan.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cgkprdrb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tcolftpa.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lvopqhen.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2egzeaaxr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2goztefdy.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2smfkrync.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2tywgdbjd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ounbauni.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tbmhwuac.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2omvlcacn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cuejgzgx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2zrokdthx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2bjctloue.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2quqerfts.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2pjfthhaw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mysmrfrc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wjqigthc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uludhako.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jqeuggnw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fswkycnp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ctuvolsn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wikkosbg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vzsozyvq.html


<!-- 参考信息 -->