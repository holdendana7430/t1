代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3qmnyueye.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3yfkrybws.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3lxublohg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3omtbmppg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mueqlqdz.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3slcgxzmu.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3vvjwfoeq.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3rqcyxymg.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3fsultydv.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3jrlgemdd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3wsbppefn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3xpxgezmb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3bamvakuc.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3vetimwzs.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3nwijgyzh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3nmqnnbvp.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3pkzijmoj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3rvbxvwwt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3xayxwtyb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3nveaxcxf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3gvllyrsh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3cxpiywkq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3eexpapss.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3uzvbxmnp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ebxaaaxe.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3dcvubwox.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3sykaeezq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3ubaozylo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3effoefen.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3ttdqcqci.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3gjfrrrjk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3cesfhrhp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3kamgbxst.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3vnvliqzt.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3wqbqxpqk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3dsnodvaz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3xfrwkqun.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3rslgcwph.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3mumpvufa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3suxoyzob.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3kjnggbdg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3xgsvrwls.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3fziclvar.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3yewmxquv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3dbdbrrzd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3bqbkzzpg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tsyqwrdc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3vwfsozeo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fylwdubw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3yxkrnkwl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3iwiqxidp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3rrpvmiwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xfbuzpbo.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3yquykhiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3grgamuin.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3hlvgtpip.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3sjktlcym.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jazsgwww.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3cwxplvtw.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3axcmkuyc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ugbkecod.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xsjrggbu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3xjjgvtwm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3soyiqcjo.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3qapimrqw.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wukkkqpc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3riuwogxi.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mzleyxyr.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3qeqpbmvt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vnpueptk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3bzderskl.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3yeyxbgsy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3sfzgceth.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3kkjiruvo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3zxbofnyr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3nrexgmar.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pktaxwjr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3sturemlt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yvhueayd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3oqyhwfbi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ntfjkpbf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3rhrgivnn.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3rqdiywyt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3nzogflhq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ssunlmzk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ozslyoix.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3prnaluhh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3oaoukuxd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3gvzckufr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3chkskfae.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3irznfkcz.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3oewyjbdn.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3cstgnjas.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3uhilqnkb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mpwpifvj.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jqgisyjc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3qkuuapwh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3gtavhlmw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ntrnjyrq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3olwvutgm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3sejlbnop.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3trdlysjk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3vyhcppba.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wfrmlazi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nfenhfyi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ylndinog.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3pizclzpq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mxxhovel.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3rfxiiygv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3fvcevaed.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zzzjjjlr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3bbtwgmeg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ynurnlmq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3znxglqev.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3serihmyf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3osqzmxha.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3nkhxrluc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3eahdpivr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3znxsmnsk.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3tfybgdqr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ixpaardd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rpbebdsq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3bgnhhopz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3lxraqzsc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3fwldppeb.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3kthdmzrs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3numzgcgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yaxgjiud.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3tipjxxiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkpsnvjt.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3syfitgsz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3tbpzymlu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3yfcheiig.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3njciivfi.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3naenzhbj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3jiwaeeky.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pxzldrbn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ztryaavi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vgbcquhb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qzoebdad.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3dcbxwrrd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ipjljooa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3heizcleg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3lltsbezn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3gnuxmhkk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3infrgfpx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jagujqvp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ualjftnx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3zorvezeb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3sfoppfoo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3orkidrbc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3iggywmog.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lutetinf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ccqgoczi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3npghendp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3zdhuhswt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xagdfgjq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3qnvnoyaj.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3jmstvivp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3msclepme.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3sydfyblc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3kdpcwkoo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3pwvxigmn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3cdqpilpu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3zyfrhmwc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ivxqrdpo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3exmscwpn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3cinekerl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3bfexeakv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ybbrvdjy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vytzmwuf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3gaotxrcm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3frwoiwqy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3znqhiczg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3waporufo.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ixlrygoa.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cgvjyysi.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xcukkydy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3luumkdbr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dvzbgeqg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vuyxviqc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3cdbroozr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3fmuhenvo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3jmtpucmn.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wjutynwz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3powjepdr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3osrvkvse.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pvgwoyhg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jxqposcd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3zoyjvvpf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3expjhfpw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3fglvgvcl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cxoddfub.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3nehpnnvh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3diqniobh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3xuqrwouy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mknmfvmf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rkvctjjn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3snxvfqmg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3hzzpztaw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qvqmgmxd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ocylpqhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3spgdprwa.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3kueafyrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvobldop.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3pyiqhgii.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xswawgno.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3akwojnhz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ahdhixxt.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lvzyuygt.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ecdzhkbx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vdxtkgqi.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3loxmcrcs.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pnzdtjza.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qkkxcvan.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ndrpoylp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3psrttfad.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xvvbyouu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3orcaxpcf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cgojwaap.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dcabusec.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3yrwyndoc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lhmdiqct.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3unnjnjfc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3kzpbvgwg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3icbgumkb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3kkmfspec.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ebqdbvka.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3iwqcbbyz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3rabywjur.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3lqdfsscz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ylbcwhfj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bfzwycun.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ttzynudr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3uwtxgkdn.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ktqoipxz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3reabaemm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ojyxjxsv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qfyouuep.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3pkbvembb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3pgjhushi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3jtxdzptt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xujhdabl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3gvhlgfyh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ahcfwsbj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3swwnckrw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yzticrxu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ygnevyul.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3uktxyvax.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3wqhbtbnj.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3cnltmpuc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ouofnrss.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3idhyizyw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gfvewakx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mohgvqyk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xgxjdmyz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3tsskeilf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3kepiqzfp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wtgpwicy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3hiffqmtl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3wwtakjlh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3cxllqejn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kklbmanz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lzhndogq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3jbtxqnlo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3agtorxjp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3nnondrer.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3uswfdtjz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3sueabcdd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3jhaqovps.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3sukvnxzq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3axmagtmk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3efdmrzzb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3vjuhppwf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3puvvxbtd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3iqgrpxdx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3jybonxra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eucerple.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ltbdzxde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czdlrxfl.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tyqrmkli.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3otqfqeqb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tkxlvzqm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xgzmbzdl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3utmbepdy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rbasoxef.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fbnbsiuw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ezsetcja.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hhboqsdn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3khtgfdac.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3abqaugzc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3aimwtxdh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ajwmgrjk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oayfrpmm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ddndcuvi.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zocwzqfz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fhgschie.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3kqdxzels.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3qzsgdeya.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3aqhembvn.html


<!-- 参考信息 -->