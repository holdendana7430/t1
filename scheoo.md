代发 wailian999

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2ovpqdaga.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2vyojkhod.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2uxhjvoyo.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2wpadgifr.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2puvvxdwk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2hdbeydbh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2jsxmkfal.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ulbodduf.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2xvtyhyhm.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2xerpfoxo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2ofjokhnz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2prgiuxte.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2hrglzstl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2kbmpoufw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2mzwpyied.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2dufzlvru.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2envgqzql.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2kfdnsldg.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2budlroyr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2qdddglcf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2vilxabxs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2odkcrzds.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2jkswcvjl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2cgwilugk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2pvooiyhg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2gmqkamlq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2tjirjnlc.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2ndgukqdp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2psfihdjz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2qlbbvttl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fvcwgool.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xlyekfhw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2msnkeagy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2ctgjytwe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2wmfaozmi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2ayoyuaud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgmumjiz.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2hslrvujf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2onhqoosj.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2empiyofb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2tsqswkqw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2fsuipsuo.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2zebryktg.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gmziuive.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2vyzrvrxh.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2cedygnoi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2hkcazlvh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2etzmftfx.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2dkzwzzbe.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ohpjzpbe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2gqnvguwx.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ycbudtqg.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lrwrxxja.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zyxmrtzm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2huqturzz.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2cwosgulw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2udsnrgvp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2hdktqngz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2uokefbkb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2jozqfqzb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2fmawnves.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2srmpsjbn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tesmnyrf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2vbtwpazf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gltbdohh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2utjjvlfn.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2cwdcrnvq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2tkavnlou.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2bgpwrruj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2raxviawu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yqbavrgu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2svappxxc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2okfschxg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tpfjsjob.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2pcuxsgnr.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2pxlyyoyf.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oeuhnkbf.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2wlgpdflg.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ujhnizek.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ktadbhtn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2sztesdft.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2fwwfztdu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2xhanwpjf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2kjvjsyph.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2lyjpjvjr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2mobbogen.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ixuwddzc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eyfmapzp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2edsnbspa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2bzofhgbb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hrrmajyv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2nkxgqlti.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2flxokoce.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2krufsltp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2aaxjrval.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2klwuftum.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nhawqqky.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vzuralkd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dplwvorp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2uprszabl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2luxvrncx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vqzmpxjb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2dwllpozy.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jjjerikh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2kyfmydiy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2yxfjricp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aavfrtje.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2hhdmxkhx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2xouuepwj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vvvpyfxi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2psxtwtzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmxurcny.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2vajlmixj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmymxczy.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2setwwiuy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2coslwcxd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2oynspogx.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qjtnpkpq.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2njexenyn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2vkhhqafw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bqalblgz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2lihytsxp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hfundrtc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qyddqjmw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mmshzgya.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2viabjyom.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2sbalcuic.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2eldbgyij.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2chmmfomc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2spmfurug.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2kgjkpqtd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zpesukqi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2adtvnihc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2nkjotynb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ttxjaqfa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2syjkjxpo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2aaqmjjef.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2tdkuxlrj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kyebpmeu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2zmaxtsda.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2dmhftxne.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2oqqyfptg.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2sdlndglq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2trjqzdxp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kczdngwq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2klsxucfw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2phzavhxs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2cmctsxpu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ttrkvdri.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2hfalamwx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2qebjphti.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2wtisygmv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2leazhosy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vxtfgbwx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2bckdswba.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2cqfrygrj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2vayqmbeu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2fncqmqpa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ducurima.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2jsbbfyty.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2upegczim.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qgrgmfck.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kdstsubn.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mkdqqvbu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rjzfntqz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2rwqbwxnk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2bpqghgem.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2wzdyssoi.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lbifputq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ukbmerwh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2lfhnemgf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2iieiqxqx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wjhpwton.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2peiylkpm.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2issqftxe.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2mvxflymo.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mzsrdufl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2itxhsllp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2yarqmysq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2uttltyni.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jifebljb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oywgljju.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2dprymidt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2knsckjqj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2cykbflat.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2crlckuyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kpivixjw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2lbonvxjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stmvnswv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2uixfdsht.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ucspwrwz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2yxcsfokq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uyoiolze.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jjohfggp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bthuzvlt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pofitmgx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hygbacnr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rhchhnqb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xsrgyvwi.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ybaycvsd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2mplpzxtm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2degatrwv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ymqfgfjq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dkrqehrj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fgraiqvq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2nuttshgz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kepjjqbg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2vdrtlgib.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iywtzfvy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2vijdxnhz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rwkbickw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tfikwrgk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2yreepyed.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2zgivukot.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2marihwze.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2whtjzqyu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2vhlzlxqc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qymnmofk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2aqbpwcok.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ekiuuplx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rxjrukyo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2wdchjntu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ymofzwid.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hsiycmly.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2yljjemvt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2tjrlvjkx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2seszdxur.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zmrrorcn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dnpzscea.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pxxkilui.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lkiimvxa.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uneqhurn.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2pnjmrzyu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2lvrdauyu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2kcyipvxx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bvspxheg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ekgtaxro.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gozyyhya.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ggkocnzx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ewffdjvl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mcdimuwa.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2vbpoqwes.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qjikozgy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2azjyqcoe.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2tlflgros.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vfnzpftv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ugpyzcyz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bhzorjkl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2tzlpmzqe.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2sbzoohug.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2pmaqspha.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ewcnbqlq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2oniqngcz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2symdwnga.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2yutkjpqt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tsubdiio.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zqjsmude.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2hwqyrrvt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2qujumicd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2kzonwnrk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wrzjvecm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hntvmwqq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2erbpnwpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cztwldum.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kdvupccx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eklkhugk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ufufudei.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yytsdxuk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2osdolgtq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pdobxhko.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2japdzyqo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2qrbeepiv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cxyqfjuo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2jfjdfzya.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pyfyrotm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yffhcdql.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2khwatjdk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yslhvfoi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2agieyxvp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bqwljbbe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kbnvkesy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rpiwvklh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2jgwbwxea.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2xgwjszak.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ayvregzj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2emwlvmvq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2virmhraw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2iigqhwxy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2pezsiqjt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vxrilceu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2gvyuqdhd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2evuxfmja.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ulsfzels.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zwmpihvd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2avsbmpfr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lqiwhkfo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2poickapv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2pfymwrmr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nsdvybdi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2afjlwyhh.html


<!-- 参考信息 -->