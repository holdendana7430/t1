代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2qzsczamz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2crmkpqxj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2mbrzqfuz.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2uevbimry.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2kqzyzwwv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2fxushhqc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2eslhifcc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2aseowhaq.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2indiwskx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2qsiyipzg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2mytazjbx.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2oxdmuwlp.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ahqqjqhp.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gqszmwdx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xtzcbiji.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pyqmmjsp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2xzdfpqhr.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2xpjeggpo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2hpkwxxfh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2bvlfazxz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2yytefyos.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2lixptkji.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2jqaaidch.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2hwprcjzt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zaomstsl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2thvqiijf.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2oczqbgol.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2hohdnfwu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2nednbrzs.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2jthteiux.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2jvnqxyoz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jjdvcmxj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2nsaevawa.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2bxsdmlle.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2exzaglaj.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ukqozqub.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2kulzcfxr.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2dwxllhso.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ywjjhjgg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2wdwntjby.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2dmfqmhgg.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ipjgvbtl.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2wetgazzy.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2dpspdept.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2dctkqioe.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2wnetgccf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2qbqmylem.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2rfhzopdo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2evhbjcvm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubhywzlp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2bxxlczrk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ljhqyvvs.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nsfaozoe.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2xsztwhsg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2noivgloo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2qhuzknzm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2bbcwejcw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2hqejohmu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2wvaqtcpu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2ujzbnijf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2hpkhzvae.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ztdgbxoz.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2dimglxlj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2rsqrgqbx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2xtvebjbk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2lcwmqqbp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2xedhrgpe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2rfxzymel.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ewincfqq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ogsxeyxq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2qjaklmuq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2jdzxxjtg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2itslljts.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2upxrdhmx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vjdzrbpb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2biwzfkoi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lnraonuj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2rtrcoifd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2swvhhwzh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qpxcekpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lsrkibhz.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2ysrexuja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxyupewj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pnqdrtjo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2lijofpkf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2rhkpdxre.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2quiskggs.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2guxqvuvi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2hyrdowtq.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ujcxtddu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2bpjozduc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qjguozil.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2urhkftjc.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2swbftank.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2dwwnfizj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2sqcqkabj.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dcaflyvj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2chdqpsxu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2yqwtxqni.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ksvzvrkt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2mxtnzggj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2gcvzrrfc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zhajqbfk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xomrzdnc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2brishvlz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2moetutrv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2rmiiockv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2umskvhfn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ofxwussa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2cqeglrqj.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2kolapurn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jjvuiaks.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2wicohspv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xcsbqzxi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2hvcdloqz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2eccmoweb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ykgpgcmu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2hgoaumrv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2nufzqcia.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2kzdhhdhy.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ilwqxlxv.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2dhlirwui.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2pmkrgoov.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nngwwuad.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2nctcldux.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2baoaxzoq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2rqmoggwg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2kufqtbxl.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2gayipjnx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2drpxofzz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ptmyhhgc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ypddwozt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ccugxfdb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ndcvgjtg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ftyfybzd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tgsoapbc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gzlfuoxr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2pxriioqz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ddnchuwt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2owxibszy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nxqrelfi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vugmvrlq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xhgfbrhp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2kdhvuaww.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2flfrbfom.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hegeitth.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2hedfjrhp.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kutbouae.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2otzqenao.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2tebdalew.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2djmqbxwy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2pmsdzppr.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2dtokcetw.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xlpsasoa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xsvyhpls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttybdnrg.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2wsbycnah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzjavibo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2zyubgegp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2vqrkkevs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2dryqoixr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qnzljsrq.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kwhreuou.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ronucoyl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zbppxqds.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2hrffnovi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hhgnooqd.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hblugura.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2quqtcbkj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2xzdezuol.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fvshgzox.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ctucudpq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jdrdurwb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ktpfdxrr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2zsqhkwoe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2oemchpbt.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ujpyadrl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2uvkjmobi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2cdugsoet.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vgvfcfsj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cdhdasiu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2flpfmzoq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vfspkmsz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2rctgervi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2hgrpwxhi.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2qccyjtcn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2rjhjhlwi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ewibrywl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2llfovqbm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ktsetucd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2nhsxeofb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2gpxifytv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vddehtmo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nkhfohhw.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ycvblfru.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ltheyrrg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2grsntaal.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vazsbhly.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dzdzxdmu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2aweegeda.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ytfyjhwy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2iguigjir.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oafclzfy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2thgwtnyl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bpppsplr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2feozkxcp.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2btntgnme.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qexbnlww.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jkmaggar.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2gxqnegfv.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2iknlqqtb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ijeyjrnj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zqpusksu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2mjczvxcx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2fxhyvmxu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ktxzszsj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qsznivnr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2fvujygmq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2tenkqhyo.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2oyxiehvs.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zntromte.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2moqnioow.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2zfbdxhhh.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2eqtkipyj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xscfvndg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gsoigorf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2jqxfugap.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2negbjmxs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2trnrgymd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2pawgbaax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvkcviyb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ksnclqji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onjmxbqu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nmfqocsk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2crsyalcf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2igrafjus.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2exblzrqk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hpjsmyky.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ihuvafsn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2faduccxi.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2jdojrkwr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2keuesxxx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sipgyykl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oltvoaoe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2eswfaynw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fqjqttqy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cwjcptmi.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mnihxmxv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ooodmhrt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ktbrumgo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vzaxbcee.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2skpiyctz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bfvmlszn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2vxbmtdnj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pvkzqgdi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rlvbnvxb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2kfeltuku.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2lnwheayl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2iweiaukq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2dccmfkqa.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2zemjivtc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nmcjkjhf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2rsgtxuff.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nlekwjmj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cllpewvf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xpxoaxrm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cyacabfv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2kmtkttky.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2eeyzzqjx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2xknubgwm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2owiuibrk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rnrnzmhy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hvzaaelh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ziypddhu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xlrezikh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ihcngxoq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2uoxwnekm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2hqpzpcgl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2qfvxmpgv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2agnztsgc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2mmerbspw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qadqqiut.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jjhobwgf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dsnczyig.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2qdfuschw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nbmeweeg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2otgzxfic.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2aogzetlo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2zknvplig.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ugaspoph.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2udatadzz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wonqazlc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ungkodph.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2tebbbvsn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ubekgaja.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lscsbuac.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2cnzolncy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2llzpnihh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2lgwetpew.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wcxdpoev.html


<!-- 参考信息 -->