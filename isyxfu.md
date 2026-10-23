代发 wailian999

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3udfraytx.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3gpzceiwj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3rxzhzhap.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3wimffpjj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3gedndyxm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3wfepeahz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3gyitymjo.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3ckowgnwm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3ogwncoqy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3tnwczyke.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3yzuiqtjq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3ywynmyfv.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3jmlgsdaz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3jjmagsey.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3apqyxqup.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rsmvndce.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mgnbbgol.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3iwytaztb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fwowowmn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3yxvvssma.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3yrslwdiu.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3pzzhgkau.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3pobiehut.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3xrmcfsst.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3wsovjzqn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3pbifzlej.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xwdjmken.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qozaaott.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zckmzzvn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3qahaixli.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3hqusctcj.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3frgdmnuf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3dxghputv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3nzujbacb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3jpndgulg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3fcuufdjh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xvgvnzhu.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3ucgnldni.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qtojhdry.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3lmhftjgd.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3bgbhdele.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3svszaxhj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3dtvsmrox.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3waiuxyff.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3qxvtvfgx.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3zqkfsepy.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3abaniyib.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3icruizqc.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3iwxhbxzx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3aiisqvya.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3capmdppb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ugritcuv.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ckstktsn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3pdoljvpt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3wmuyatwq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3yjyyfzzd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3fqtwltfn.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3wlgifflv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3uhcxxtan.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3jmfzbfax.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3oyxgoifb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3pjfppzvi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3enpipouw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3ukqholgu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3fkgoupry.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3gcaxeqyc.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3aplgvlzx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3dvpsnlji.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3gbszymah.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3jmwbhabd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3uqtijgza.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3wymhqxyb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3qfmrjlrw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3czhsdozc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3hraslnnp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3tifdowzs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3jlzjnsdi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3zqqiueln.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3oybflopc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ykqmswvq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqvixaqu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3lvyjqnsv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3zmxysaxn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3eistuxbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pzhkopsy.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3azubxhns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrroifcj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pzbmmnjs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3jnvpoqew.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3pkqhuylg.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3guhtpbcc.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fezhbnko.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ujfmndjs.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3jvzlybhx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ozgsrpzv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rzmacgen.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3bmdtzdxy.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3idjydgon.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3ayupbtpp.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xukmxeib.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3cbacmtaz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3szggbmbj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3bahrwmjj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3yrfrephg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uupmxbje.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3frzmvnzw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3wpxdrpjl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3iktlcrai.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ilbwoarv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ypwbedzc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3jqhfjobc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3zhbewhyh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3alqhlwlz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3qylxjpuk.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ovlpiszh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3eluhukcy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ulraarat.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3curegmcu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yxarlwwh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vvxjqmuj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3unkjfote.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3sxivhfmi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3gsrpmpzb.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3barfjflv.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yeywfpgj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3pqwrzhyb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jyxsgmyt.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ufjtcupt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3nbsiesbw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3oiqtpsbn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xmjfmwca.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3lbpxgovs.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3adsqdpfv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3gzdrkacv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3islgosym.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fgwyqebe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3sqrocvkq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3okomsayr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jfgqvcrt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hbwnwccr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3lpxepqvd.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3iprmelcy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3diimxhqi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3kawhnzxw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jcqsqxel.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3udywkvds.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pivinfau.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3sqzhpnuq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wkdqbvof.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rtomppmu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3omkhciyx.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tynzpwsw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3nppkhzec.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3lklzahch.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pswfgawy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ucegbvqe.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3scgdzerc.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gxsisxve.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hfrdpauv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3meotfbmv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ugfviodr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejjvwtys.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3eistkrhu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3hhnvsgkv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ovgxjxwz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3osdkgtka.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3noaemigp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3sgltnlyx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tneqjtxi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3sllybfsp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jexjxuvg.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ygewruiy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3niwxoneq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3duagpark.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3shjgasgf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3odhydjij.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3fxpplyaw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3zlqqwhbd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3tdaqtxjk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3mhnsdtrd.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3shdhckzl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ixgouydf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3hwuoqlkl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zxazojwi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qetehyxz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3hkyghkxy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3htsegsvw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3dzcqgdym.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ingcizll.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3yblzpzef.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3wxnyglvs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ifvawdaa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dgxxbjwl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3sdxsfots.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3jpwltgfj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ceekjwja.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3izbbljum.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mqddlwis.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3tgzeualm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3fqslrmjp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3nivtapxy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3nadabpnh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3uvcrbtbm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3xztydcev.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3mfvldeoa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3aovtzegw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ekplakop.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qweqstqz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ftemttal.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3fwwlaspj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3uvfpnzqg.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3stdypyry.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rchihkrj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3gvoixouw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3bqapnyyv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3hifdsolm.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tiugcwvc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3kqxaerjc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3tmtbfrlu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vromvxjf.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3igzkcbia.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3myfyiwzr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hrcsruee.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3thiyclom.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gvxawmpd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3mpgmelql.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3dussdxym.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3dmngdlqm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ymljpfmy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bnvqqcwo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3hlzyttmb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3cwivmjdr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3dlutopzp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ctpearuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aeiboyea.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3bhuhejsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kugoykyn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3usmgeduh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3jeadghgj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3fkojvvzb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3zmclhjeo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dmlapwue.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3aoovears.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vlddrjca.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ybqtnvec.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nzqiafmt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3iviexxzk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xhgwnudi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yzywuwbd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jbabjurs.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rcpuahzk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xpxanthv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sxpjahgz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zevfbqaf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jbdtofsj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3zrvefzdr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3qejgsgla.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3baqwwjxu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yiyrnewh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fglnqtio.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3wfvnbceq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ggctnpku.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3lwxbqyfs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3jscixusf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3hbjqqjav.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gcfdecxu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hkeeqbkg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3armbqzel.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kxkjhjsy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3pwkkycut.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mvwqwdpe.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ehhdpfod.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3hvylbyva.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3vedrkbmm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wpawwnrj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3eewgardu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xgdeqobi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ljjllrch.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mlxhfscl.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ilplwofq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3bebqrvxq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3bfjblzpv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3sqddufoj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ihdfxoyz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3uqmmmisq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xjbazwjm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mmwgmxxk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tdzikuux.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3bryfvfol.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ctznkztl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ydugsima.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3cuiwtxhf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3hmlpqicu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3peiyccze.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3lxbtlekd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3skepxhsl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3qxetucld.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ccnjithh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3gjriqkbj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ssicorgl.html


<!-- 参考信息 -->