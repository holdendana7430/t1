代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ujhghzjq.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2znpbyswe.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2bbmlnuvs.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2wvilzkoo.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2twhwvkwa.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2gftbmbzh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2guxeayrn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ylgytnqo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2gspyzrvv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2tcaavetp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ehnixtfj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2faqdxqrl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2esplwbdt.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2nungbymj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2nwzmoxus.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2oaeeauoy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2iehjxxrj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ikobemqn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2zejrdxik.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ldixmjds.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2xjcvtajb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2mxfdjdwx.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2mkwgxutp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2lraayauo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2ypuinbdk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2fmaiktyo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2tdpekxcl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2ptlcrqmb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2humciijo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2eakzoxbo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2vettfbqn.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2cpyurczo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2jhtpeuyw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2sdqbvxqc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2uavgtoed.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2yhceqrau.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ormooxen.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2wkinikbf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2ecwlzxrb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2hlygtqfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmlxsvux.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2jezztrsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ilgpwxvg.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aovepbuy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2koegaaba.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2mkeqsfef.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2akgiunhx.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dqooixns.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2mowqrkbl.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2owyrigfi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2abpkeifp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gwayamno.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2gfdganez.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2sqywjuno.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2gnmbwcae.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2chkfwwts.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tddeqhmi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2sfxsvrqx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ylzrqcin.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aodrfoor.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zvromqkt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ynxjypne.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2vesehnll.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2vvynyxmi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hbkpgtqc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2lzoqnyay.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ggheearv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2jxxihdsw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2ododwohl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ckbrbsti.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2vvbigwzk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2julzjqdj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2agshhryw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2msjpkqxn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2aaqfvgbl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ayfibrvw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2uasmphtw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jocnulas.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2plthpblu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2idfvhvvg.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2zxkmnkhw.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2lamuissj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2oczqolry.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ogkrbivm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2xjwagukw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2mgvdmjjx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2drnvekqq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2bxakpboi.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2bvyawcwc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ixrsrtjx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2rmrlwzfh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2fhwyzkai.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ttcqpxxj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wvpfhpup.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ttnejoaw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xtskavtj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jixzgdyd.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2lviyendl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ouvvcyfa.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2pxppmucc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2akmcnklb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lqjzonzt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ovftwvup.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zilkqdtn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hhjjqbsi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ekgubexv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2cpgeinns.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2bodtqlso.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2rmygftsi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mznetszl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zptocamf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ngxawxdm.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2utmfabiw.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2imvgahso.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2nryieelh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rapbjbba.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2qwskdmbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xqvqemiz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2wgzoqyvx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2dtcjlztl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2dykqcdbg.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tvevmwqc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wdpbqjhm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2zwtvxjsp.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yaxqmryb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2eoniyaxd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ifjsblui.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2awljyybw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2mqissgrk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2rvbxcnrj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2junloeeh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2glunzxnk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2mcejsybi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2lughdgcq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2wjgwwrpi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kghojsnd.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2mthuojbi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2umuekyxl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jhrmzdtd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ummiizlm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2usgkxeqr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2qsedpowr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2sxsflpgl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2awulpqan.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gsjzgchu.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ngiymqxt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2xmqiuzus.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2yugodrms.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jznqjprb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pkscynqo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2znnqgxwk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2uobptwwb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vlcwscui.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2knxuevct.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2nwtiuels.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2lfzocjdp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2nqypkjoz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2nyeogjny.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2pobfcxam.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2nxwmrrjp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2pcljezbg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2mbvspeev.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lpffmgmh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2zxnucbwv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wtanbjkn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ntrdmaaj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cgmztlel.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cctlmdjh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zohvnhtg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2smgxzugi.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2tkgxiuup.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2wyomvtob.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zafqvmbe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2nbhsjjle.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vdfvmojh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2afrafchd.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ykjkwvkl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2eydtgmip.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tlmtqoem.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2kiolmzap.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ovakvfwn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2cfgfaumk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2clgzkooa.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2wfgsjvfp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2btwxxlpl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zmbeishj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2qrcfphgu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2jxwpiuwb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qbefpoor.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fswexqyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2puzhbqwk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ylhohkky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmfewula.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2urrtpxdj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2tltnvbpn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2pbasmxac.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nymffxpm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mdvnocjw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lodllqgg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2rkiajbti.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2lhfdvkua.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hzysuaxp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sgeheirx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ogwmomeq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qsdyllpi.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fvtjnsdh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wpsvokwh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gskbtbpl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rrgcbvlm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2xaswtnsa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gbbakvac.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2rkurjgqj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2oxfhfhwo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ldxesoje.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lanfeutf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rzjomqdy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2cnwwcxfb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kgskmjaz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2xhnetyal.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2xjmayavw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2hogfpccg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wqcabtdv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2zmkikhfq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2toaqqzah.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qahznyue.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2pfacxjyh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2rkorsqua.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2motteaye.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2cflbnrnw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2byuweiok.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aklitpyf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2mfxyqrbt.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ranxcvcc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pekxvqez.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xxqmektq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mmswohpt.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2wcaxormc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dunleqdn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2kcnjqjot.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cbpiyqtc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2figymdjs.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ozwqhpus.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2okpiebab.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gspdnezk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ijvmiajb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2dloebrcq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nwyyfoqb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2qgutfjrq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2bhxllnhz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2czesbhyf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pfriabje.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wmfvovaq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kyutcmci.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hcitpxwm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2xyionvlf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gveitrop.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2jkqtoujn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ipzwrzrw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2uvzkgshs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rcfcdokz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vlktrixz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2brxpbdgn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2sivsfxiw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gpeplmvx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2tydqhryg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxluetfr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2intymkry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyickjmn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ugwkhfmb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hfukbqpz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lzpuapyd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tkodgvuh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xdimxpgf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xeeetqul.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ohltxulo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2tbaxpzvo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lvhfytig.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2arcskbbh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wexheags.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2haczkiwu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2whircbhd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2blmnxaed.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dhghtiqt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vhvlukfi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2sbzutury.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yxudmevc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2jovmkvwe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2beoxcrbk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2lcgpagoe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2funeddqb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wdqqqron.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ewumnwwh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2caneorti.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2sbaeqoam.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2zorqufia.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2scmfjlzv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bzhnibac.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xbgivqbu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xbonohii.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bfsbelru.html


<!-- 参考信息 -->