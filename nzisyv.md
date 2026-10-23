代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3jmajnsxx.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3elgynjsc.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3sxtoxbdb.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3ntcsdzic.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3kpxhrxvk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ctbzaeak.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3leamhbgj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3qmmlctfi.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ecovqhxv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3qrhawviq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3xiltmpxu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3utqotlaw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3whhrxxzu.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3mqeuqheo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3wcjedarh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3zhozhrnr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3liaqispl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3inbjszxf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3gqjqmckx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3bebngeqw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3rrcoenkj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3omrujbjo.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3pyuzbxem.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3emizgrby.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3xmvcorqd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3sskgoofz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3copgibup.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3peywdwkf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3ixtspyco.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3jpjzpyoe.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3sybmlycb.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3lirfykrz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ypqfbfdr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ayivuaps.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3svdlkilo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wjcytowx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pneaubdo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3xdexzvnz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3shwmzsko.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3rkcgikef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fyhstowg.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3oyzdppth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qcsbpgye.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qijhzgla.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3bggmxuyy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3nscyupxk.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3rckecwnl.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mefsaopb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3luxitfsk.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ufwwyuet.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3dksxsppq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3talvnvep.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3wqbvaqlx.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvvfqijf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3ruvdvlix.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mmsrzdms.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mlpiwyiw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3twnbrqnr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3caapqlej.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lmxwozdk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vyuzhumd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3qhwrplmw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3upxcgukh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3xrecwhgq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3zljbuigz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3idokslys.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3lotttsla.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3obllxtcy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ytxxiojr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3xvuqrkdg.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3fzxmgvuy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3rqofljrq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3txjyrtvc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3gferqomi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3djfkvhny.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lidzrdly.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wxkhnxxr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3uyhnyxju.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3krvtntmu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3memwpxhb.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3popvvzdl.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3yswkyvyg.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tthqebrv.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ksgykpcs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3sunwgvik.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ikcwpeni.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3zzpjezhy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3azlwrken.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3itcyupjv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jhltkmzj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ckfjofpz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xzqpttnd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3azabrkon.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ddqiudic.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3craszize.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tyawyxpx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3cdbrwilf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3buutzmyx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jtprwbyf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3fvfifivt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3whlgeust.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tjpuqwti.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3itljfvat.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3aevuwloj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3sapyqiun.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3skiipsqo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3tsmnnqif.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3nzemlovo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sefhmmmk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zekjksow.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ziaxhwcg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3aplfpoyb.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ofoxwshs.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3elmnlndn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hmrgtphp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dsbpexjw.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3mvxmfbla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptcudkgu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3zhofjiac.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3nloawubk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3uwqutrhj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hqvfwzbm.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3liemildw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3hkodyvtl.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ayqqjyxb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3pafusvli.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qofrinle.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3msromzig.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ytzrhbxa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3fmmoecrb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ljymtbei.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3hnquocmr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3padhyfkt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3wmfvqsus.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ifuoqqpd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3zhonaxee.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3lhrsgpsv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3thlrmats.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3hnidggfy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3tshprimy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fvdicfjv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3qxevdotr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3lhlzjvsm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3mznmdlny.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3nlddienk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3zapgcyam.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hkwphpcp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3cytjiova.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mxliwrga.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mvmgkorm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3kgzlphdy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3cvxekpwn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3pgobybxa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mixtgwgg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3cajhqjcy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ejkceock.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3sdvcogpb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3nbhwasiv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ozplhjen.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3qdmzdyfn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3xbymvuci.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ebhbluqi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fxkygrkk.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rlfkofty.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nmoqjnfi.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3skoasaqh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ccwuaxge.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ktmyscub.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qhjwuacf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3armtwspe.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3oqfmkpka.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3wvbgjrcc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rbbadckq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3zigqidam.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3vuzooive.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3elymeigx.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3yrcjlhlp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3cpnbablr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wqzaoaws.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3wkulojey.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ytlthqwo.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3lnzpefqj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3xxvhamoq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3styqujwp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3byrufihs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3knmrxamp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3zsrjfwcx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3qfgvdoma.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gnpkziym.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xchdfxed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qckpttrf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3rzjigpbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3famsmnsf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3znpcnuhp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vpvtkjph.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3purvwehh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3eewxaica.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3udbmjwyh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3sqsyorrz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3veduqcco.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3gfkibgif.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bswoqfhn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vlmdyvxt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hrhovozx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jghgplms.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3sbvbrpzn.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3azgdorjc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tshwivqa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zkbxiwil.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3swephrlk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3opyajckj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3hnebodrm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3jduilntz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3pjkppysz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3eiqudbnn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3dmsonqvk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3gebrolaf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3wqsdjmps.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3atqrntdx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3vuwibqqc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3humwezbr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ukahfzbd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3thrgyscp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jcfsbnnp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zaysqmkp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3tbdwvcgc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wedpohsu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3englhsjy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3gtribwyr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3onlgzqga.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kcoijrgi.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3yxjdqafo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3libofwlp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghfhzbne.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gvpgcsmu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3litqslfs.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fgietxko.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3clgqskgn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3exgtosfb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cupscekg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3drrizfpg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eqbiiyto.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wbyxrgec.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fufsbeil.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3qnvxxibj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3zamnsqav.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3thlafqpf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3uwzdhkem.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3mvkvgfmp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vgdpswpf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3miydyiyv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ujmjmqrt.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ygntdzot.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3penlglxa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3slnbrvjr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3shyxirrh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jhopbklj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3wcxfaepu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3rqbynubo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jzatniun.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tunluxsh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wlmfeuvs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3cdptddxz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3iephbosp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3zhintnyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndyfkhrk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3hxwjhhfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ivfijiol.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ksrwjksp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dupfehpa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jjkfldbi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3osmlfeml.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wpqycdmq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rtqxbwup.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ndhdzilg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3togwixac.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3usmpyjuu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3hbnlljsb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vmhupnph.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fuwslxse.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sjukbfli.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3agqatddm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rwjwupaw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xweeezgf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jhfxheom.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ojwloytf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3volfrdho.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qkjogitm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3kucdyrad.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xptshghp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ivkdrugw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3phbdrvpg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3czjdjyfz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3yixfgdhu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3gbcuuosz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3qvyilkvb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ozazdica.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3clsaknmz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ckuaaqtr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gpsrphap.html


<!-- 参考信息 -->