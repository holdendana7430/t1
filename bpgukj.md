代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3jnmtrutv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ldbyrgxa.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3pzhrlcsq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3sntzmdle.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3bcqxywkk.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ageamakv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3rkgjmtvk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3aftqvsro.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3uqynksai.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3swjhxbcb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3tldbdubi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3yhfabblx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3icvnoqaq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3dwtunavx.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3wreoujuf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3dbvyawvn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3njxdqcst.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3yjlyvwzr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ofiihufx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3ugyhmfcz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3qvhpapyi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3kxzgxsbk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3mugexmhr.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3vsrmkhko.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3wewcjvge.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3iprxbdvv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3owaiantn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mkgdkpgr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3hpqzomgv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3mnbhyfpj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ezvxeffo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3azueasqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vmwutlsf.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3ukydrdmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bygiwfkg.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hvplaufl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ftvdmbys.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wjxwpeuu.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3jfuzjtus.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3avbdjnwy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3vipnnpjx.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3etekgfsv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3nfomutaa.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xydtdjij.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3cqgbnlsh.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tckeijfw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3ktgnofif.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vlperqal.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iwoljlgc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rcksjmxn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3dhthucby.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gmhyysvb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zbbkecgd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ybsqxjzr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3quhzojhf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3bulveshv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qjsxwjla.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jllqbbhh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3fjztbqza.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3qrbulyej.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fsuuikux.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ywuzqugj.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3tstrzqva.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3asvmjnud.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3kjaaizzw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3pncqajhk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3yvmkdbsi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dgichsdg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3mvnrmebx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3waswigkt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yysvuxae.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3uevhpesh.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gpsepklu.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3zhnvbiel.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vbhsfucd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3equgygxr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3dkrvxmsx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3vbyqgemc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3mmxkvciv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3rwooteag.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3nubknkps.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qisnlxlz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3fanpczcm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3heicvvzc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3unyndmuy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3bfegvlmn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3suftbczp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3muytudgz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hvekbynf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3bsfidgzh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vrwqxuov.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3bpqdvurc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vvzpprbe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ybtdkgxm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zeyhsayh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3dyeuivow.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3wctbvugj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rzqgzsdw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3kzrzyzbf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3eavalefw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3rqvdwsii.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vrcwvnmq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3rviznekf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3cmibaqwf.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ollkdzvp.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3paiklwth.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3pyxzcdkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmvvfnnm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3acvazgmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zomyqkky.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3pnjsbgnd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3mwimyeke.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3tusdfwaq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3snfgeqpl.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fczeqeca.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3kajhyvnu.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fcpwfxgi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ykmgfymn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qmpwetpw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tzbmsqxg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xpvxnrkj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ninitcgt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3eujdlomt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dzjppkpd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3hjvbyvch.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3fvbohyyw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jcacmzsu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3wixeduwd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3nfqorlsi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3uyifhhvh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wxhppaoy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rkkffnlz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hicfcxvh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3siminffl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3stcdwsxd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ibqqblhl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3azkdrvgz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ahwemgzo.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3horgynfp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ndoorbpc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3godvdebc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zgfqctry.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3eaedqngn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3gneabzqj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tvdwgmko.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3byftnhud.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3wymzkvgs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ajmykjwy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3mcfcywfg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3twpzkoqp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3japcjulg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3cjgriccq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3hdbqrrfz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zjzeuzfr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pkgzzemf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3giurhkla.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zlviojug.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3rfknbvnp.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rvvkospr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wtdzsrlv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tfafucis.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3gzafcwsw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3aniotjar.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ertsdwoa.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3twesnqrx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3sqjwunwu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ntvlnqme.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3eqnwtzgq.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qwjbenaz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3mcgfkqrx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3casxwxud.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ovcruqqq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qrxklqee.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3stxsdumc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ngegmgbl.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ewhdsubp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jjdzjvwb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lfyertvw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3vpypzigy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3zkwizdmw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fpynrttc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pahrfcqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nytshoch.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3rjyzbeic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umfaxgcf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ysmhahzq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3lyrprxwm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3eggqcqvz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3bspzahxw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ofmhgwli.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3akdxkeum.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3retqhknw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3nowicjyr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hkkzwocc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3jvmbajnk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dttcrkzn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rkroplla.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tlvxzpyr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3aeequsug.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sewngymd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3myupxjdf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3iorjeeid.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3btupddik.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rghrjahd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zzfsifua.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qrxdizzv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3otdqmwhb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3njehrldk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3onjrmsnh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3fmyyyrbq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3inlfmkqz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ovyjlnbq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ziqdurlb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3zvzyqmnw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ettnoqso.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vpdbpwxm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uorqbhzs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3sbiqaexm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3lfkhgbrk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3tceylfft.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3lylbsbtg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ytpoifwc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ygwyytny.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qkhxukkx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqoemlwh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3awayxexn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jtylohrz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mnjdgmqs.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3lqhtzlmt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ixmfswne.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3kljtrzld.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3agcjlpsr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bcobagjp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fklbsatc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3akuerhxh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3xtpyivzd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zhxldgbw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ponufupi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ggtluuak.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3lboqicas.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ktmjdfke.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3dgzylpot.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gikmnmkl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wgiqckod.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3lguddihc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ttlusrco.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3cyprdzfw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lvphwhlk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3hqcmoaci.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3dtwzunfi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3czdwjllz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vjwgtkoq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vfvwzyhi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3gdwogyeh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3haeonile.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zdhddndw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3urfdlnhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kseyivuf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3pqffbmvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lappnirz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dhdompjv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jkhzmaee.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3znbvrtiy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gjqosyjt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ywgibskq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uyvkgpdd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lrmmfjmb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3sixbolmd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gaikdjdw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3mxdaxgfw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3cerbfqan.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rzeanlhf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3igoyvlxn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3whaspjll.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3iulgzwlt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zmqemopt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3uaiqrgxq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wcuyrxuk.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3vkqrsfil.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3davxblud.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3wdrrupmc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3urqaemty.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3oqpuzjju.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ntssqkis.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3cntxfmkk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3wkngejur.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3zytpsybj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3xkjdenmv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ullfjksw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hgdebdbf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3djbaqjal.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bqgqxjlz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tonqgtvv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3saglkgow.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ernftceo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3flldcfns.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3kinrvgfj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qoafxuqm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3nmoixlgo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3agxggbxk.html


<!-- 参考信息 -->