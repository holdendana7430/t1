代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3jgdqtpxw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3biptayhz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fcgrzbnl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xyuammxh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3ffwbcjfe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3ujyvqfwh.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3vxnhfkzy.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3kziwfxgh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3bhulwpka.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3gxrzmkqa.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3foxdonbd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3zgysblbt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yealfgta.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3vgjgxobl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3kcicxpmr.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3pqcbdjyz.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3xlulhvmd.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3fgwsguos.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3mpxlkivf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3skrnbjel.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3qbieyrlg.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3ifncoxyo.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3kceuyabd.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3bywyqiln.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ghfyngld.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ixnwoobx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3lsdtvuji.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3zmxwatvb.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ddvcrujw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3lirhnekr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3uotgzqqw.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3kljwalia.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3wacsqzbz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3akfinwqw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3scpougfm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3byzobwvl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3ywpxprgb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3wghmsrpa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3rwdnfzgq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3rtwoiepm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3vyteoarf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3ehpcmwgl.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3qnacujuu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3meumbjzq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3mabjvrkf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3tbvtphvo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3sanvpzjg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3pifxoudz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3fclhctve.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ygbkqsej.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3etowimeo.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3ttskdvbr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3cjrcrqfv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3slmsldwg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3tksokiko.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3seovovej.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jedejjnd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3qixisbgx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3zlltyozl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pbvbhmdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjrgsrbi.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3czbgadhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgscqord.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3weeggkth.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3mdjpgrmt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3rkxjykoh.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iskcprbp.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3skqopsev.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3sqwzzfhs.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3zfleafti.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3iayxrvdv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3pkjuppwr.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ehrgidpv.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rpmxauiw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3oqflbnsv.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3jtnktdom.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3pqwytfck.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pnitfxdb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3lthslayz.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3anzacfmb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xkywrwus.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3iporxnpx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qilnzbpq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3tjanwpqd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3jepgytkq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3xkxtlntg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3isvgamwq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3xjpfuebt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3gqclnrze.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ftfvuyly.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3puwxtsgr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jkntrebk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3gsflgsqx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ayojlpxo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3mkmalzhu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3cjdljsfb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3kbmvejrm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xumxfyjo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3cnblbktq.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3fvxezosh.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ylceqbui.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3gzzxngdc.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3znzvgbua.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3nrmrfznj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ncxnjvjt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3ybfchkpx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3iibotdip.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3uzivelds.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3garglkda.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3usqnelth.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3frydymih.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cernnnah.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ibvgdget.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3uriwkulw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3oimgjwux.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nedspgyv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zezleccu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3mpbadomf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3afuggwdn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3wbavibku.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ymulbgkj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3isjlonkv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rwlatngk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ljprigls.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3glbvnoak.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pqwcxwjh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3pcymjixn.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3hvwhxley.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rutezdru.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3sfheunas.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3wnqfgifi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3tzeiydtk.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3itcoghth.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3htrewnul.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3enbnprsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ipzqjxxt.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3jiooqnow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxnwatut.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3rrchairv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3xlmgmbux.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3voiohfqh.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3gdctrssm.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rndsrqrw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3lecnvrhx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3bckdgkzf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3hxasvwyv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3tlwvciny.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dycdqktp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3brkswazy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3tmbjtrkl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3bfzujfdc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rqezvkuf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3gtrvbphb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3uydxeyab.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ylzxhzmk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3zakozaxe.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3flrnczgs.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3focwatbz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3wtqexain.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3vkqpktxb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3drdigoei.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3jnwndmxh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3tthanoog.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3dosubvbx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bsunuane.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ogapqlsm.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3gdjpqsyj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ghlxcgpq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3kyheqqlu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vsqoqtrq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gsaxbhsx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3rtqasphy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tgtxyvxq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qyrgljxv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ixplhopa.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3sqgujijh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3vsolyple.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vyfegegw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wswjjeyt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3dribfphb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3cdrggfsz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3kznqefgt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3htvildlr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bqdwvczh.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dxpccidr.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3byrqlxkd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sdxltufn.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ejbnckro.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3nqdaalqk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3yhnmsxpu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3iewgxygr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3drywercp.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jxhchinw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3etyhfcmj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3nktvacgg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3uctyqzzj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pjxozmve.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3xsakfnxh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tjytegys.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vcmstpbr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ezucozew.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3vwwxarvg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3muytxwcg.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3sryblkkd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kzusmguq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sjddvjff.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3pkuzvlrf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wiqbgoer.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rakkuxto.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3meqvaxbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvajrwvn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3hbpoknpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dqzrpxxx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3snohzbtt.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fqlthauv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3mymbgddn.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hdygerik.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dwqoagon.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ddyqbnim.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gjovgeyq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3octmpivp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pifmqqqb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tyzzdjey.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gpmkyqyg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3elpuouey.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ujszjcfc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cxxyisxc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kwdqrdcw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lyvzrdnv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3bviscltf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gazsmixx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ynzqovuh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zeelihdk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3legshkgt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3entcmmzl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qljqvtab.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3olyqjzuy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3drvmhvkn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3pfnigtbx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3hvkeiito.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3pyhwcypa.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vezbovwq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3qmgvaree.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3afrkhzsq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zuhydfgu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3rgwmyuzj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3kqakqmwa.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3jspqcyfj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3fjdgrvon.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ijvryisb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sqgnlxvc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3csqkborz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lgfolrjq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rkqmjnvm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3thrxhfoi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xeurgneo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3kwlwmhwi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3gtxcjfzm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3kuziwvkq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3pdozgula.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ukeontlc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mfjwmxyb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3anzdaiml.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3czdlzumk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3hcoiwhfk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3tgfjpsxa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ucljlwfl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3rmzpjvdd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3tvdjweeb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3girwulah.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3cqbffxfa.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3uwntswwy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3jahvatax.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jtvrgdox.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3cbcrnlkd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dvsdlkuo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3teqhykid.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3bfqemdod.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3mvzgbtry.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jbsrgcys.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jlubjilm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wdewsaei.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3cbhwwozt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3xrzbxzdx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3yybhvgph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cyzbokij.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3eqbvskqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrefrkiz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3aeovzzwx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ahebzjcd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3paxthewk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fvpqkbgh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3excutbgl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jcrltaum.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gjmkzlkg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3vzcqbjxj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ntcnyqpb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3fwpbmysd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ywgbulxn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gdyhjska.html


<!-- 参考信息 -->