代发 wailian999

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3fbhbwjjv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3tufkqspi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3eqkrkvvk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3fbxyvnhl.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3bysxfwor.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3xxdavprm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3jgxwlniz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xpgjhlvr.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3chtcnxoa.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3zkxkhwdj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3emtfpdda.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3gjcocuah.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3vvoyonfs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3xgxoebnl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3lnbqqwjh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3bhbjqgai.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3tixnxjkx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3tzkmzgyb.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3vucdkpxo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3pyxabgze.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3ijfrsaod.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ktzzmyti.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3qsadxyal.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3tvdudiyx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3gpbqxbej.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3jpwdxnzj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3femjrmdp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3zmxpnpok.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3zjzwqusl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3pethdwse.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3xtdfjfte.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3djyjmcsl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3gzarsjpd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3slzgwrhz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3umoiyvrl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wgvbsojt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxvpgszf.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3svtzycuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbjlkask.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zcxxrfzd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3lgppepxk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3klyrxbqw.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3gonfixni.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ojbyiqhr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3zfxuykuc.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zmcxdllf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3pblpgirr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hdymzvub.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3mouyiuqs.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fknuzbkv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3zdcdvcct.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aoxoqnng.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zptmueat.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vmuvgbrb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3cqstbgcw.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3fcfzduum.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3krcnzulb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3owfdwsug.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3zwvsipnf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ynrtrbmw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3jmdzodse.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3drkupahj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ftuzauvi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3hnzinjwq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ektsveej.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3amhrvhus.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3bqawfuai.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ukcgvfue.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3pnttcquj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wdfnarfw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3xxiktmqp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3mjkvprva.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3mbnbcayt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3smtomblu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3cvkymsjf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3dzcftxxm.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3phxzegdg.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3lxoevvlx.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xipwyohx.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fmvjfrij.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3hsahwvzy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3mhyohuon.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3zjikqlfy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3icvqjhpc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3lbwhajgf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3dmlhpmkx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3hnerahvw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rlqekslc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3upvdsmeq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3egvojpdu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pcuptrps.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xywxloxu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vactfcqe.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3pznvsmwa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3movpucai.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3berdtfal.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xikcmolh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rbpabxtt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zomkhvif.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ytdyiifw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3bhghlxbr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tqdqgsla.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3bmzzlcxb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tlxsgmnr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3plyaqkbp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3npyftsar.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3amjbgoom.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3riaqbpfy.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3wukdisqc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ybgbwyaf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3pofpfdgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bzkdogpe.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ytfgscfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfutgwlr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3xtrtezru.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3vndypttq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3mbnvatra.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3schigqag.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vwjelquh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3pxlrrfbw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3izecpogr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3eiwdudsw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3aepojspo.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ejjupglu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3esxasanx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3tshjcokv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vhbnnsbr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3dnnpuymr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xqxyrkrg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3htawfkxx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3oijvozjt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3howuynzi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ygycncwp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3nytvpwim.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xyqqeoke.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ycydgaqt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qvfuikqq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3pzcxokty.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cblgiohr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3cjwrohgf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3wiaajlcd.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ponjimni.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3tjzkszab.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3oypehrud.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jsdxsdpo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hofxxhut.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3hirmvfeq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3mlejfnvg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3kvqmqjiq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3knvvgshd.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3aphxhthp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3jendoncs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3pntkkfdn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3glfszcoc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lyunurdm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ixvoqclb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3sxzholtw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ymhfqaid.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ynwkagxr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3lyerypam.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nqlnrxhq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3otmxnjdt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ftwmwnnv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3autoozqu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3aikctmlj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3mloydblq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3pugxvuzv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rviawcjc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qghegkie.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3mylcdfqy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3wnrkemzm.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tvyfnbgj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3eqrbyzuk.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3hrogybgk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3znitceol.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3xfrxnimg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3brnyvowy.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3vwzvflwt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ojogilfr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3lipgzicc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vhyjoumt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kmtfwlbi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3npuafduk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3umzorqcz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3izplbgut.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ovqcvxjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wggpvvga.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3hmokmihe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ergwnqis.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ldbxoupv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3utrssykh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3aydfrovv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vpgqbmmo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cqpssuum.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mstdjbuu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wcepusqa.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3syxabptg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ywobhaka.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ngsjvqtn.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fevseiki.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ntwjeauh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jwlwukio.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rxstbbaf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3blzfkyji.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lnnigzln.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3qrnrfwdi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wyriiksy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3zannjkjv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3enaslhzo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3oqkgmcrx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ajgkctto.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ffrlpucu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3qrkdgspi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3mjlqmpks.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3qkrjhujg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ebvkamhc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3rmktxumz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mjmpygfp.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xwgdkciq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mthcrdgc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ttlwktuw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3xxravryw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jhdnzkok.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3keouwnod.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3xozacspw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3pvvwbpws.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qyipcozw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3breeygpt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zzzrhnsf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ogawmfub.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qguzzzrh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3whlwcxiv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3bisifjcq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3culqtvdp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qzsvbyrb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3aehqeqit.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kjhmkpcj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3cxpesurk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uqcugdtl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3chwqyyvz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3zzvevsgl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3zhmyblrn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3acohxmjz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3iodqbhag.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ifekxtsm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3dsqdxwak.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rnfrzoye.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gfdmmqhl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3fzwzjqbm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3zzymjrmc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ynjufhoe.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zgkdzunk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3srtfussg.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3hrwlgtnz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ahmsvqpq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jyzzodag.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3erlljbgi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wgehjbym.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3zzuqukks.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3vybolrpi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3dbdmbkvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfjenbzo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ehoypcfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3owxmbycc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3svhqlkfm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ygjcjoss.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qleeypgw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zdqgtnwj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gdvzjvll.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ccnaoctc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vbjuamka.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3bpbnlbqp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vyxarsrx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3upboycfy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nijoczdp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3cmyngley.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fvyqvxmu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3roedbywp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hulszofx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cvcyrszm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3polwevah.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ngtffbyk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3pxjnvwet.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3viatrwpy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3jmxkvtvk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mfkkhkld.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rfjwqypa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tmyocdzm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3yuapqqao.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3fscpdzci.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ouwvsjdg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3zulwskop.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lagjuxld.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ubwaqlex.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vswcliqt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fqoqpyjy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ifcflemp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ddfcdswn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3otmbbukn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qalclned.html


<!-- 参考信息 -->