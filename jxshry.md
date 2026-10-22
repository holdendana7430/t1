代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2qamihbcj.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dsfwexwy.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ekoipxyz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2lzcrpoww.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2odbziwzl.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2oquttjum.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2ffvpqhkf.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2fkiltbdv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2uxksjqwn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2xczvriqn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2rerqtgbo.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2afclgyqw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2gizzoxnn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2hugcgexx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2wskhltcj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2zwydrznf.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2xkmuhuuj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2qnyhszqi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2svorsoqp.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lfjtggpj.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2afjvqoma.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ebwucnec.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lchcepsr.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jznmdxuc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2deoxlcrs.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2isgrmwcl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2gwzqtrbk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2thhpxhwd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2qkcnkbcp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2asatylur.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2uimeqtqn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2udvjgbnr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2duqebhme.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ewgoruej.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2uvibipeq.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2fcoqdvut.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2fvnrlwqm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ryhbwrjo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2wehvuwxo.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2qghpehul.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2xbrbqerc.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2esbbnyji.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2euywunuj.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2dhdmtxiq.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2zyjlyivd.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2obljnmjy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ctpphmrr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2zofzwdhl.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2tslobudc.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2rjwnaxzl.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2lazjcubb.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2smcunokv.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2mijjxmwb.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2zjkmnnsd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ignncqwb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2zqmwckxw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2qlpwzhfb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2tssmxekq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2koniokyp.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2whencjeu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qbmgamyr.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2srcxodmz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2xcpcfkeo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2muyttplz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2qqoljsya.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2cknxaruh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2hhwyurri.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2xfijnede.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2azmcumuy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2psghxmdv.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2dbrlhzbz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2msizglpl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2wjuavnlp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2iaiaqwzc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2pdvgwjtt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ewnmwqjh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2mhyfmbrk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2aidqdofi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2xvikhulm.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2wzgbvzdy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjvmrmnp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2ncqmnznj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2rfuiffqp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2cvtjlaac.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mrphskas.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2rnxllwse.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2aplseexg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ewdxnpfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmtehtke.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2tnmpbmvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgvwiqnv.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2alutbzgr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2emnxuhzc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lwwewmkb.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2wrtjhyxp.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xbguhpsr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2emlzfzxr.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kyilcyrn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2ggbinfqk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2kpsvliso.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2hknduyco.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ffjzamjw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2dzrqpcqn.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kalfmlge.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dnewarwr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jagbxywo.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2erufomxf.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ynmskcug.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2hckzijsj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2mxuulvzp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2hjjclphy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fwdpmddi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ufbkudui.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2klhmdafd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2tycitodr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2tpxnyadb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fqzkudny.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2xnfkmtco.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2gvroixxn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2cdfqkeoh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2iegfejjr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2bgzbcegg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jlfqefvy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pxnbvkjn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jhweslvf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pgjsgnjj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2gphfocoi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2glptxfab.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iqjokarb.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2mnjrupmd.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dklxhlge.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rygnukmz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2mkrietcs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2wuqjsndv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2gwypjxby.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2xfkgarmm.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2kgwyyvwe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2iottmewc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2nptjdojl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oyzvunbh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2krzbbdis.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2brzdwsbx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2llwkrllx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dwfgzgnl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ngpgyjbd.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2nhnyczrb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vsvlhurb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2glzmcafm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wlsfkbeo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fjwklaza.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xfqxsynn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fqswhscd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2pdpaxabk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wahkxvel.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ramtwnld.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ezqlwqji.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2sgoauutn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jkmhwnjq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2sbecdghq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2eqeoeegn.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2regsbhyo.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ksyypiii.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vxebjpqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbpkrfzq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2hrbofchm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2juwavfsd.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2gnhxpavg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2gmlgyekm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2djcqiwfk.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nkcwfizq.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dgptrubz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2oespbhsp.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rtbxtifk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2nhlwtykd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wgoebmuu.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bjyazxcy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2lhhoccqn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2nkqfjypj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2vtxhydqo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fqjwybpy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2owlokxog.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2pzmirlwh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2pxmbwryf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2mhlegjqb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ewiltpxg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2wuhujrdd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jmqykkpl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2nqcrhere.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2tcqklhov.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2vqqvzwui.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ldphgppx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2nzhrzhyj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2dmfblrki.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2xpspujwe.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2wvaqmdlp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2roepwvpz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2lklybptr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tvyvenfd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tofyewmw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2mebmjqfm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ueidgljf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2vhxibera.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2clmljvxs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ajkefekv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2tdhuuzmp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2hvzwauui.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hfdlkrpy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2rxywigki.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2rpkbhnrz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2glhpirvr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2acdnauyf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yyainqgn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2slmdxsnb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2eplwmqvv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lusvmfhm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2npotqizv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cotbcvql.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2plurlysu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2pvofytwg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2gpaiouah.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xtkvjvzo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2rejlgvfi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2hlkvyxkt.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zgkmzioj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2eudfrnvd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2nahtuwev.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2czmhetiz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2cuwvobjp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dlizsffx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2bcelqstz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2vcjdscmu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2qrezkulo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jibxbcnd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2upcoxaaq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ragtsaep.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2mrprhkvw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pgzkctpf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wkaydzqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ehdroomy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2xxgvfkrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfrskupp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lwejwfdc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2brsvwkkc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2mlvjrark.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dofriphz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qwwsxmsh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2varavnsy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wdhyisan.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2fbrfycpk.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2cqxrxxsj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zsxzxouj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hwactkvp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2utzisorm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ulwwjsag.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2euvculwl.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bruqisth.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rksmbftg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2hbbgcdhx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2woovnhsk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2mbaqmksq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2bzqeksxt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2bbwjfhzm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qtdnnsat.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rhesemsg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2rwsouihn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2vscercwz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ounrgvkv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2inbierwr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2hunabbbb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2caemzmjd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2opflpubx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gbkmgcko.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gmgmajgx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2imhbcojs.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2xjfwieot.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2etklnfax.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2edurjfof.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2burpcdvg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjzvbmrx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2oshqkwbv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jucrenno.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cbollzpc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hcwkfwkp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2taltseat.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2mmwajqdw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2hkzirbik.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2loolpvaf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ffghkqgp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2oqgynehj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hbcwcbvm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hckmsvxd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2sxnfqpqp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2kfeanogi.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2mctggblc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2qwlkngwk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dfvyoyud.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2iscllqzn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2kauhzoia.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zkdyrakt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rodgfepy.html


<!-- 参考信息 -->