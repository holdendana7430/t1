代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3tuwlgspk.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3yyyokrjh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3mhidalri.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3lpouvmrt.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3bwmhngpl.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3uyesferv.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3xnqguxjx.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3haeuixcp.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3prerzqyq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wlmlnsrv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3kjqgupxy.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3bsqrjpsy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3dlkwcpfd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3indatgxn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3blxlvtdo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3pjncuwzc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3cznoqgde.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3jombomfy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3pmjnyaoq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3tfinqrxw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3htpyztub.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3fvcnpmta.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3emrftisy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3nyepqjwr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3chnymozd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3ckcucony.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3msmgjxys.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ldgeybch.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3uurtovle.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3wvtdtwkj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3mbcrwotm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3tcrmcpjo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3oydhdoss.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3yasudkbo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3tavrwrgy.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3cwrudhqj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3jvjbwiyx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3plhjbeuz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptgsgixk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3fslykaml.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3goidpokp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3zarnxpdf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3innjndgy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqpqzulh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xoqedwrh.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3onqtyljp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhmwxkhr.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3ksurctqp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3cemcxptf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3threirrm.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3odbuzczs.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wllhxmfw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3qctwrwvk.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yqjcfzsk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3lamftdsk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wseaclwt.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3bfdpxaik.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ecgxogas.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3gsrupvar.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3cppdxxli.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ujdkvqhn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3oshqwhvr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ebwyzizk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cikztuop.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3bixaxlwu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3uwdzpuqh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3htvhavnl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3qolancie.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3mxfbuszy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3lvxspefx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ecmtntpf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3kwymktxv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3nlsiprja.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3qqrnnzvi.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3sldtxyux.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3zgvynvid.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3apmacmuv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tqvjighn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3lhbcoulh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ssnxyeas.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3emmcrehx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3zrfjfvlr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3uoagbeyp.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3rwayegls.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3yzcntlvg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3yysjvsdi.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3yymxhanx.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zjbbtksa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3kfqhtldb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3kjtqlvft.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3mbkxyhdm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3ylzjiwhc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3qcsxbyyk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3shesnzry.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3bzhjhtxt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nbdxolpf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3kwmqmkzh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3dkuxlxrr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3apykwgxz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jzealvtu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3umgaefsw.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3mejijscd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gsgkkkli.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3phjbxkfk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mdicqygu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ckrxlizd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ptxtdzkp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3yoripbaa.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3azmibhzu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lfiacfaq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3wufaddll.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ofbxouyw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3tvglghhy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yjjacyql.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bawnxxzu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ozobpawn.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3mppbqlhj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tgtbzckv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hifzjvbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldicjrhn.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3akmvtfaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrmzfoub.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3bwixqkhj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3sfdxpbmy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3dkqvsakk.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3niglhqgk.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sbtgfjkk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3tjplrzsg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rsbuxizz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3idslxhgv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3mulsiuzz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dasxeslt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3zhowhclh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3vbtikhsb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pxapjbty.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vwmmxnkb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3osnluazq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3xokibeas.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3xucbpcqq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gnkyqaes.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3htdjjyic.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3rqwntvnv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3znckcqzl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3elhmcrhh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3sqcstnjx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3chibrovm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qrmxqrno.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3cngpxwdp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bafzjpat.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3btgofcpp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3sgrmlueo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3qecqobks.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xllhjovz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3glatqpnu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gbxmgqfe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3mjedofqk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3hjtrqkuu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3lxyfewrz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3arxhcnip.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3oldypxda.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3lfelodsc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3cmlofndf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jjhesmrd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3jrjcnuvp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3axvsvvly.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3srlagpvi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aafshdvp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ewjzkuit.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3erxhoeom.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wcgmvylh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3istrdhjz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sljbljdh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3asysdgqn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3xbhuqejm.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3wroxbjrr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3efdhekag.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3klisyzpw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gzuzsmyq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3zodrnlgu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kolfyqlg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qamciuwl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3mdkdrpcj.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rtnrxvgu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3cpngqbmx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mqyyevgk.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3nzlkcven.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ysyejylg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hrvrpeio.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wckanplo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ukyupaqb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3mypljumq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3hrshossy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ytxrnwle.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3vtwkzyci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqwljlec.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ezkvzrfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkehooyk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3olwebquy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3vczzwrub.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3dkxxzuiz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3doovnuvx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gnqropsr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jxjrbrmc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hdrwtefo.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3embbbqqg.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3lquoglvq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mkflzfju.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3btmaesnw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3kffhhkpp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cmwwzmpi.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3diemeypr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ljpnseja.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gwjfkqlv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ikgumkrb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cjoxeyrx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3nnxugvwx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bnlujqeb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3lbalemsj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zfdvwqqd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3anqadyud.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3pukdosxg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3thcjmabx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3zhefmkay.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3pyjairlt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3tnszrerb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ksxnqvml.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3tasrdgog.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sspehqoo.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uihlnysy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3rlhxpkao.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ngiggcjv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3tqshorud.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3thkvzhxv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3pzjpkoos.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zkloqfoz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qykfqjfq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xtowvxwe.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fietlhrm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ahmmajtf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lllufunm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3yenycwjl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3rxwdohxr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3nwtlfysk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dedosaol.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ulpzqfde.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xfwtufjg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ziubxity.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3gduratih.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3avdhvigc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3gwfxtbpi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3hrvzwjpg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3gtqhioqy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3qgrxvfye.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3hiuueqbk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3chbhsmoa.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bqeddtva.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3bxcsmicm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3cijfhgdz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3tdzgwsiv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hgmlpyos.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3rzwzaqzd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3fvjpctee.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3fnvaluaa.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3meinlwng.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ptsblylx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3douwzpzj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3yrgtjtae.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3itplzluj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3vvudwumv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oghpalbp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3aglozosw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3taqaiyyf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zqshbyvh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wmorvrxb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fmobyqdt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wkiwnkyb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hvgqojup.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3viulcrls.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bvqhfnoj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3lpgcmddt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xpxvisoa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3oashhnqt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ktiqplsk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3uxlrogjn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3oeuuoidu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yvokphhj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ikxdzbai.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zvpekwhg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fwikivvq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vjyxftqr.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3fjqvdunh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3pfqfbcmb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ecneusuy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hmevngyz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bzugynvi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hunjrcwg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3zzoznlhn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xwkauncq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3pdpmxqyp.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3mjszuiwv.html


<!-- 参考信息 -->