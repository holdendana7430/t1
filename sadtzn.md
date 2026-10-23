代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dmcpbhjf.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3duyscbdx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3vchtwgbp.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3dxaqosmk.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3hleilhnh.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3lfxhfkrg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3mbffbnop.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3cdkouljb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3axirygsa.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3upqsekjl.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3wbgegnvz.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3xlmfnojw.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3vugevxtv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3exbcslvl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3xirccnms.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3pczxlotf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3untrjmxz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3reydxikf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3jxkwcums.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ffdxqbjf.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zrigqvvn.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3udannibl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3gamrgipt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3vzbaofmt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3ncjhaiwa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3precmaya.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3mhhfzcht.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3asrxhkrn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ycxiupou.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3uxhdvbny.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3yfzxdueo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3lpjugzyu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3wxsjqizw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3bsocwzkx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3sniyapwv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3baenjwpe.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3nogvpcga.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3btpxwnjz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3xjxkissa.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3michlwkr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3fiwjutrz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ymfdoduj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmopbgzo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hwyvkqzz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qlkmpnlz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3rzezvpvw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3jopcupeo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3uorrcfxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qssxdnjn.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3ylavrrrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzzlmlcx.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3notswzxr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3zwxamrft.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3sjbnrrvs.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3umnzzflz.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3argwescj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3rqmarkww.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uwwymgqw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3sofsthbj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3swqyxzhq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ewklbpoi.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3neatbuiw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3uotgiwmz.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3swfgmbox.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3gfoqcxfi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rurawpem.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ixmeivfn.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rjmammod.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zhtaapkw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ynyfiihf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3qreyfqcd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3svozrnxp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3bttsetys.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3vvyzsxrv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3vljeypba.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ihdjdkgw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rmzgyrdv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3zcwrcjiv.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3neaisnqv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3yehtypog.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ktlxkikq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3duydinfd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3pvdfdzvh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jounbcvy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3zzkqpoir.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qhtwxnqo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3sghvvrok.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3xyyjullt.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ryqqtqop.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3uakctwrg.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lerahpxj.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3klxwrozg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3eaefxfry.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3jtadyzxa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tcumjtvc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3dolkyrst.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3tvnlycaj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ohsrypyi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3eqphqvjv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3zcbffrro.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wxbuihqe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3jbjxqtam.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vcbuscnd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3soejkvkr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xdfkogkc.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3wpnqjocp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rcmopcbf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3jfgreeiv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ttnnxxof.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hxwzjzcf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dbgwkgga.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3srasbqsa.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3ygwvfldu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3osuxlonc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3cmermxrj.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kshrldpa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fpcoisgm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hxznjajx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lopnoziv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3eekftltq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3iohhbfba.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3otgzxdea.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3egfvsqia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yexxgzyf.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3mlribvox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omvtxhfb.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3clnyzyub.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3bhonxdde.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3xamoynen.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jnfwksko.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pbovsuwv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3xptesxfa.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3umnmcpwh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3jrsngnzi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ghgkywme.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hvzzdyel.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ghteighb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3sfcfcwvi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3lxmleedb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zjcrusem.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ouixfgcy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3efraewnd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3qhpwbids.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ytfxuqyt.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3odtahcve.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3feixkamn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3yvbmnldj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ocykwggv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3kjqblecr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3jcakcepm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jjsirbem.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3zbhszanq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bvzyzqyb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3hobamfqv.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3rlnvqvrj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ijvymwlj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3sbwrzjkd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ngdwipxf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3psgjmcqf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3mkjguxop.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3qdzcqhsm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3pngggjbu.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3gswzqnlt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3qmtuuzir.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3jqqhviwq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3figvotka.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ogfsdoow.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3fnbqotjy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3mqoajgdj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3pdxhrbjy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lggbwipe.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3utuecwov.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zccpexbr.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cnpzpskq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ukjhrlva.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nhusfupl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cpowzyko.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ukxonezm.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ddnupfgn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jholixew.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ozjjtpmg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3trxqjeud.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ankqolad.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xbqxqinx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tyhnokgd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3cjxxpnbn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rlnytdqs.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vqvqgitw.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gywhgvfp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3jrnolvnb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3tnhtljuv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3gkcamwae.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jmkjkxjp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xddckshm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3aldnqwpn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3saxmakvx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wfoiizmv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aotciwty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chbunheb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3bwcfjqzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vdlffyox.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vpgmmmhc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xfavlatd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3xltglvzz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfvjhlbp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fedpoepp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vuvjidpk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3zbjdrrlg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3jkrnjwav.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dwpckkif.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lxxskpnq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uxlpwpqw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qsnsaiiq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3uvbuudia.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3sftxmkfz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ejezyshn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eaukldzk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3kuatkvds.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eonxomqs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3wrbsxawg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3csxnckyl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3mzqyjkpn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3pnotaflj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xvkvyszr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ydzkanjh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3hrgzcejh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3anjtuhbo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3jhasisxh.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3slpziteq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sckmlvqv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ygvzwvax.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3aqfhiiul.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cyvusnom.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hzgfhwfj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3llrwhsws.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3pjquqioa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3rlvvkdfw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rkffjmli.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qpjdlihr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ksbmhqok.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hpwfzeca.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lyaocwdf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eephaula.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ofnjpktj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3mcnllkfo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3peirgdzz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3kfsjeghb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ombexzco.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3mbmuhcnk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eubisgau.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ozqunvaj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mkjkybji.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3isyjzeac.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3yinygpvq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3zogcitae.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3fkkecznc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3elgjxagw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3qtxwhphb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3weqeltgh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3nepiixix.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3gpobaxsa.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3dibcfsbi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3zcpklpio.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3tiujxxkk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3qvnhiura.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3sxutfvnt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ritiwjtx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kzvrurup.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rxmjvfze.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3aebggsga.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3pyulcxjb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3lzmfegdb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3dtxpthrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3buorsenm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3rnflisca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zamxpcwx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3netyafir.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zhkejwzn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mnsxmwkh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jqmdmzug.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pnrnqtng.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aldkklas.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3htwhzbde.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3zwpfykbi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lmzexdzp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3rhnyojct.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xoxsqkzm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3revskugr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3igspgygv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ctjdjlod.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3pytrfjlq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ojhvqpsg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jiaviwtn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3bptqecak.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3gtpinfur.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3dtvgwzcj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3oqbofimt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3nxlhkmcd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3aehujdzy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ejibfvll.html


<!-- 参考信息 -->