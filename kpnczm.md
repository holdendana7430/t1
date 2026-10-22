代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2seowiyyi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2pcourbpv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2jbupsrza.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zilbppcv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zlygloiu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2ovdgodmb.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2aovbbwbb.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2cicypred.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2edjdtkbc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2cbdlnfwl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2dkfbaozz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2nfuzpwde.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2icdrcpmf.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2ttxxtbyv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2czbsswxu.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2qaogumke.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ypxfnuij.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2dkkxsxov.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2rwmwilsu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2kdjglpre.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2khewvvyc.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2vsswrcso.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2biqzosgc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2bmvqwcye.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2fydstnsa.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2anxwgxao.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2frrhgjay.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ymuzbrtp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2dnlysxau.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2mxuhygdm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2opteffhe.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bjxiqghy.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2rknmoldj.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2mplkrkof.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2dvzdmwlc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2fjgvxmig.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2dnaifksv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2mhiogzgm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2cpipnhhx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2agfqtezp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2ymjnvxqv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2mreoyyox.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2wgrxzczg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2rylhssfk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2andpazfx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2gqslzomw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2pcoaudih.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2ewyojlkr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2kgmmuqfp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2hjatrfen.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2uszduerb.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2zbarxllw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2xiexnxmj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2jmutslqs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2fltbgtpg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zragisrq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lpvnphik.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2wkqchfiw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2snqkkasz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2llwhzbng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2arlgzrdh.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2dbwaljcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldavrxfo.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2rofhjxjf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2zocczosg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2oydpaxmq.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2iilhxect.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2yqeieylk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2pplfprsp.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ntmzdinj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2afvwmebm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2upbiryum.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2ydplprxg.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yaeidjoq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2mrtyldez.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nsfilpuv.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2qfrqoztu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cjdriymb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2bogfovxn.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ycsoxxky.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dwnawsrh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2fhbdfgkx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2qgbagwax.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2convirtw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2qyrykizk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2dwmhhviq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qikauozn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2oxqzzmzs.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aptieama.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2jbypttas.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ufdvrbwx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2wnpiqbbr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2dydoagaz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2xcvtbkcb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2dhtkzhhn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ytbhtfne.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2aesayaul.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ussdssue.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2yregjswk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2rzwuvfji.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2hmdawraz.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ifvxbfku.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ucnfkvdw.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oqnvftdn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2fvglvhrg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2zyajybez.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qithziph.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ecthokxg.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2eczefvlz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2uvoiiwor.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2zbjlwpng.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2pmbaxgzd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uvnzoqhc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2nroiaxqz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2kplcbklv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gbsenyfv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kcgkxeif.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2rabgwsjn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2oxxywpxx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2patbbkun.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wcobrvlg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kbrygblo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2oknnngyy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2djvzoodh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2qorskowi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ejixtzuo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2sreelwks.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2fqqmevin.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2adtnuwmg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zgxtkuoh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2rpnsneba.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2vevkxvhj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2pfzbfdwn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fizllfrg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qlaslozl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2duupxtae.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2kzslyoqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdldytnk.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2zyihlggu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2wdyeetqu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2dhwchbew.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2mtzsqrzn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hrfypptc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2nvqexwqd.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rmmyydzu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2rtzzdcms.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wxxwgksq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2omqvumoq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ghxvbjyz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2pqdccfak.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nvnatrev.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2yzkkwbgf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2khldoutg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2bufkakks.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2nvfvbwrz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2pcrbvgvh.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2mbwioyez.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2zrbtdbta.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nrjylplc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ngestodj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2eckugzmp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2piecacdu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qzbuqesw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2spbxcour.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2miacnjwq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2xxcvouep.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2gxgkulol.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ionrxtgu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2scnlimth.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2nxsnvbpu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2zgklwflr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2mgsokofx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2axtzvref.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2caadrxoa.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2phrhhmyf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2iotqcpwg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2dgexndmx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2akegluoj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hnwxtict.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2uffrwlhx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2mvuirzym.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2gipevqxh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ispzavfo.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2mprbdoei.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zppfmlth.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2aumyvzdq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jkdfqyss.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rezpnigy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lyqmbtzn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2rlncxrqf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2vqlzekbh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2bfkhhdbx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rfxpapxe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2znfrcsab.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2torbyqcy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jdhesxsg.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2njyymzmu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2srkwxolb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hbsamxoc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2afmghycw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ogbhhxip.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2nonltdjz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dbccesfq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qlwnqfpa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mpukifha.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2buctduff.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2xeoucvir.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2zvoxpboh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2npeikwvh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ekbhnjeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbqmrmpo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2yxdwxhjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yumekmwa.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ahvupfdg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2obcqratw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2foxooywb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cyqmyrsd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xuibbqel.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ruamrybx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bzwtijdz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2pdxlnkqz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xagpbfqz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dhigpxux.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2eawoaxxs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lcnuiyif.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2pjrebwdf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2iikmmyzz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uzehhvlh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vmopwbkx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jtzzjhip.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pblqfcmy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2veecvaqn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2jfqoacxr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2tuhhxtxw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2deesaccn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kwydiwff.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ykwlszjr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2buclkkmq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2dtnvules.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2lmxurvqs.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2yxoirltb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ilypfqvh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2smhuypnf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wjtpefmk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2clppgdvf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2jnbtsdqh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2hckfptgr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ioxeswux.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2oqraxmze.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2xadzgylh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ysiqdssp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2knhgdexp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uczkthys.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jvzqnrfz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hsptwijo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yqxfkcgz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2uhkyyreq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tzbpdixc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2pmaprdvp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rgpazwua.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gqoemthi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lxwvwoxg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lqxahima.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2jwfbhibm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wrkgykxu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ammdtxxu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2xfmdeafo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2spvrvwfb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ivuazfqs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2jaidhgtc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2indmfhmf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ehoubqsg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tbgfwpyi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2uxpdvjud.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2plsykssl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cfgkwawg.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2hxkznycu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2uxwtkbwo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2hmnfkskj.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wfxxydtv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qgqcuyhs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2gqreojgx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2wsnfrsje.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2crqnoasw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2rckicywc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bivhtihy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2hvztwgbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exwlllge.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2owkbyyhl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gpseefug.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2liccsxpb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dbqnyjnb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fqiecujf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2apvtxksi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tdnhthhx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rnsofzaz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rwdohqxi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2zmrraczp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2readsmld.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2okrnabju.html


<!-- 参考信息 -->