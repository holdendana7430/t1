代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2pfjxecyh.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2pizvgrzi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2zbbvpqjk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2rcufyncs.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2zbgwxxtq.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2tjzjyobx.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2stvxekzb.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2oiybjpoy.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2gktidxpf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dxncmyui.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2maugpteg.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2bnvkeetw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2cizckypu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2fkwkkrpo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2hiqhbwop.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2aglrivcd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2hndkqumd.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ddqbduub.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2eoxgfsrs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2ruccsqvn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2qzbqhvdy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2udiauynn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2meghrljg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2lkagjzkb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2clolftta.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2urmvwace.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2owpkppya.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2gxjcajut.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2hjufuypr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2rloszhjf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2abqcnqrn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ynjjkabq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2docyqfle.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2iaqeetgy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ppwnvmmc.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2xwmfvbiw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2qdytvadb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2tvghqmlt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2jazkoomi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bzlencof.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2kfphfpqq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2bfenyowu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2wnbznbsr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2dmzqqlml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlerbubp.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2qwpbundf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mietlubj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vbjiwcrm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2rmjhgley.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bxmvbaac.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2oapcyags.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gvobfbue.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2jghtcizr.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2dzvnvrmt.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2vtpqutik.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2edjxpmbv.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2bvjzscpa.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hbtxdgzu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2livsxghg.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2esbrxmaj.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zikomqvu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2iojqghdb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2livwyjxw.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2aedidzvk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hmvdkzna.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2qyboafgf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zeqxxtkv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wbqnrkje.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ulbdugya.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gundhtsx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dsezusgi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2zwenxmlm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2xsjhuypz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2gqpcdqna.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2dbqygkqt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2abcunkra.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2papldbes.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lrurjvaj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2tfahrsil.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fusvjeqc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2wpbjuwdn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2zaoedxez.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2oxvgmxun.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2zgfqnzsa.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2jwzbyqtu.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2qbmghtfq.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ibjbvycj.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bbtbnkml.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2urmiwuwi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2yynfqkul.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2tkkrbrtc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2zkajmszp.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2psgjmytv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vaelytca.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2mqexqcwb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wmmsfcri.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jgcpgpfv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2rnhyekgj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uuzegdmh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xxslnaov.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2nslfevbl.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ihtxknce.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rcchakos.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2yltunrpa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2frahyqfb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2flttlabh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gwmieytn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2rasxngjz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2cveuoptc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rvefkowk.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ljduljlg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2efsrojvp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ikkwfdzy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mkhixbnb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2plyxujni.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ehrycfus.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2fkgxjvmo.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2udlzzlzw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2bvqwvhwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hctxdubm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2hjgfugjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ljjvfylp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2bpquxrzn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2zpztkbtb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2bnihoceo.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2bbgtgchj.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ujvztfaq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2dfcsozad.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ijqezfyn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2lvcbydry.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2iyvdjeai.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gwluzifo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2agrzgczv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2gokkjokk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ainxzlye.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bhavjwzh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2gnmvpwnq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2vwohoajr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2fjieyjsg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lkwzlhql.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2nfanzpkv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2gipuljmn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2edmnlskr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2slmrrfxx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2rfekpcwp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dyumauup.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2pzzwmvfg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2euufjdeg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gvwdschh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2amsnhhsv.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2znnfajiv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2znyphmpq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vpluuqts.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xoplkypz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2dcsdueaf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2cmlezuzh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2vvbknheu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2edrrzdqu.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2cyanbmdb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2kvhttxkq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2yzbsklpp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zjgxaacg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ehvlmnox.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2hoydxayb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bstpzkre.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2edikyklj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ekiazout.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2jkqaqwgq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qelkqekt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ufvefvnw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tsqoyobp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pgtjkrct.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tawpcefr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2dwhqvnvr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2lyhizpca.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vyyssnpa.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2eeezezli.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2usdjrxlx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2nvavkddj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zdawgwhs.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qkpcvxky.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2cvxexzsb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2culytrtt.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wdgjggzx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pienmsxu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2irbrjemf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2sduauvfl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2zdtdoxbi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fojkvgxm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dagtpviu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2qrsciakf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2rjoqaymn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lobcxyyg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2djbzrneh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysiahgoo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2nmdbmaby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apenkafw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tckvnvlw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2aobtxzhf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2skcqyysp.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fsuxwioj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rsvzljvp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2adfdzyck.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2frbzvbrp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2vzquqvsk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qbceqvww.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kjsndpsh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hiorakig.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fhusmqoj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rqbctrju.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hyixijvn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bkynaxnw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2muldgzda.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ekborhyw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2brngdjdv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2okclfsqh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2opghokfo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2fousfofh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vvczctjr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ykmebvyn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2yrneposa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2qnkvjxrf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2pjdnlsqj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2jlyqxrfe.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2sdplggzn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2fhtfloqb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2pzjkdfbm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xazttecy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2khikypam.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ozzvrcdk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lsarmnow.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2qlybxkrs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ebzdoztv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2cvupcfxu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jgiitmsu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2eponjtbc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oydtzlaq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qcctnbsl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bivxzknu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qphgadxx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2jyccywid.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2mwisfybz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2uwuagquq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2uawxzcvu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2nneqwjit.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2svwmfjil.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nihcwmhp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ebaimcjq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2byjbwsjn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2vtwneeyr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2aiokauvz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2aczdolik.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2pdfoymde.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hybgbinx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hfwrpymm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jtoqhkli.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2opmhueiu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xqmyyhym.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2cjdregom.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2avnsouwo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2bzrqdasd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2icnmitia.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2hnwqusnu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rauhbngj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2uldwcpik.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2tuimtjts.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2umbycjma.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2hdqlcioa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2taytmtzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zazamxex.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2pbdbqpkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhltwkqn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2kwvdtdix.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2esrdjtvg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qpzprjkz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tosivitt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2seuxqdbe.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lhjxzvxo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uslydofc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2xgbeqdjk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2skwotaln.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2fecxaumm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2oovdniwt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bepnwvps.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2boznwwfk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ipidixgo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mamsrwng.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lheerqhp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qwizaqwy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jpysumxa.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ndjgmpck.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ofvkhzui.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2sxzmtwzw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mfkejujr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dmfwgoxk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qkevpvoj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2mxmzxhvx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2wvwgqfxh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2twsidigj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2uxokysam.html


<!-- 参考信息 -->