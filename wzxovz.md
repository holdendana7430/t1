代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qwkdtvhy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qhubmsew.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2bzfmheil.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2etszfxtc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2aahtlxtg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2tnlqbobs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2stifcsrb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hsmeybza.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cbrtvvaz.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2uugzuvgy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2zhkzfiff.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2anzjvftx.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2zbiyttea.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2lbxxkpqw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2tmheoahq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2njuwgnfl.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2jusdwjfm.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2rxkxpxin.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2vnmvjcjg.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2cbfdhvbj.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2kmqxlcwi.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tvwjfsbm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2tiftscen.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2kswjkkei.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2wiknhhbe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2mjvrxeyx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2nxtnarji.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2kpoylkai.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cbukpngy.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ucmxftpr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2lghocebq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2jyltiirp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2exwpnykb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2qrzwyoop.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2vqxmaler.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2xfcprcog.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2jseddkvj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2vtvhoivd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2keqxkawi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2hpshzkkt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2jnbiaxws.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ytsowbhn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2pkfexqeq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2prdgfvka.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2nwciohrn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2lgjgeipr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2smtusztz.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2zmtmyiek.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2fxgfupuk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ttvdwmnc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2ekryjmfo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xvbjehtp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2strqssuc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ypcylhka.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2ugldckmk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zjlfpdgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfyaveki.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2qnympzgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2htvievpy.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2opfghxkk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2iznggkwd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2omzwnvea.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2iuirxokf.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2purigwrp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2emrshfpc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2aayaynpr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2mewjgqty.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2hbmuoklg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2uimhnbks.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pbdimamn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2dqbnrjxo.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2sqmqkhee.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hizydhce.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2sjjvghmy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2edbjhzhg.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vufytyds.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nhavuotl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2kumbmkom.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2vlaflpdf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2dvqkiidb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hvdyzybc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xvdnpzxn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ufqidsre.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2eclicsqj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jpexqbnv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2vnydivft.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2pfyperid.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2smbxmxza.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2vdkqlfyy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2rnprvgzo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2hgojldcl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rcodxqfc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2bxbaxlsn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wxgcgghv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lpcaxjcd.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2rlwxjrek.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dwkapozs.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2yvbgwklg.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hiafurge.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ldinjjfn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2bzxjrefg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2swzfnqsp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2abiyyney.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2hxnsatpz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2jkkvdvuc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2thenymly.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2mvtcxnos.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2zsmgkvxf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tcarnlnz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2svvwlxyl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hokwihjf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tibphldw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rjbjwnqm.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2mbzewbdo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vzkfckia.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2luxftdqh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qejxkinr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ysseosib.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jdaasdkw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fprjyayi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bygsvnli.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qpdoeuwg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2taowyyne.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2bgrgmjjt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2fhcxotud.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2akdjdpio.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2hynelfdg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2pwxcxrjf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2poqrgrmu.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gdbjmjlc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jumetghr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqbxgfbe.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2tuprjxaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jrdiktii.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2vkorgwkt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2agptniia.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2yiocblbx.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2eeldecls.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2uhfkjqiu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2saibhlwy.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2stvsmbmw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2phdngkls.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pkpsihhf.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rxeoxnix.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2radxyjqa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2opgtmhqe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2fmqhzcmh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hgkdwpcq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zwzldpdy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2iixyjhzg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2otzqsbak.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gqibyfus.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2lxswwwgp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2jqwifiyh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rcmwiqju.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2yhorhruy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2izfhtibv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2qtsmnmht.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gicvgdgj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2xdohwqsv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2jsnmoscd.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2idfoidma.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2nuzhzfhd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bparfxns.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vrejdxap.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2blhahiec.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2uthllyiy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2dciljwmx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2iyeismhe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bmgiquse.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2omvxnbpb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2wcotnvyf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ydehtktl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2cfzjzldv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tixdunbz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2fujytglb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2dpqcfvzu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2pxirmpuy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ttvkiydq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2evnopgqu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vwsjerhx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2xfuubfgq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yahxthjy.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xtszdqma.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xarmuvag.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2cbilfets.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2dpmzjasa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2qytnbhez.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hosjukue.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2bhxvpezo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2kfeakovf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jswralod.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2cfluecno.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2gakcjtlh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2milfazea.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2cstdyimc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uaefkaex.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ibjoittn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2kfpygjci.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2bhrbthnn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rvligpbn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2eeglpeho.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2upnhizxx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wziollcc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qredcvhe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ugmpvuxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afglnjlz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2qwlpxpue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfzjwdmn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jhwdlatz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yiaxzuvu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2dhluagcy.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2appjxwvq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vdvectqv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ldeilffh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wbewskkt.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2gqhdzmgu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wividssq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2chtpebti.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kjfvbsmd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cyumgxcc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nfuomdmq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bxqwsbvn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wjcqmrya.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zjzotgoc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2sstsvvpu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2axutodyl.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2jtlozqgl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pqefnjjv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2nwekcuxl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lvltmkrk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qkukfqfp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2fqpgitek.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2gsjdswat.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2jamrmgmp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2sqhdlgkr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2jxrmjrjx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2sjflrbwv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2jeefdupd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xzklngmz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pkhqfejg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2mvformbm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tqkavgny.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2lphfqiee.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2gjrowiia.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2redyftzk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qzepjimm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2zyyvsbig.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nvkvujva.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2imntalax.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fdhoivjv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tqzvcuml.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2lqkeahvm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2qjlwauls.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2asegbryq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xmtmnate.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wosswwjp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nptcmcqx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rgkpqckf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2voszwevi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jkbmzzmc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2tgqbpdzi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2hbmbtdsj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2urrwpnkf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2intnedtc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nyabvopb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qfzfwfkz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2uyerywmt.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2heczlgxu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2jecmrvuy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2sciwmpql.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2igcawqem.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2mxvoebvr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2tczsclre.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2swftumbg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2usnrcpfz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qvemjxzm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2fwiqzacu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2njinkeap.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hwdjflch.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2dxlwiwny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfbsrquw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2qxqauxrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlnsliby.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2griwufvp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vdolaxju.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ekrbpkdf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mbnswjdp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ntdbikkv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jmuacfef.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xvqvxltk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2uckwiaca.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2coswcdjx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2sxqripgl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rzivwblh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hkufkuna.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zlkdornq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hoftgaag.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ndeggajx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xjaxzbbf.html


<!-- 参考信息 -->