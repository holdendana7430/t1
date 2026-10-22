代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2emhwxtgg.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2pqpmubax.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2ldzclcup.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2cfzrjopv.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2fheixjda.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2demstgje.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2ppqlpwbs.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2xnbsztag.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hjiebrhq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2zgvtfvgv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2kkekliak.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tqwukgum.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2rrriaprf.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2zfohhlob.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2tmjzzmdw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2hhitqdor.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2amefarob.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2degohvpl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2lxdipshe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2zaatnhxj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2agqmegiw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2phmadshh.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2nqviyovq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2adxssflw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2bzgikglw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2pnmhlubd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2quietrff.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2shmyahqe.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2cfezeuyk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2uuwljywk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2evqdiqfx.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2xdeacdzf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2rbevsvyv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2nvfenrrm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2chvtjlor.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yzlafxzg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2agoehcxn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2rxbsvdzs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2tyhyrjil.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2gquggfip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqcozxfx.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2qzrgeowl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjihtlhc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tqadonaf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2cndsmcvy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nreoopiw.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2airblnml.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aixfrqae.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2hrojywzz.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2xocbckwa.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2rgexlhgj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2rhkujfvd.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2bnjvwckt.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2hgnlxxvt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2wkbyqypt.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jvwrcerk.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ooycmhpr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kvglhshq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2lhppuyih.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nrfhvgox.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rxncacrk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2suoebshm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2tqkbrcwy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ixxoijtx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nemzsfbd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2mxagawmz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2igmtfbfi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2kvndukce.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2qhnseobb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2dnxaectp.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2kyrgvupp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2qedwwcwo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2daytxhfx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2gfkqtqsy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2pciqiwfa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ijcxagap.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2fdmrnnhp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2bbevslwt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2fwbyicqb.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2mxzjvwer.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2osuqhfbr.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2qhtdgtqm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2umbuheji.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mvqawemc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2wkzoshzc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2mqpratdr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2pnxuvdam.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2pognfuzj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2bimkrphi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fskpqwrd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2vfqzkdlf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gkhmpeqx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2uwzggxdd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lvgdnkyr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qunulhbg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cxqrnais.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vkhdpayo.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ajcwknmi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2btxfalkh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2gbxcjrta.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2erceuxso.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ovbyiuhl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iguxfvnw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2koiwarbl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2idmyxmua.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ucufwukc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2orddhipf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2mmubgmdb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qcondnij.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ehzjgbia.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2tvmmhiph.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2tgrnhluz.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2vjzcsiba.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2isuewbbp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2amffdqzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yggxpqoq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2txmavvvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hwacrpzo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2yxkqlsvv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2bdhjhmqk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2qdcrddcd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2znswrjgv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2hcsrvuxo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2wecfoarz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qnzpkgax.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2gmzuevkp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ffvagskh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rznpanru.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xnqfhsgt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2jsjrzdxb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2srynonev.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2itsamwye.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ngdeuatm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2iewqhlpn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2slrfxfgy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2srypuxfi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2micwqfpf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2tsyqojkh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2hbvaosvw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2glyeuqjv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ushchgsu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2vurwbwys.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2sndfjokr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2dvomzyin.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qmkaixtz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2lsooacrf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2adqaelrc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yciwfmad.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2uwvughfa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ajhtcnbm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ozfmkwbh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2eouflgeg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2bkwtgobu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2qwldpldz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2xjpcnasu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2lkfuhvpk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2elknwbza.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kgtsmkzb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2blxxmpfr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2doiqwzfe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2cdyoxzba.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2awdyulvo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2svkqpogy.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2dfscrjvg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gnrhhtsa.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2nruzybrn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hixvoeic.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fiqrkojo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ztdknaut.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2glkjnkix.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2edbhkzxc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2zplaldvs.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ixhuxhee.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2igwyrzfz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2srahcstb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pnwtqure.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pqyhccbi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2kjjuaajy.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2egkzcjaf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2rrvqtcha.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2odrqqczl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ovlutlno.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ucordjbv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2avlztpac.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pwtkkaxn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2izzhuekv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2kdmbofoh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2qmtpalzl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rhsebpew.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2duechapk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddhexkgm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xeesfysg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2drjiziid.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2erckivgk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2uigthnmk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qmjrcluf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2llxwvnoh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xpqylrtk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zizyhoxs.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2iawwyojf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ybmnyikn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xokloghe.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jguneikn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fhzqkdto.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tuaafqry.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2thzxewud.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bpihyugz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mplqnjey.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qxugfqpb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ewnxdeib.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pipicwkn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2zktquhfe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ievyjmea.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2lhibqkoh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iywpekmc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2czvxfgjj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2isxxvweg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2coznawaf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2hvfubaxi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2kvepqlai.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2tcivfack.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rchfgxbb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ipditbut.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2urlranol.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fltttiez.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2gwbqdqzj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zysanqjr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vzpbsvik.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2bifgmbcj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2gykzkwyh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2alhqpvaw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2uimbkvkx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hajwkvcc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2udtaogrw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xabrasfv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yxchjisr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2bwjzhrqe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2nxhvlpoo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dichsulv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wziczles.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2oolwhfrl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rgqkyjag.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ictxltsw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2zzojkiqg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2tdjqarfj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2cncuejag.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lbmmncjx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xipkrqsw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2yazutepn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2tjjyedcs.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bwrvlyws.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ahaaeztb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zjpjfnfy.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wkzkjewv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2lqdikcmj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2sdmsbulk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2hawomcux.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2fwcznjbd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2vxxblucr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bpwtzzlr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ugerjwrb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2gzoueung.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2aumguxgx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2jtfhvbyq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2agxjfvpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycqqtkyc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ynjzozpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcqfofjf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nxqqnqce.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tlkpasqo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2htnojeyi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2izomeugr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2thclxcyi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fcueokra.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tmlbftpn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2bpekjxzw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2owepcdzj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2hyhogccl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ruwlthol.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2gzozcpwz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uixckcax.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2afdizfap.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2epcutvkz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kurifxeh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jvoclkxt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gztjlpfq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2qwrqslbe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tizjobmh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2entqiwdg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2durrsypa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2raboeksf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2afwpdfky.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2lcaxhixs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2hnpgjvyq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2fkgyuoii.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2xiazajsz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vobsgovp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhsrqjzd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2btejrbtw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dxbspjpn.html


<!-- 参考信息 -->