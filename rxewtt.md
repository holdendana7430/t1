代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2nelqujxz.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2gmcendir.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2quudywjo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ccgbmxjs.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2xizajzqz.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2retibtwg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2hzefdrvg.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qkvxusfk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ipnelztd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2dvvqciad.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2uuixbscz.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2bbpvtpoq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2esxrzomi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2errhjnne.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ehsyunpj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2rquqciuo.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2pxxmjenq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2pkxshgfb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ruabsvjs.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bhvcijkv.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jykeiezr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rxvwnuft.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2cnxyafbk.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bxtkdnda.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2xhyjckbl.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ownsilnm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tojdzmev.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2rzrmltue.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2jnxlphzz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2hpmkhyai.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2twshuiif.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2ekqaochh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2lpsevdjm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2krbplzjh.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2xbzlopzw.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2ujtvanvq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2apnilwao.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2zqegjpjk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2miymjatd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ctzkrzme.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hqfxbflh.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2rqtyzcpt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2fbzqfmbz.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2spxefgoz.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ihdvrttj.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2ekbyimxk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2zencreux.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2dmdjcpmq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2hmeumptk.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2djpbchbo.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2cnwtilba.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2hyyuqzem.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2vbunkkpq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hemwujpc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2vjuuegzw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2kbneuajj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2zrvnqnqr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2hgfgjikw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2yyesghmk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nscepppo.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qtrexfel.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2plrzurlr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2cwsbhdff.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2halzdmnd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2mmhwuhxg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2fjlkfpdi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2wbggiiiw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2ygvgmtxb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2zhwlgqek.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2owgnnzly.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2bpltanxe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2nqsufxvi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2ldjoffdi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2likpsqdo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2rdymkiau.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2dbgktxjm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2stoelwfi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2hbazwtoq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2qdurejws.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2zfihpkus.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2fkulxjxs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2fkporyvd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjgapfgu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mrcickyx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pphcdhqs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2cbeacjou.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2guvaxney.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2srurutkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2inchjfoo.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2gzzzrnef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2duacnpir.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hjnfkdgl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2bvzkjjap.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jtiazhvg.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kcpuquio.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rkzhzppe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2irdijfmj.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ridphfof.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2hjfdfwrr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qqvuqkij.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2isuewusw.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2izahpfeg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2vilrzouj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zgkuyrxt.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2azwhmdgl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2dvyfymuw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ywgdbjuf.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bwqlhnsg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2korpksai.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2rnxspomc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2intdqflu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ubzshymk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hltluswo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fzknyqeg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nacyxvly.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2hriykrhf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wzcjxsle.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2fjduihmm.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2vpwywsln.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2vuowcoyb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2bdsfchtp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2efbpobsy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2xzvolcjr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2saritjih.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ogbjvtsv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2yanihfxd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ddpxusib.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2disonswn.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ojhhqzcq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2pytmdfil.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rajuqtke.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sukafbvr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2cnclybvo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2tuyprurs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2cebgcmcp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2caeblytp.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2njczmgag.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mciyuipg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2btwreekl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ejxitanm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rdgoubea.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2yvobnznq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qihsyxxg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tjvwxrwy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zemspmnx.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2meeyxqwf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bajmfbdb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2nhdjyyuh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rdvgtbvp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vmvqbjnj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ushqmbmi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2eigwnagb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jpddolgy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2afzvkyyc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ptzmqntj.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ofphvpgn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2qafmjsvm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gpgaoxdc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2uaqcdhbs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qrnlwdkm.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2gkuhrtvr.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2qfcfywfd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2pdpridlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jolpmgej.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2klpepyta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdgtyihp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2towmozcj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2touvlyhs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2mvilaugo.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2krakyotw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wmownutu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2tsuxdqth.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2dybdwoxp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2tbbqkaeb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2fmmvfeiv.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tmezhqsh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pekkxsla.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2hbhanntp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hothzxdk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ayhfzpti.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2cxgoeftp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2hhqdxowl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2iusgjuaz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jwehwuvp.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ekwyckzv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2prrkqgvm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hgryrvin.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2prmwsnzx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ckakixze.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2usegepwy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nafivnwh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2stumgshy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2dpizebsg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2xpohvxbz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2tswncgib.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2igmdnusi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2keyuswpc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2thoqeuul.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2rrqqtepd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ofoiujmd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2isjwxjex.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2rdetsovt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2lsedxxyc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2chbnqncj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2gbscodew.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2mxbbvskd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mcbomtyz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2nvklqfoz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bwlvbvhn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2yrcoqmus.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fnbxwhqa.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2hwibjlbt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cjrhmbqg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vwthyiuq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dobxsoua.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wdsrljjs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xgbuziju.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2dydxnhht.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2hdyacoeh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lrqvusyj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vxedhmnl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2rccinpbo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2tolegrln.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ptkvvyed.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2aqspggqj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2sbunqzvb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xpvlnufc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2eeuhpmfp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wvszntre.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2rqvbykby.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2djidqkeg.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2epmaxljm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zeqayaxr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ulvvkchk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2zbtojwxn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ecvptubm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pvjammyz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2rlzhvwav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jprqgbrm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2rdskjvpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvuqklzi.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2efkcmpzg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qqdireym.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2glyvscgy.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2paitfjob.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2yrtgcswe.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2kogbfdip.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2khodgdzz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2yvvsgpcq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jgqbexsp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qmgufpln.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nnvjscid.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tkkmlgvl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vjeyurfe.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ddjwutdr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sukomxek.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rseyiuko.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2uupnefhy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2slzawvwd.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2samtqqvc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2cgojkfml.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2swzfwmri.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hjcrfbzd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qtozqhbw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2pfnlteel.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kswmcrnu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zwddslze.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2dmsikvlz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2grbphbmu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2otloamqe.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2aodhjfkp.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2objzgzed.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2auqwpggy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2hagptbbq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2hmpfxrxl.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2fnuylyfl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2zganwbqu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2anaxnwzw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qbfpxjyx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vyolxqis.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jrxyeykg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2caqnlgwg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2avyixpuy.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2asgthtrc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ghteewmn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2sxykjsec.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vrrixwcz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2uaizeacf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2fvmsehxk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sfqaigsm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ieqpjctg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2mtxgfhcp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2cdxfhimd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mrttwxyd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ugqadtps.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kasjvmui.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2rxgjtioc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2msdkrqda.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rxqkkxom.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2znwbgfde.html


<!-- 参考信息 -->