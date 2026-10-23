代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3dhzyqklk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qxcoskdj.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3jnstwnqj.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3vlqyldbd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3bymdmjlo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ixnenuyd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3jnvunkse.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3czhfzluz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jyskxjjb.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3aehvjhpt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3nqvbutvc.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ywhamkiw.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3aiqjpskd.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3ykjzujct.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3qijbexsv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3fevfqnil.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3vijltyrk.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ijmyrdkg.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3xjydiznz.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3clfwjxkd.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ukxdskbi.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3mdzlcnrn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3hccrexkl.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3aptknfku.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3cjvzzswb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3gtvozbza.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3talbcfcx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3svqaalzq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3azrlpoew.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3mvrzuduv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3sgxenrjr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3xxsgzref.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3witzwisi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3adkihgmk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3sauwiubs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3nwybooiv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3rgfjezyv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3kmhrrssp.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3asdkxbrk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3iakhunfd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3vepuyqyz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3mfsahdco.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ergxrxmc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3fyvtyxyz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3swuejmdq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3stqpoqsv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3qgycqbdc.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3npbzctin.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljdtqimb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3azwhgjdf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3iiagfrip.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dkxsxvra.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3sxovpdvj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3lyuoyoxd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3pyckzbwz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3jhbpjgll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3viygihac.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3dtktubpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nucovswb.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3whrtkjjc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3aeajousd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3xqtnwucp.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aldjmwdj.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3nirpbndn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3lspjtfpn.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3mpohzoqn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3avlnchuw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3swpkqtho.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3nxzmmdur.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ngdfzrji.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3bggmnecx.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sifbneur.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cegbyprr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ioycmxqd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gzvcjnee.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3nppebnke.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3igwczjpj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3vbtvczye.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3aqtyquem.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rfgfjzol.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qxbuchjb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3btaoywtv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3yuecmrcl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ijfmuzuc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3uvhkujsp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3vharqycs.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3pdqjiuin.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3inbtchqk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3qwletftc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ohopibya.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3llwspxjm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bhsxkwfa.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3nvheoelj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3eouirbkk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3tnvjyqgj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3duepzeda.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ynquvagk.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3revtbyyb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vjndpmof.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3sniiuccg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ngeixwqq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3ibujwdib.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3elsuhmmg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3ixvysvwx.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3lfwrbdsk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3rinrxsvq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3zllkkdpi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3buhvguwy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3rgwwsahp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3gitrgwti.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pylomxyl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3adelojsi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ddteldjz.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3fwrztgwm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fjxeiodh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3zhtyfsgo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nbhdxscq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fuwvzmwx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3veoloijr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3zspksywx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xrlmspqs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vhxdkcbi.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3qgnftpar.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bvrpsgzk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3vmgbexux.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hlwivyin.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zupjtdyv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3chdnlzvf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3qnhuwdlx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3abxgykad.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xtfonwns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzunjhjd.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3vilvuxsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edqniisy.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3axjtmixe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3nllmibec.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3mlhbnoii.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3knahypfm.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3diaezpiy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3aurtihce.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3exaaqwmi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3xryhgdns.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3obvlmxhz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3airhkzin.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3cujcnaak.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3utjphkeq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3saesxbzt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3obesymwt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3yrckeymh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3pshcckvw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ohnzmgqx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3wijvlpbt.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3fzuomkld.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3hzztshpw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xziuoujp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uddghlob.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3cqtpdyra.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3mamxatfl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3otuvoeaf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3lfuwavgg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3gbnuatgl.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3nuvbecbi.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3uyrnmvmo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3tkjqgdsl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xvrznhks.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wjhfoczm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3nspzdtlf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3uwqkdeap.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3oedmebsw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hwwavezt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3urgqwhcr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ddotchct.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3jguiuxhg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3heolrmhl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3eppuyxih.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3nxqylwun.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ootturit.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3jawgscjt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lnhrmqmc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3clhyaysm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3eifdjsub.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3btchfkex.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wenescei.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hrrktrwe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lnjeiqrm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3zhnxbcdz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3uaublpzt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3pexxifvd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cczlefgi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3kplaabdx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ncgjvdvo.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ywxsaavx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kqgywzzl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ocwsvmbw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lzutzdtc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3dcbinxwb.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mjniufra.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3jtujewnm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3caofkhpi.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3uedwbesy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hiuozhju.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aegswhrp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3umfvoicf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3nxhmmkba.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vnriiaud.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3lmpjanuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ostdbjql.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ijaxeawc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwxuwfrp.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3njjzricd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3qqebuyup.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3pgegxlws.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kxfoenwn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lxfwsxfw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3owunchvd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3kvjsmzcr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3tqxjpwpl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dbmmqwvd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fgbzplpg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dpasibft.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gticcrzn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ceqosywd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ulpzjkgc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3khxdlaku.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oamccjim.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3xcobbgpw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zdfkzemu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3jjckfqyl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3voxoejia.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3thmkirjr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zmgybsvm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gabjssxf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ntkpqwbj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3opmclujd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3wlwauvdu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3irhtkzrk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3qutegsih.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gdtqyliu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3dzcztbar.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dnpqfirt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mhefytac.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3yhzediad.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rztgiwba.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3gkiqbjcx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3uarueetu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3oycwawcu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wilarqtz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rdaacrpc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wulbpwxm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qwdbrmwp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kopawljo.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rnnrpjuy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3wqflhamc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3svqbbdau.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3vrxidzxb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rpgxeqxh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3awknitez.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tatdcfte.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hvmpoqxe.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3gnegyvsq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ovwtcblh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3glkqxdnz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3fshokkuo.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3udnixuiy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3fvpqjwef.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3yvliulws.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jmehonjq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hovdfdyc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tjaxyvyl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3bvgmzfak.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3cwbxymgz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3dngrqekd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3vvsboisy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3eqfaehej.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3wyvfpcbn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tkqvatwc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dbwrdknn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3yvpopnnr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3hqxsnjvb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3oxlddyut.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3qyzwtwgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ykvucbck.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ivuzfwyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cgfrgraq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3awfiwfzx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ywtwipur.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tdstfvhm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nozkeglh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jfgvslpw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rsqnpyfy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tbphmtuq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3vopziynj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ccoimopw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3iolwurce.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3elavydvf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wesswqrh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ikotiabq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qqyqdmqk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hdfoyjsi.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qbfqrdgv.html


<!-- 参考信息 -->