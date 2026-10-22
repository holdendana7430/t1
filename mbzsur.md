代发 wailian999

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2lsdwefkp.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2jcifthrg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2ugruabzz.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hjgjgaie.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2qdifytns.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2rhibrddb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2iestpzxj.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2ccobwkod.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2eqjqbrnc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2fnnsyojc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ncyunczx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2pejltsay.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2lvtqfimv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2aipcfhwn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2baiuxfup.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kpfoqjzo.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kffzxvvm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kxwmunsa.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2prscddpq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wbynhjdx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2njqvoyrr.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2cvkcwwjb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2khrcxrut.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2hlfrumdh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hripajsk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2kuuswbcw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dpbfzdgv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dcgrbadb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2iufiuwzt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2puphxxpl.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2mwpiztgo.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2lgswniur.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2zgolxgjb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2urauktyy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2mjzdstyq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2crnuzjbx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2quztlbeu.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2htbyjlkj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2kgdsqapk.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2vyoqvbny.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2qkulkgox.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2aayxhxkd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ccoogjhm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2gcmtepei.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2klnxqxxu.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2malmywdo.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2aukhsgnw.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2sxrzszll.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2kabwzeiq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qowfcojs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2buszfyry.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2uzdkavwx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2honrbwbe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2vasirnvo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2usjivcmk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ackewdgt.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2yknkocnc.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ktyjawxj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2pqfqztwr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2pwgkguyp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2edcnecfn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2wslmkbui.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2mqiynagq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2lbmgbeuc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ewdkikru.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2dxttxean.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2jpmcjuwk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2fylmxbam.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2fjolglsb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2klwgmtlg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2wumhiudg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2nknafebi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2gtbiwhrb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2rjmdamdl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2lhlavfif.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2gybzycxd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2fuotofgb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2hvhbsecn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zzmjacya.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ndjqgepe.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2tannnddw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2kqzptnev.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2haqwniqw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2dmimjwvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nsohvafd.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2dquebqrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mkzzvzou.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rjvjrmfv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2rtfxyacs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jqvlurhv.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nqnxivzx.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2tahxgwjf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2ajhupxrc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2wbitcgst.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2phcwubyd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ceivvstd.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2bvpnevxc.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hfuayjdy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ghwcgoup.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xnrpvhpi.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rcijecmd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zbsnvjlk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2rlzodbgk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vfvfehpz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jtihwnri.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2lcjsgtqp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2tjsawpub.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vbupvjrc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2taxpckbd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bwifjuuq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2mzepigqy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2kpmavixo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oemdwuns.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2pjwnudkx.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2rpbdlyyj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2sxcyeeox.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2erbabnts.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hbmuhgtq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2wfmjlrgz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uvcimyea.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zbbqkllm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2pzgjhqox.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2jqwqpchl.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2kiajqaoy.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2yqxmqpag.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2yugzmgbu.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zlzmhswg.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ephqziaj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2bzlqvksv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2dtvcjbed.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2naxcaotj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2inqnuqmn.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2nvlvnhso.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2xdvxmgen.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2sjcceqna.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jswdftkx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2vauesvyj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2iljedhbb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wbvccinx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rczopfpy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2iilyhydy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2gdybavyz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pnqkcygu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2uqbkzzsm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dtlplwuh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vvrlamab.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hikefttr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2hlnszxiy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2nrkmixhn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rqgeurfp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2dgdayxkp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2zbyxkbbo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2njyeytjs.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2necfphzc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2edetzjdb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2erkkabeo.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2nfiuaxur.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ixhtixmn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jalehhgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2beoaghyq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2adwwypgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnlfxgyr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2kxyubmog.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2qpzffoqz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2oyfdswdw.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2nzbrsfrn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qqxwkbto.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2fecvlokf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2achnwdpt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2pwtsdhfb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jfwpxnvj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jldpklrn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2dhioeysl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2tcszeylm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2mzjfvejv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tmonaxwc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jxrxxqny.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ropxaajr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2jslghafu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2eidkiyiq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ijsklibc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2xkqdrciy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2imthdore.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gsqbidlx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2pgttxslr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xuseirzj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zqoaroqy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2jxyzcwxe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kvuvottf.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ucnlgznu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2bbbydthd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2akktbfhs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hxlnvnqc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rgitngma.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cxvlxyft.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2lhvydhyx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ntnohfni.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hqhbvhln.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2qpdueaou.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2rghnrpsu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2weumqzeo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2lqpbyhky.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2twtuaaul.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2yajcpadm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2tgghnpyy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2djrnvrit.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rpmikxiu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yhujbbsw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fqmynrmi.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bdcfefja.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gobnbqxl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jaepqwak.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zdmqgfvh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2zfmvgqsx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2lgkuzlvr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2akgxwpdc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2iuiejjjd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2iodgumpy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bhhwmbnd.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2bhzqrtrm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dzncojbc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2thpuieto.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qajkwsrg.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2vvkhoqji.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2gburpzap.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2zrtpcdvc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2qcioqzqx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ajpmetcb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cpnvifbs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hudurefc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2pzsiwlcy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ktfijxti.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2qmozrepb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xmjjwryk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twudsyaj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2patiwcdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjqnwwxb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2cxoqmchf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yhszkjir.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2lqqzmtpc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rbjrtndd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qqxsqdio.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2lrlgvbey.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2lxkihzak.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2tqbhtnof.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tfipseaw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pxwgyjiw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zxpywvwy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wwmdhvpo.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lcidwyjs.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2benfguyj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yamvoapr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2symofvfo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2scnxqfaj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dhdtssrw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2wtfngnag.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2imgdwjas.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gjlrwhpa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cydrxbtc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gomocfvq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2okgktxej.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2wjkpzjph.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2sntjcuxl.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2xzyjzfzc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2fzirgnqg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2skrlyhci.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2cxthbrlc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jdrixnnx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hroqcrip.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2vyktppxv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2hcukexvv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hvihpiwl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2lqgncctu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2okcxigkd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vpovktdl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2swpmwzsg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ktncpyzk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qkkpvfia.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lmjjeils.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qknyvlgp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2whfjbrur.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2oqweuxyd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2hzyeivpr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nypjdmpg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fnsablur.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qmpgbxtr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mgyypamb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2snmpgzbo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ooeqntjc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2engcdlyg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2txfqqdfh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2jbepucyp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2fpzpzjgx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nzqzjvof.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ixpnwtsk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tckwlsaj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lvdgnptt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2vslryzxt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qxtvomsz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xvsstxxy.html


<!-- 参考信息 -->