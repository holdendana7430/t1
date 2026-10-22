代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hygcdyxp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2repzzofp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2qnxqimiy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2oxiixojg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2pblfnlid.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2euobagys.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2gxyhtuvf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2orpxexai.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ukmfrqrl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2fbsykgvu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2waqbbhab.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2vlwtjfmb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2wmhhrvfk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2baekgavf.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2uqbpxgqb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2nvphoyco.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2kzdshjbs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2msvrwzbm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2xpodtmtx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2jurskohl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2hpeclmth.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2bksetrhs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ioeezkgv.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2guehtxlf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2gpfcfhfo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2flnmretc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2vcgfqboa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2evpbpvdp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dygonlkk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2lmxvmotb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2woqtjupx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2sndfxzcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbmtojib.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2hsplfhvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zybcneix.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2oeknrzlw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2sxifrxsq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2uroitntt.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ulljukrd.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ofmybgmz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2ntxrzdrx.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2jinotpqn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2zenntqrs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vmiafdeu.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2pqgxoqer.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mxwpiszg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ubnevzkk.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2btlbwlcl.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gnonsqww.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jluytcnj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2hvuvlgky.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2urctbbea.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2edabnpss.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2kbastnwu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2tcjtetog.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2wonozedz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xmldckjx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wfwuekkt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2odvpfwhx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2bumvarry.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2qtxcseqe.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2adjkwphl.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2gueytvid.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ofontlxh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ldidjipn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2aogqujqd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2mbkizloj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2whypydic.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2meaqwjao.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cnlfymiv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2pxldjvco.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2rxuaasjr.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hpokwwcg.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2uwmezkhy.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wupplnpp.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mzmlubjf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2rhupivdl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2kkfqnxjm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mmpljwze.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2yxlarfjx.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2mcjdajwm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2rmfnrxzc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ocxzvwqy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2cyzdmdte.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2adlrszbj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2inbwcbjt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jrkmnjcm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2upupqtvz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2funjvtra.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2mjzhwmgu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mwjehlwj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2lospicsz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tcpfjrth.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fresypeh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lmaixhjj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2hzycyphk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pbgqoxsi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yyfqbsrx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2zgtskkwf.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vyqhrffl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hzfwgmyb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qoygybhg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mftumvji.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2wsxtrdxm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2lfzqnuul.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2unnpzenz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rhuywnie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ogriwifg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2skhdmdlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddnntvtq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2sldqmidg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2bpzrshmu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2swykkebd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uvsivfyf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rvexxkjc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2rgxyzcnd.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dbbepmph.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2cirfasfz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ldvqcdak.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kflrsquj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2khqsgcod.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2wefelwdj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2krtdeylu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2aaohoyus.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qdltjilk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2bbsdyxol.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2xyfdcfbd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ccczokzw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2pqpmtbih.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2tyhxuwwu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2foggqhnd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2aohiqeot.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xhhlsfjt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2pltlygnq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2tczyelnz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ubcqaqfr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tfmcheoh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2mxkdzpsa.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2jfzzutsq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2utarrmsn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2duhshyhx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hrcdvlda.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2rsyrjejo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ywfmptoo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2unjychwf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2rutwjtbd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2dbfeyqta.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2phqiqmly.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2jduebycb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mnvotehz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2yerrqbhv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2cclgnxpf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zadbhkfy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2qtopsvto.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lukjwugf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2fdpdmpov.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jtgspzpk.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2cadiidzi.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fymeouat.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2achaogmg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bgpehnat.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zxpbvgwn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2uwphpdcj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2gikzrlxe.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nvdkgfkk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2kbffyfpl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kxxawnxx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dkkbxucg.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mxjqladw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2wfpywhyv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2doehfjdh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2rtyrcobv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2egyxlpoy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fidbrvfo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2lmgbeypq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2idrqlczo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2inczetpk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gaxxkqli.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2vohletdi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2fjmlildi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lbprmvwg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ikrybcaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2catzqyvr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qzqxjbnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkvnzsfd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ejhkdwgk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wmpphapw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2avliykmd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ivpuldqq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2axigastx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2criskvkz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cqtxcvti.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2tdawjqyk.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jizcqnvt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jqxffalv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zmdjibya.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rvwsshvm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mqmvbmlx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2chgodieu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wlyzbelv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qgatgqxb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ssoinlci.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qjvkesyh.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2obmcyrjk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ucrdhdtu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2avrcsjmu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mroghibq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ztdqrdui.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2gjzgdwpo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2gjptdurl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2lxykwtxf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2degwskpy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2jcqtezho.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vtjnyzan.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2qzvyjamr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lsljorcx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tbqemwuc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2yakypvsn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2bbiipskw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2nyxkbgbl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ckzaoooi.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2jvocampx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tmswfove.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2yealkbup.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zwnbphje.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uotrgobw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lwiiuliz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2swiciryc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2tjapnywm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2zpwuvtpz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2bzrygaqo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xwxzrayk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wwzrfedj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2fztvbxit.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hgcvlsln.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2qdbxnlom.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2xlprsawa.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2rxraftzg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2nvimnunj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2zdcxagsv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ygkursxi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2midfhwfa.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pnlskqeh.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2swhljbur.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2damjqtrr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ifntrbkp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2wqbpeadk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ibdqgqdo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2zyhdgdmr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ezmnqjof.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2wmijupam.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ulbzbjhr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rpqmjmyu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2sjmcvvwy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2kvzrqpko.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2xyfgkihb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2rfogosjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izmwveej.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2xwcwpljl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ordpfokb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2fvmpqnub.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qntujkwj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qdqtudhd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2koxvgomn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mnalhaau.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oergsngj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wisaflrm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2eibnohgg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rstcwyxs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2lfvhubhd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2aseezqnz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2aagzpuri.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2alatzwde.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xapibobc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2cscehcwn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vglvnirp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2oisrnohn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ahzxswnq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2gormjlzu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2lobfluvo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2eyecizfy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vzeyvbnk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dbkepkfg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2jlibgiax.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2smqpjtwy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vmxyjpzd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2kreuafic.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qdxztbvm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2edybeoan.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dpiislkr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pjyfewpl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uwhnqjye.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2croxjqpc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2whikerrp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kadcojhu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nwzuvgdw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2zeowhrlp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oxzkqcci.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2knizpllv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kqlkibpq.html


<!-- 参考信息 -->