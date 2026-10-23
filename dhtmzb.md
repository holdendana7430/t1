代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3abfyjuko.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3qqxqqugp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3kpkgojzz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3lmynmzcc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3bphwerwr.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3uafnpnkb.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3nghgemkz.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3ovatyzrl.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3rbhadayc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3qdfkjwqs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3cyffkqyp.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3mlejkbsr.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3gzawxlru.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3gksmthcw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3zttfteri.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3yehdqkeb.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xataypiz.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3abljyqmj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3afwgwtui.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3ooluutqg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3hgqivfxg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3atnslcxr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3mrlqmkff.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3xkpoglee.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3lqkzwhex.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3hklsubvr.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3whgaouaz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3yzenvvlj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3vwafxoca.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3kxmhhmfx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3mlfjujoa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3rcpodssv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3nzlyhzzx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3buvczrqr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3rusbscvx.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3glniutqj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3csnqpcxe.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3pqbyqonk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xogzoywl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ctrqccip.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3dvwuymyw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3srznaqii.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3uzqgmxsf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhgmhcuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbvauczc.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3rabxacpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nranbksr.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3eziyouwe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3upseomsn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ustdzkdz.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ndmhgcil.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ieppjppr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3nonfpksm.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bvfrwmqd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3qeeumvhl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ojlimkwi.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3yhldgsvy.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3lpuyggzf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3nbmttaij.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oqtmvwqh.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zmpgqplv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cqiajfhd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3tukwxrrf.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fzrbbyxe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3imgnftay.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3lctvugto.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3lxkxnslw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jeiuvjgl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vlrdhfby.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3coeqqgrn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vztobfxn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3tvgyscao.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3evacvlfm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3svrqcpdo.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3mtzyxicn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gauxonlv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3tbuufhky.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fdldicja.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3arrzuzqf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3alysniiw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3klhjoiby.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3cjqakxui.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3riddqekf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3xjbscnsk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xhfsddez.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3kcnrhngu.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bcjlxqzi.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3dnfvrdaw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3pxnyvhcf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3otadfwja.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ryodiysf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3jfvawqns.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3dsypveed.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3djhesoki.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ulbcaixv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3riilbzdk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xoeoqvdo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3lqdrjexd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xnzesngt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3cmkivksw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ndysfjjq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3tznhmdlp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pogkkqph.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3mmrndxzp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ljpfypru.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3odiuuqyl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rkycmmnt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3nmvtiwvd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3htyihtrg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kqdrsfpb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ffcazfsk.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3fvinovkc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3zransrmq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3rcyeusjn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xmkuowot.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3czqnxriy.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3xucncglt.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3seyfmnit.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3yfoznkxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jzggdtth.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3neegcbyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxrrsxvm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3dnwwviic.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3vynobovu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3tglhbblq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3trktcyjb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3nzbklhaf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3wexeaxdd.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wbgktsqz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3alagajzq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3myrlebem.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dtmqbeja.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3cudlqkna.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3bhrqdnod.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3elnokcjj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3gykcriub.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3plscapho.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3hokxkhka.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3iizihhqf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3zazkliqg.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3qnyiuzei.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ohqabxsd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hnzwpblu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3efrhtilj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3fnwcnhsw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3yuhuzyay.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ajmpnaoi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3btprxkxl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pxaogjxz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3sbvogjxi.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3esoatfqv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xrxyricm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hzviazxz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3dvejhvzo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jipxsyyh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3jkksuyaz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3yhcfrdny.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3yjvzifoy.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3nqipyiyi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3fcqrfieh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3wnxfjiky.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3akdtffzp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mrsrtsrb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3abmibjxg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ibxnfyki.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3dutylncv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zyvrzrzi.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3zwegvicg.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3imdzoqpq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ajvghwac.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ksexaibp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xjqqdduc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vzmyuepu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3rwqjnpkq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3gxcerlax.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3szjfnhdm.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hyvehzgp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3uqcbmteg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hemvafns.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tazrcacj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3sczqjavr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3xbaggybk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3igstlbui.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3rnnehuby.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3oazqdxna.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3vajhbvjv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3qigjtesp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3sanmtlgm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3isgculdf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uevkxgnr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3etyrcbog.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3vlcxhyon.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hgrewkho.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dzybkhgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhgbjwtm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ucxknyml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrwbsvbx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3plslcxnq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wiexdmlv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3aafdxdzo.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jptfrkve.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3adqtmbrm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lwvrgzbl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ktlxhyoe.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3pxvdcbpw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ccsulzpi.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uccgantx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kuxmbayv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rfbltcgo.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rvrwctkt.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3doefwqzc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qnherazn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rzzzdmjy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3luzksvad.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tswliuaw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ovctsyjx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hsqnydpj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ewrmntbq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3joxggvjb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dclnmcun.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3gzwssqzr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3mebdtxry.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3welkqvvn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3rqxaueiz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3pjyjscka.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3hllvzwgn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3xxthlmhh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qulnmcqy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ltsswqqy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mdyokwpw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tjjtpckm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vgcqyqrx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3xuvieqnc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3shoybktc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvchobai.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3dkfjgfft.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zrzqninu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nfdrybug.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3venlikyu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hdfholft.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3svqhwcai.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3nigdmxiz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3zgsktnmh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3rrwkitcv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ivkrzkrf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qhdmlawk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3swxyfwjq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fxevdgte.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gattllaj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3tpedgpee.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3rwlpxnnv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3qqmcqzgr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3rinojdqw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3lksuktad.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wfpxyvbe.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pwfzdxss.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3lfmlymro.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3peyxtpwx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3wbvgdicv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zknejgom.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ugvgrmjt.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3coaaufkc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3rxznaqyz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fxyxjahj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wtylthsh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3wzrrznaj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qesetixp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3avisqlap.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ikaqxdrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bittjtwl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3aergcffm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nucmqxbi.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3zjlidblf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cknfxfzl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ndtufnvl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3plvhmmvt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3niwjkjvl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gywwbfpe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ihywukwj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3xrguhcvz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kbwveeti.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3xzlfbvfl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3alpoljtc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zmidbudb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ssmmyquq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3unggtgeh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hiwofmls.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3pmebzgyt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3akxzlzmn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gxmcownd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3jtwiojpl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kldzbcmv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3gtcoedmc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pzjyyuvp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kjhteqdu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cinxdscj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3hgxjqisr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3rprtlhiv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3iugsgcgp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3eupxehpk.html


<!-- 参考信息 -->