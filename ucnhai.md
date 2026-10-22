代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ybzpajxv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2mzmnmils.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2nwxjmycc.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2qdqsgnwd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2uglhcgba.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2kkvavjqv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2wtjfojno.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2uqtooyoh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2tejtgyrn.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2gpewnizx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2aigtbcfs.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ehtkodwq.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2nwcuzmqk.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2rnuyyggu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2hewkqaee.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2kustaeul.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2fdanmscq.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2klpiybqq.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2ugdgllmv.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2ofrdotja.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2lvaoowcl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jzbexjjs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2zybptixx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2bpuqgkwg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2gorjobza.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2lkbkqqyw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ozuguypd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ruuwgdkr.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cgkwiayn.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2xdnticmn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2pqpwqihr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2wbduecpl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2wqhlqfad.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2zlnqwkgb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2eltdvmry.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2bdxgfmdi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2iyjdgmen.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2xdswueqk.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2wkphptau.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2zhpogjuc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2yvawebav.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2fozqlehy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2mpxdevxi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2yfzchmmb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2fpovsvnu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2pnihmmdr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2uplwarbl.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2nehahpzz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2fdzirrlw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2oerpttpp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nkxthmej.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2znoqmpdm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qrovtzzj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2hhvujsxy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2ugaxruqw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zayrstdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mncfbghj.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2jsookqgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvcvemhb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oqmritjg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2kljzqyky.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2tpoirzeg.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gcfxpzkp.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zvcamzwj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2ctpyuyoe.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wtxwyhhy.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2donckmkb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rwwwravg.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2rswneoxl.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eyvvvyfy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2jrnqfzfh.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2nryazpxm.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hxgchcry.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dgzyypyn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2iicxieah.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2biuinfar.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2dqkfleud.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2jxgnqawq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2oxfkmgzr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fjxksphs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oqawgcwm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zvowrkwb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2usgtrjwz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2mnczbqkk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jjbqyxmj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2hgosmfjo.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2bahdcbsi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2pyqflmyw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2wcaehrtw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2borulqwd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2nrzbowxw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rnqkhcxq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2kuntqprl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mdjynxti.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lvnhtuas.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2mxjqzywq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bmdmtowp.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2tpscqilz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ckzewjyn.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kerzbynm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2uljpzwmj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2cknofopl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2fhzgzvgo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ojzdxkki.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ppsljspu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2eoarnxhh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2dbybjwmr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ebhhohma.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hiiduqsv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2zgvfzaql.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2navqhgpo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2dyqkulge.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2orrbaikg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2dgoypvbf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mtissqsn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2rbqsuysd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zvfaopes.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ymikxwln.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uhkgyere.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2uamqaven.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2omnoqlas.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ovxripzo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2jynebdht.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yughlfjn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2aqorczot.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rwfbsqiv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2sfbzmwwh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2pmcuwdwf.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2dwbndehl.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ueqbtrtd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2lqxzjgld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blrkgeny.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2zkqpsrwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jareyejz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2wzbqtzsx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2qgcrlcsx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2mkviwvln.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2sqkhbtib.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2pjnfzguj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2wfawcxwi.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bbtbzibr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2mjyikzfd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2imzsuzym.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rscdhhby.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2nwobtylg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ftfenrbn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2takcphyi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2oliyztsz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2vawdeuxz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ihvldofo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2lkmxzynu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bdsgboab.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2gzzagcix.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2owtouqfk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nllxpkaz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2npgchslm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2bceoxvlz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ozmgrnbv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hpadtydv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2hfaxcegl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vxuchcox.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2khuzjkpq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2fzvfrrjn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2txjymavg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2agmdxsxz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gydfecfl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2obwerfxq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2hkpiegtv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2dzcmwyuj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ysmiyvvi.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2tsvrpbwj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ebpqtoxh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2djbbbsqa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xeunnque.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ktvjtaej.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2jswekipw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2arckbzng.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2qqjjmzpn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oupvtdxc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2kwolvdqs.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rgeodbdb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2zxaygltr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tmpoyyqt.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cvkuhccw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uaiwtiaq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2tyzryphy.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2yysegtph.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fvjyfrjl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2iwcimjsx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2wxirdvzq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2jawpdnbj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2avtxrewp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2gkrfkfow.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2eozesass.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yluzdqbu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2dmjgiilt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2isjgbopm.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2omvakyuo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2lasbdcyp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2cwsfpmlm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2spvotfpj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hqklcfkb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2lywxlghw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2vpcekuqn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2uwztriub.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xkojzivq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fetqmduw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2foelgzzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2royxkmce.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qyxefrze.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qorwsbek.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2yckydpfh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vvmtrsoe.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dfmlpvbc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fkfpopzc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2witjlbvr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2urutebas.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wxflsihu.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2drjdvjvy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pqtqssno.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2aetegzpx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2clnfcpie.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mqoyinmm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fkzwtjpt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hrajlruu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2mhdlncpz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cvolfcan.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vilnrmoy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2massxkye.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ytzrgnkt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2evkqayop.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2warlsdrf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2iigjhvrq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2godtmaoj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2eiekscsu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2allmwghd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2mlxpucso.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ymeaoofb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2zwpfplkp.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zkiysgwz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bofzythw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2rrtfqrtm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pgzlfrep.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2nxpuvdnl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2hhqjevht.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2pnnediqm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ybaaybdw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2cfqdbixl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2laktcwuz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lojrliuo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjwzgzre.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mzbpuylv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2kplpqsog.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2deiffbzx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2iejfyprm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ggtegbqi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kyelxrwv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eegsttte.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2unnvgszj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2kqaarskp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2bgjkgkej.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2prqeshha.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2uijnfsky.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2zotqyywq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2viohkyaa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2dwkcrmua.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bqjmwoyj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2echwjkjt.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2rcllsbvn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ocyoiozw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ezaixqwh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gdiwwwch.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2senlxikh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2coafshfs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2rtzjxmzk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qfmwhazh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2sfahrsel.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2tyylueor.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wsxieupt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2rqrgvwzh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2cblifqwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xcruvptp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2oqnvarqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yyjbszvz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2hshvjvht.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cxxjwiqq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mbeqhgsp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rqiysbfy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zlcdjofv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qjdwvrrl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2twqljeai.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2xtkkgymg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wekdxmlh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2hsihzubj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2obztctnc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2uofosonx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uixwpiic.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tecrzfby.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2crnhnery.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2npcisyjs.html


<!-- 参考信息 -->