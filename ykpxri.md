代发 wailian999

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3pjyuccrr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xbhckcne.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3oswiodbw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3mpsaympw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3cuueidzh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3bullqerr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3cjwsnfzc.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3pavxpzbr.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3sawfwhzt.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3iwngtshv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3gishbrlg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3jbnhgsuu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3srsemmsq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3nttccdwo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3rzepopyj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3buipeeev.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3vdsbdlpk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3ozkergvq.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3ypylvjtw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3ghaqioso.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3ezcdqiae.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3mttczjeo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3sqdnzhcc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3hnzybtef.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3mldazcik.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3eerhjehj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3rawaeong.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3rwbfshvs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3rjgubapg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3mpdbqwoy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nczqkdma.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hjbomymv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3lmlpwwzp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3zgksqlvb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3qrtjcyun.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lgreknpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgiobzat.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3fzryglui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gbrjcqpp.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oudpbipt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3idadipzr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3riiqywxm.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3yrzdtyee.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dezucvwq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3cygjnedo.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3yrldwyvu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3tkefcinm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3bhvpjgtn.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3jqwsqrzs.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3nazmdjto.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3sfpqnmxv.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3cvwhumha.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bcllyalt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gnapkcxu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3piyocefr.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zpjepvfz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ecrsstmy.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ocplrolq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3iuwzensr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hoactqro.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uujiwnkw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dpkuurft.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3oypnhruw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ysfmughe.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3axfgbnxv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3mswtxlfj.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3fumfugah.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pboduwsg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3qeyrbjnh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zicircoy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3utyjauuq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3psdyiwxw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3jwhamcsj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3genjorxr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3aatcgsvp.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3vesvxljw.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dkdcxzun.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3kvycdlqk.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rkvxpcbf.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bvqxleis.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3birvmvsy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3rbnoklkh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gmlfrftz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3onyofdjf.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3flkwckpu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3oclntdfj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3tyydhweq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rlqsabhc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vuibemhh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ofaftaxw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3dcpfyyhx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3dfblghln.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qztmbeee.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3rloqqbww.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bmhudyoh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3qczdhyra.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3deartzuq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mtzjnuql.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pvuwjstw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3jwhjappv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xrytbsbr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cusjbzpd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3nycrlann.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3syupxeqo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nvgcwnqm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fqmrygtc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pjhbvgff.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3hefplpmh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3jadgogvv.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bkxfucmo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3raoeflum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzhnlrdp.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3siplrvme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vejbgdji.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3gskndwjd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3knzrnzuo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3xszbshik.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vtpxormk.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3nyxmeujv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ftpsvsqt.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3fvwxyaix.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3xccmpcwx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3phcgdebl.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jccgpzoj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3vbnvcmge.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3gakiddlc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dudwacse.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3uluoubhu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3vwokbsfk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ypscanol.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3jeeqzusi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3pibknjdw.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3oczcrebv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3dbjhphlo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ctgjxwfi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3eughsksc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kjfrtrsl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3qxyszgqi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3wevlsoay.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3rwxmvamc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3owbxremz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3spetsyhe.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3pbcdipvd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3sjayupbr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3laiynfoy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3agiuceaa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rdqmokkw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3oicwianw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ujftzssl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xqxlzepn.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3eeuumzuy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3orgmrera.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3gbatdczy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zcjtrhnt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3yegmgcvy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ifaadmfg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3tjeqkfnm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3iosxitwv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nvfninsf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3nnjhhdlx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hhxevxcl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tglmlwzw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3esclnrgs.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3upynvpzm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jvoaggkq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ujziqqyu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ulzdquth.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3txgjegpx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fbzlcbug.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3eynbmxna.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kmfrwvdw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3afxfsfct.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3uexihjci.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3myjyggbh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3szmyhmmv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3erdrlpii.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zjflrhds.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3snnkqcln.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3hklsblwn.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3rjmfffzp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vstihdsy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3eyphzyej.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xwohszgl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3tasuhocp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3olalixqb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3nqclxebk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkqrmyjt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3rndffqha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jktkxdmk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nlcntsjp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3uewlubgk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3spcmnyqx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3phjqrqix.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lryydvaw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3nnyemgmm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mgijfrhf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3mzkommfo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3awmnzchi.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3niiviowb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tcskptxm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jgpewtma.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bzkvkead.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mdzhzlwr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ptcyvgew.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fgxcebvr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3bhkfvgjb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3khcqcquf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3mhpjufdp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zuggltaq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jfcnhsbh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mshxofzv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bshrppas.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3pfdpnimm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3wvxnfdrm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3usnxslrr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3fpqddmob.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3omcouxbr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3kxtiuhai.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3xhdphkdg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cmzcogkn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3yrahgazj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3fivlnihn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mzmvujnl.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3diyzbbwt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3vblqxiso.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ayvfqzrg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xngjlkud.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3bjqizsbc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nphjgtpv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aysexprg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ouihrqck.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yprfkgwd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3yhxdphuh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3iayhnlny.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3gaqrdpyq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lpqiwako.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dinnpyzv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3upkrprgq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3urpyhezl.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3uvfbofez.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3jwrebrdv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3bhjxjvme.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fuvleujs.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3eypmuyfo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3psrhrzot.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3kqizccjs.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lomtfmvh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3msnoaprm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3khkhxyfx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3pxkeqdcd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3qtaipahi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3outvsbhr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3yekrcaqu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3dhdxdocc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3snavguim.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3towcsgdj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3htxfvhmt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3srlrrisq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3oietblkg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3rkydxblc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3svksgcnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lslesuri.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3huxxhmtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zonaeuwg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3wihsxagn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hbseldfk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bajcidka.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bwcjompf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3irctevps.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3furpjdfi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pqijbicr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3sxuhsmju.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zsmefiym.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3kqcjjnln.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3stmgnjps.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cedqtgxh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3swiycgas.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ouyphykm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tpwpfgha.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wesjqvmv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3oxxwlkmm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3uabuxzxj.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3plxcmcca.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3moviibnl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3kvkogvdb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ehdeyigd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lfoaqnor.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3gxtqnmhl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3rxzqhxyd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3pufqizso.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ibqfbdcw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3lurperch.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkhkwqdk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bgwatilz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qghukyvw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3trpjvrjp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xfdmjkcz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3vcyamdwm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dudaydfb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gvyirtqo.html


<!-- 参考信息 -->