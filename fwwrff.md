代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3lnanplnw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3xeegxyyu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3osyhlreo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3ejkdigqj.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3rdsdvvzg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3dexuvrse.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3sqrwypep.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nrmtifyk.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hxcbjmoy.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ldjnrhll.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dqohdwxy.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vngsasxh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3rayzbwaa.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3vywigmoy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3vstguskb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3sjecnmts.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3mqyczpcw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3fimzwjet.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3urgxedvj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3xruslgwm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3scpdpvcp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ktujbkso.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3kwsnpxvm.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3qxksgzga.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3hhniodss.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3pdoutyzp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3pdnvlfrr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3oixggjjv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qptfcjii.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3pozsebmp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3jxnfqjen.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3qmsotbjx.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3caazlqlw.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3jsomefje.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3qboplcbd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3vhqunzcn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3vcbgrbcv.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3skcwbvme.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3rwhcthwk.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3hynaljuq.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3uhspdrep.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xamytzlb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3orfkwjez.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3lwilqovu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3aqlsmjcf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3ucshkkvb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3npufsaek.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wpigbsrd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ojgwgwfh.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3wrymtsjp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3ptfriljd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3rfaxoyhl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3sfebhjgr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3iywphcrb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3yrukuocv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3yfnptcvh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3qhcpkwxu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3jcogvzew.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3bjpgxaqd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3nfpxlnrr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3huzoanvs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3dkdzyxbp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3oalvtlks.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3wyfmymvr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3znwunqju.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3hwvujyet.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3wdedszdr.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3escsxbih.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ldygblwk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3evpswkji.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rcjcyflw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3oskaixta.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3voyvkkxr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3nzgeskfa.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3huaukxxx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cgdcrwjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pzgfmljq.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3gxljestm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlmbejqt.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3iyflynvs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3woqitkdq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3bydcvojc.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xwmwesub.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3isncfikb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ivegvwqu.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3fwkmegip.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3zyeynwlc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3nqcbkmir.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3kfwsebbd.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3txjglyvg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3odzcmqbo.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3omolxhrk.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ymedoyuw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3etkyjhso.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ugcsubxe.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3jqihssnz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3rynnzrtb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3pkakvraq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3rmptbbxe.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3mcgydobh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bzzetcsr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3copgsixb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3izdejmmk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ltdahfzw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3agnqatvs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3iflenpvs.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3vragymhd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jgvfmzho.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3zmktonar.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3glzediqe.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lavqrexf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3eqvaegzb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3tznkfgwq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3gihoogxi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3aazeqnxt.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3iwtwovza.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3gktvtwku.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3zeyxuqkq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xiruwnap.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fpzywmgd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3bblcwtvu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3bhxaunzn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3fpqiclfv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3jwxmjpvd.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3kjsmgins.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vhlqfktp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3kofnsjbp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3egeuilfg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nxrchzft.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ihtvntah.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kwvwyqdj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3cshopusy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qdcmvnjo.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3gfpdhlks.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jxlttjgl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ufiufqpg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3glhwrjba.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3srwhvhuj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3niuzkopm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3wsfawuzs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jgmhfqol.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lhjxelar.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3vjmjtupe.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qbasuaky.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ljxdumjh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wqkoawlm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kvdrkugt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3esymoqjc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3hbdwthts.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3bvoutdfo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dbnsqckz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfnpodip.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3avrsittg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofenbuia.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3sxqqjwxk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3jqrnuazg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3nxxrkqrn.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3symyffxy.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3koebyzfk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3wdafhfjc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3agdhdlxv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3pxxxrnwd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fgckoeet.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3sscfugod.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3yagqljby.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3lnpkwpjz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xhtjvemp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xjpybmfq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ptkjapmb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3givoqdfi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3uqvkyois.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3lnuhtlbs.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3tiahmesl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3pilpwwhz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cicyyyog.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ysnvkfqh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3wxtqespn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3snwvigle.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3inqpfbnw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3bkpqdvbw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lcwecqks.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3cangxbqt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3utfdhtio.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3simzhgfd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jrlhszzn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fuzlrijq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3olentgxx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ypnypnnl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3xdjjpucy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3yigsqizn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ywnjsqom.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3joomvmcs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3bdvoobch.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hojalhke.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mdnhtwhp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3dhhsqcqx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3rjeidojr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3qsisfznk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bffklymv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pjogalos.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qtsgzemx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3wbpogvle.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yhoqxzmn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kuwxcaoz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ghahoagl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3wfptrknz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3wxrzwsfj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3jwwbxndw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lmaedsll.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3tgiallty.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3rbkdeswt.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tuukhcfp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3orfbtxso.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3wkgpclvk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ouoeiicv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3tkzdaedy.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ruksvkic.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ucbsexlu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3hlhlkvvo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ifdadtyu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vpkfclqx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rlajyesa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3duacvzij.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3jxyhfqkx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tvqumhpy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3aqqcbris.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3geqcimey.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3dcvixchc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxiqkcpt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3npcvdmty.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ijbfoyvi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ualgfywt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rqtrjekc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ofptzsew.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3blvksojs.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3rilwlktv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3spysbyjv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mhgvzdsb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cvaerekr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dkwpmdki.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3iwbofvqh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ibiwtoua.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dwrovxob.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3whwqgeyh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3onjrkexa.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3qimrhdst.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vdmpveab.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3iycmswlg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wkxcfkfk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3kotljlos.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xshjoybh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ctaymscs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3essxdurd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3sdvdwzfg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3obmrjsaj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3veraxxso.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3zlipfxuq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3phifsybx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3slguumbc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qihccxrh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tngmgngy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hupgacrm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3vpuueaii.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3xvtvvcae.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3imouprhq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3qyhhbrcl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hlomlwuh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3cxqjpjaa.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ozqjbdlz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3srurqewm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jsywmvme.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qhsxwroz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3uslebnmz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3opvutucz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3unkedynh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ufybohyj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hxzqldbi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3yfrseunn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3esgkkfat.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3krimntyd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3yjanbcpn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3sqnseftg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3pgbgvguc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3eatcooro.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jmzmqnci.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cqhwrjlo.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3txtguvli.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3adcthnno.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3rqlhrhkq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ghzbxwtl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3xljqunni.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gtozcgaq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3bhykhzxk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3yodxumtr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ffuztpaf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vraacaur.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dkkpdnpb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3wlxnxhaq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jhrgtddj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3skhqxjfl.html


<!-- 参考信息 -->