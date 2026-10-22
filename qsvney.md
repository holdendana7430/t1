代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2gdqldvsv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2kszdqusq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2nnmohwmh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2npjfldis.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2kgayrnfg.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2yxjsoooe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2faetzbwu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2wgqldvzm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2fhmwpwrg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2xknakumx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2iqdehcgw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2vmhqhxbd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2mzqrgzzr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2yuywrmmd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2igwurjae.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2yfobmxam.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2scyehetz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2uuliynuh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2qrllprna.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2ygtuefmh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2bweaeevv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2cjcbbsxl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2tixjsdxc.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2clejwhza.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2xnnbxzen.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ybrackzs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tvglbajg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ahpvzdmv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xotfvpzg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2antkhmyh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2agslkjti.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mbckbctd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srsvkszq.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2zplraolf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yyaxxsvx.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cglrkcwp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jddydepx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2qnbujcnx.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pachlakf.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hvvbpcdq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2xxpwnudn.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2gxealztq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2faqsbyhh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2iojrmsle.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2mkynvxyk.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tjxzfgcw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2hsjnkhcc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lhmmbcyy.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yatdmsdf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cmubembc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mrwlffqf.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wrbmzhbl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pvivqaag.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ozixscrz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2nykilpwd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2qinmhixy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2glqczspt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hklktmuv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2xnnegdyw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2joifnfze.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2jmteyams.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2kayfpzbf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2hzeyobrk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jceyobab.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2kgiwpdfy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2drytuxmj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2dwglqmjs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2yhpvlfrt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2obiglzny.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2tuajhxfd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2nwvwhixb.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2swwvbbjl.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ozkhtzal.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2cvvwmqdh.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uppbsmxv.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2imqvjjsn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2iswtceoj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ltaotkmn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2wvvwikyy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2vbvqatax.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ilihrvjd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ywdhlamy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2yrwozfxd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2sdvopphg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2itbekqgc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2gxkzfzia.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rruoowpg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2guyesvlt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rehnqqei.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2sevzadaa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ulemniqm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2umfrofae.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2aohcvawi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jphacakz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hpktjgfc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fzemsdci.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2nffpklre.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rqgwldgy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ueglxgcq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2mdmwcpgx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gofpleqb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xrndwmgv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kyteuncf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2eosupwqz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2qujgmqnf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kutpvszf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zuyigbjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tlkacfji.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2jxjvfedu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xxzydpyz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2vnwwktuz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ayepggxv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2bntagrfe.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vhrnfxye.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nnzixswn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ofymrtis.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jnpbhbjt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2dqsqlyhh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2pjyainyx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jmnxewhj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ekbegcek.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2eyxnviuw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ezsvmfro.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2emxolnew.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2xjpowibn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ztfobdjy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2cjzkygih.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2wyhuptfr.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2vvedwlip.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2cnikyhxk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2oggsvpzx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jqnejdmd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2npvpkuhi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2jndwrmac.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vagjfbfw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2xrsfymcv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vmiupyct.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2hlqlhzdg.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2mqcestbw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yzmmzsyy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hnftuyss.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gaeciofr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2patdmxni.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2dnxrqyda.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2szhtfahd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hjtmlhjx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2pdydjaoy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2xgctmkrb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2dduzsqut.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dvhxcagi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2okfwhsaf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2hddqlffi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2prjkqfht.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2gybnzcmv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2agyvzcsx.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vpxsbyip.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ctfrwqas.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2narokfrl.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qwdnrgao.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fjedmbkh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mikrglav.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2umkmqwae.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jtbfosiw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tjmghxbt.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2iguqhhtu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2podqpxyk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2mmmpysfs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wttwuhqd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2arrjxtbw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2mbmuhlzl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ajktpvxm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2cpmwsmmw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uykajdyj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2hlysctkk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2hecikwfr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2mldvhour.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fdzepkfu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nzmdhrtd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2aboowjfn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2heaqndqz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lnyqbxqt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gppxxdsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wecoefyd.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2mzgdvubj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cyqjiefk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wpfhvzyj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2lszsxmtf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2arbebyod.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tpgtjitc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrdpvqsd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2iezzlwnz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ngszoale.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2eqbddfmu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tbglewsk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dmefoibs.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mojsyhob.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jdjiduct.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rfozjvtp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2luuvrcba.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gdspnnqi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2geowbzaq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2mgaceric.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qafxeuob.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ndzkhavj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jvttlfmf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2mplzmxnv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ckjohetc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nnbhjfcu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2krkawkqp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2toitbzvh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2savqubel.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2mohbdobn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ozzqatnh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2cvkwnhpx.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2hbgflbpc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gwzdriwr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2liztzmgo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2xpynxjgm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uafsimtu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2nqnvpyrf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xdlkvsra.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2orwullge.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kkdcjfpp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2mckgxrub.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jqcwydtv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2loewbbnu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bwmkkkul.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmmkbumc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2kesgslvl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jlqhdunm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2gbafbrlj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ypoqwibi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2albpgewu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dnrjpjdf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zsiuupxs.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ewiirbmx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2pqyqmebm.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2dksndrsc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2tmemstet.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2tolgyzuu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2sdmreroh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2eibjwtoq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bgcqrosd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lkbqhvrj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2pnpdhcfv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zbdfzcri.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ewmceswz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2stvesgze.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2qwxdhfxp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2hplxxrxu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2adjatdpl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nugeqbbl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2gsvgdxua.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2dwaiysdn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2qdvklrpw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2cwrgwnqs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ekhvtobq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcwfmnwl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2gboqfybp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpzafyaw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2viqrahuo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ilzbzbqp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2anxxkeso.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xsrzpglc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2igavhtjc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gokgbrqm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lymquvmq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2vsxnlmvh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fkimxjgl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2tfootgqh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fvqbwyeo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hmtdhzsu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vrqrzfxf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2acwelqah.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2utavmncd.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wjfiuxgk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2cxxfvqft.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mdjtsziu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2cdvpigfr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2inhisvlx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vkvlvrkp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hppebkjy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ajnpmrnk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vjqmyney.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2udghjfaw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2xxvqtlhg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2hernxmio.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2pziyjkrg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2khmrhgui.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2eydkrkzr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ajjtsqfd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hetjkzug.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnropran.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2tqawfaut.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vzfdhxdk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fehlajve.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2fnqcqeqp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ciaislyd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nejvyjsz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2yhdgqpyh.html


<!-- 参考信息 -->