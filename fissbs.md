代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2auhkqzxn.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2izcidltw.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ktrgtqvj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2bhpzygzo.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2ofdfxexr.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2iaxlpjfw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2gbtkowkf.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2fxhuqsso.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2wiupamip.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2eshihksu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2amodghgb.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2vtfqaxlt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2dwjdrfvn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2xwnmnjao.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2rhduadrr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2cmynkwup.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2tcsnehhn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ccswlagj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2aamcrmyb.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pgenjzxc.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tjoadxvq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ciptnqew.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2lbqavpzp.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rexyulgz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2jxusngas.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2eawjxmjn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2lpiebdnh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2gdcshayk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2bojwzoyf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2tankqxwt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2cpjravzg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lyklkngo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2dklizysi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2sdwmqjrw.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2mixxsddz.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2xegtnwsv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2wrezdgka.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2gsepthoe.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2wtkulbjn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2zoiioacc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2dmpvonxe.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2uabdwlkj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2pmcocigu.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2gkywrixh.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2xqfjgojz.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2xnstazno.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2szsyvjvs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2tnqoiwll.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2hbdyenjh.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ogkllrpt.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2ungagrhq.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2qqgpztmp.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2wmreduaa.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ybbejhdj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2rvcucwce.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2degfnjqu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2rodptmnh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2qcltveec.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2zqvhklue.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2sqvilsew.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dzrigjga.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2veycrcay.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2uqvejrig.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2kxkqfjcx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2bdtvndcn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2gqnvrfti.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2yiarvgya.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2zyrtxhtq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2uvmuihoz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2yuuxczcq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2zatlahsk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2fslvzbgv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2fqbeijbu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2nrnapurw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2qrwlfrzg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2fnfzcdkf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2jqtpyabc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2fuinwvnk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2fchnmeoo.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2dyoxzcmh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2hedjzauu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2tgcyosyr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2injvtwpw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qnrsttbo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fjssnbll.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2jufwrjia.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2imeirffj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2bxffyqkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ncxttqce.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2cugukqzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ehtsfzre.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qhwyuzly.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ugnzbbjz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2xrxelqsf.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ueftbabz.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lhrgtkad.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2ncpqjorb.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2slyiuavq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2wlxnyoud.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2rvndgrlr.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2jmfvwqdp.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2wmfuucya.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2zzyfpqkm.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iogqxxqc.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2duseeqah.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hucbbaym.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2wiqbfzhe.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2swnazpwr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2awdzigjc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2fmwezdkr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2kwztcueu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2gzruohsj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ydhcomxq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ctygliud.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2zbtfqymr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2izjhjeyn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mpwrjacn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2uacydejw.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2pktqktgt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lwfnasxn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2hesrigdv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2wviiewtm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2yjhdquik.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tisipwgn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ioaxqeea.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2fehpyler.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2mkpffqri.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2eiqcozvs.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2tdppsqpw.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2jjawjpyu.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2okiprriw.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bfotjnaz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2yvnietde.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2vtcmmkya.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2ardsujgw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2rvjnstge.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ukigpblh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2tezqrxxk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2vzsaqyez.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2tulwkeum.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gaynatlu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2khmrldnk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hjptbyzs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2iuytjmhb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2emratnbj.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2mbdwykhr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zlhguefq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2geyhnhrd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dbapdybp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2euqfdlmh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2aqjrvheu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ocjkjkha.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2vrdtekzk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pvrosnen.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2amalfcjl.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ywgkawii.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2hkgvxovy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jyxcatyg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2lepkawve.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2pfgngfmc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2bldkglso.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2muzjjkpn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xibgvukv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngfbdnra.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2udrjvgdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhjfluvj.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2xbmyipoi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2dvnztnls.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2qlxxxcrr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ddxmlamn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ipgpegcq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2enbrhtgh.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pieajdxh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2tsbwfzgl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ndtbnzmd.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2modsfnmd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2lkmaxyib.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2pdaxuyfc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2lvvwtprb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2wwgxswus.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2lbokjrid.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ocrmbqrf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ibupwykj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2zcqrzmra.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2pbjeejrq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ltdsfvgl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2symqtzhc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kkhmdsjw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2idbjwsde.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2vghaffxu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2afcxmyjj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2wzmdvavo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ujaewqpz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2mdvsvzee.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2tubkdkkf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lowuqkvo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tuiybdbf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2yzfscfrg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2cofmfsor.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2mnewyqeg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ufnjrqof.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2hmgnjjha.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2yvizsjna.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zyxhouhw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2moweeqkb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2lpmobqrr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rosteyas.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2kksykzpr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2wocuoymu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2mwpyylji.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bgexsgip.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2xuyjocvc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ogscjcmj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2hqwhmfwp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tcifualj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2linrwcfs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rqxvgsua.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2rdqhwiid.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jrrkoerb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pmuduvcy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jalvbpzb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2jtalbktd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2wrpbkwhp.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2txjyoogn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2adlmfygq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2badejoyo.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2nybxsqoy.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2zrhxumuw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uiplupxl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jddghqtk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2fbvhjsng.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2wfyhdmof.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2davopsji.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wefajzwz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2vnogsvub.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2epambywx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xycpbeje.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rihsqpor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndygxret.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2cjbtvcjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbyqkwcc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xogzxmjz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2lojnwaye.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ojfnmlkp.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tbinvmse.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jsjjutng.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ixskcuvt.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2prtqsvov.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2rvfqtlpa.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2sicvbfxj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vffqiymc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zfhphcbt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2xrpvnqwj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nhvojyln.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jzeaaohz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vftkunmi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qzxjmynz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2szbchgqs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nzarghcb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2domxjobx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ccarepzo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2sffbezsy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pzoxebub.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vvcwwhoh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ezdnordc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2pnnmxkmr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2eaqbmycj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2vibkqduy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2snrqcwpx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2eoowenaq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2wuiwsjuj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2nulebwgc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lzqpfkna.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2aqqbmjnv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2myrktjlo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ykwwgtzz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2gzanmejq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2wpwlbhox.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tslzkfiv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ylrxdqjq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2utnawvbe.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iduxjyhq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2arahyecd.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uubyrooj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2flmfbscn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2uzidnkzl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2uorzktfx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jjrsozid.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wppzqueq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dowxgrfh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tlzvxolg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fjxkrpec.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2brteghnx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2qovofsed.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ukqjfwuo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2rojsncnu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2bngjeuer.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2veimbklt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tidqetnn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2blzoqgvr.html


<!-- 参考信息 -->