代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2qsxkezhx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2fralnfoh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2gnmqrikx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hanaljkh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2pmacquhr.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2qxzvmfye.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2urvnuldw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2jknhcgii.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2hlachqyw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2rbpgwiyw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2igrsinti.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2azndcvvd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2asfyjmnd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2hcesexwp.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2pqebczkh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2svewnabd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2kkbdvpqd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2bjhbuiuu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2dvgcddfp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2esadnrkp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2xhlokita.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2eynljhwx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2lgzzoxad.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2cedgraxn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2dztvzeyy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2dnowqztg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2osavoevc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2prrevrui.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pnyhekem.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2vuhdeprn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2wzxyfupo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2efwkpgku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phxlaakp.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2jrtgfini.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsambxgl.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2txytyuvk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2yfwitnzr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2scypmuwc.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2exibiggw.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2emztniaz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2mfaopirf.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2izepjxcg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2mppjgxdo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2vwnuyhyk.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2rtiifvti.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tlybbang.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2lxccbgpd.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2usfngtlh.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2notxhdaq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zzgctpxv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2rgopddwo.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fcvigdoq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2natagugl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2azgktlyc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2chapszdn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bfzlftuy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bsxckmug.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xjjumwet.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qndgnmnu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2odmpjqwo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2fbknorob.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2drhxwkzd.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2qcjmwiqr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2aewkbvnk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ohrrrcwm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2afkgezcn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2lybxrndi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ophtwhuq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2biropgpw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ltddtfkl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ianqmrmi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2rsihfefh.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2sdxmvjbn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2qctbiwqh.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qtcjavwy.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2llykisqv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2cuiqxcup.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2xijohetb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zkuniknc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2uwdxtkgs.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2vlwntarn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rxdgxwsg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2uprsfzxp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bjxjpojf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dertuvcu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pepixnff.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vmddhmul.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hcrjanvp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ouxxravz.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2vsfgqbpv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zqthysdi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2oeyglhvw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2muxlfpjr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tmhgcfxd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2iepewlpl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ysviheoy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ejbshrjp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vdpreppc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ujlqvskm.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2jwhhxfjm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2olnvabkt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2igxquaov.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bzgbnjev.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2shfokpdf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2opjcbwzf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xbofnthb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2uzfcftjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdifodzp.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2xobwouvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vnsroaaz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2dlsvgeyl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2fdfwfksi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2rotfnvaq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qobxdndc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hsbufwgh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2nsvyanby.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2zbmzrrcf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2zktrdpwn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jqpafhjy.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zvwgpgmi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ynrbhmov.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2btfoyrtk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2btfylxlk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2dmwngewh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2cxojrjpf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2wyvenjag.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2tblwzwnz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2fdgktuwp.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2eoaolsxn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2inkaqepp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2eylvphpd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xryzwdle.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2uomdiurw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2gxgyuipb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zrbqlvxl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2nlxdvbcy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2evwoudxn.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2uitalqux.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2usvdbkft.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qvgoxbuj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wmkqeluq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2afwwzomp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2nbzwwutk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2kevxliel.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2pgdvmoxc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2krfnjqxk.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2nnwmtzda.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2qpiisxqa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2fumibwzb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ashchefd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gvezscdh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2cnjplhbw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2qdyypxga.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ildpfuoq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xyaxxadi.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2kqtgkiih.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nmkrosns.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vshhkxfb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zcbxpykk.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2npghdwyd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mcmluyhf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2fsvfgouj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2rfbfuuwv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2escuwlml.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2raiggpwa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2vjxhdlfw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wjehzgxf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2amhxpszc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2agjndfpo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2eilsletu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bebmgkjc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2swjrqtkv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2iclzxqvy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2pguxuztl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2tqqqeidn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2mhfcpaot.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2afzcklnk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vhvkcddf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ayikfkiz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2sdpyjjyg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hckxcypt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2lbzvpdcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhvtthov.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2pptgdjgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kuciqplo.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mnfdhyyw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jzbnmboh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2szvvhegp.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xbycwjyh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xsxuwobh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2kwnerzlr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ffcrbuyj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2mycikpzs.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dubxofkw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2monjarfy.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2poszfawh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ugcztuyr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zpdguqqe.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ugbvxmdm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2erixaoaa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ymxewfao.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2giweavls.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qkdjxzwp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2hypfwckj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jhqsuyfu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ibqizpba.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wacdqohr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yglwqavn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2qxwprcwi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2avxnbgdf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ihflfkhb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2wipydfvx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2nnholfjq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2isqskuva.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2jkoyghqz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qphwjlsl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bqygrxqy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2tlsxuuud.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2leqhatmc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2roxibfwf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2jvntgtbg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ifeqkoao.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nhccspsa.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2tmxumpad.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xptazmht.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2esmclzsz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2beixrfht.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mqgavdvm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2womqhnpr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2hhcorllp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2wiceetyq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ctlwanrv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rlketxov.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hmllbzmk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pparhmpc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xbbemhvy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2umjqwjmi.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2btmhfhmc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2sgrinfsn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qnnlmcqr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ztyppnvj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2muhvtqhw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2uglmhwfb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fnecbmda.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cubuebnu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2gqdxrglr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2sakfxmsw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2qpdcuarc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2faofmkhj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2drulcufp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2mjhqvmro.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fuotspbf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fdiwiltz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2gwaqvgzh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2blswycow.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2giyfncdr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2bxgfzhki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdevdpob.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2jwqmignv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nlzxrwsk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tixkmplv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zvatlows.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kuvdnflw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hifzprjz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lswwfizl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ftumjkkw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bhduvlob.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2qvqbrzqq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rulxvyob.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2uzfrjzxq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ylizcmsm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yfjwkxio.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dtslheew.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2btayumsu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2lhcuuhaz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nfxdmsuc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zuhsszxa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2oedijjac.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2boceyqvp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2goxnimul.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ywiipume.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fpsgwwag.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xkziztow.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2cwndoqlw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2mdjpqxsn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ykjftjyg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2bowxduat.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2yrvyulzv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ndyaykwj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2epnepncj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kyzyjmih.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ijwpaesq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rcptqkgc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ghtadpba.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wyyeazoc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cxihsmbn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2gayiwniw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2foxrckna.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2fwnbsnup.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2toqpjogh.html


<!-- 参考信息 -->