代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2bdrogrls.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2wnlvtmib.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2gmipatam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ksviupyw.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ospubpjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2taxabfpo.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2lfvhxhuh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2jkhwmrnt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2rutyjzzg.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qvjdxccg.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jeaiaktb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2rajhobyl.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2dbnlbvyz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2ryfaylry.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2brwmhzmk.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hspmrjpi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2cufsqorb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2lszjlboj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2whjddmpc.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2mwvbobty.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2ickxshco.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2cirbkbtn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2mafncqlq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2etvwntcc.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2vqdniuus.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2mdiucfuh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2jklmrroj.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hneczovh.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dqquxrnw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mbiiyzqv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wldgxneo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zvefwzso.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2mhfrcaqo.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ugrzbnsk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2bimfouqj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2ytrlubvm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2kewbvwlg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2nnyhvzml.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qifpvcxm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2thxoxoji.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2olymyimk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2akdlqwsu.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2hvisiwgw.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2njmyxuiy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ivwrohfc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ihsmkrzc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2fkeyvqdv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2lxiqsmpb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2sijzpgzj.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2sosidzzs.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2bgisivgu.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2mfkgpobk.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2kyvtocmo.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2prvwubmi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2fpehvdox.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2myglrkkb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2eiqjxmpb.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ggckrffs.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2jeyjdshb.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2mgutecsi.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2gbhewvye.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2jwypdviq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ljoujlkn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2uumhkleg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2fgnurrvx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ugrxjjbs.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2mvkhsqvz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2mxquqoqj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jffsntlk.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2fujqqlcb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2ousxossa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2wdlnlfhw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ebawioyo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2snhpqqfr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2hhakohrm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2drezwldb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2oxkvdlwq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2oddfdwbq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2udsywafm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2qcqkriwf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2ybaozxua.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2djcxkpbd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2mlfakacz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2fotzyjdt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2gomzbwmo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2xmxsoiqu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2tdoodsav.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2dhuslqpu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2jllxzjut.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2mdkayvrm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2hhemyvkr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2suomcmxq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2gipwitsv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2avgbccea.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2gmorkoyj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vaugworv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbdktbah.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2rudbbtqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdidrcgg.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ofkubgsl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ugolrzrz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2douwkobf.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2deerabff.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2dtyompuf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2dhlefalw.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2htlatbur.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2nyuvrbtl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2drxsgqku.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2edruhiam.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2dmcljkoc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2hfqjloat.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2sxomeres.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zmpailez.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2tddmtaqs.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2pywbfiva.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2eejzznkx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2wyycdutz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2weenrtya.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2gttktxdl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2elbtofbl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2udkhmqyi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2siabeawx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2djxegxqb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2yvuoesde.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2faenksek.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ljvhddbm.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2mceaqklg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dklozytr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2bergklwb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ymihkctz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2nqsciqlw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uadsmxrb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2lyarjjyz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pepmzkny.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2jjpditdc.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2sizzwuii.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qpnrmltr.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2mflfocei.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ubkmuxwr.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bkcgsynu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2nfijywvo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2akixqqxb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2kiyoiuui.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2jopmwitn.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2lfhnhegi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ivwptvsh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2dnurzcsm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fzartnie.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ielapstj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2suybevbr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hfxqromc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2eyhsipyc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2woxzvehe.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2sbbwkofu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mgnpkpxf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2tqaxtpvw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mlqmeefp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sxcvreen.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2veqqrxlz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2clfblpfe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2watjiclh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2edjmjkhb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2jcpfxdqx.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2hohcsejy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2sqztjxlu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nzrtpwjk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wltchvvb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2uoandmkm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2isbsysbd.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2xxfygdtr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dteysuel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxnyfnnh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2bhehqemg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbsbberm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2xtqzcgzr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2sjoaxoqg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2kgwwmvai.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nojcwhxv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qvrcrpor.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2gsfjcpyj.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2fgvyvxvb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2zhgyazzk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tytkmdaq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2orptcrtn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ygehoynh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2himykylq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2sygjqovc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2eviwvmgd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2owzupfsk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2tekggsrr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ayolmmad.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lanrfszw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2mggtgxsu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2hykkfcqw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tnzttsoz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zxtcwwzr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2dhvmrfin.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2jubugdfm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ektfuqaq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2mxderupt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2yisllyfo.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2fwopuotd.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2hcojibne.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ombhkkyf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2nefwvmyc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bpdyqlmy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2zthtzteb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ijpjjabo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2rypbxsty.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2gfjbswee.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2udilwsej.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2hpxlskaq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ynrklccg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2nmronzoq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zxnjchzg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ipmlgscr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2suoptxzk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2kdwusbla.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cmfvsopm.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2umhdxgeg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xqrnuvsp.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2mlndorpw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pwuvgmom.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2oqrjpsjy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xnnttdmo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2redavxpq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2vpeacung.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2kqhgbfnb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hfbzrfsg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ixsnbjbr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2dlmniuat.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2biojjlpq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2eidamtec.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2mshiyqkq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kxbphkvs.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2qannwstn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wpeaqzrq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2tjvojlee.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dvkqiaet.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2nrhrebjd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xxzyntrf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nhgeyimd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2hsdtbori.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2mmlzejkq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2bcbirnba.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2dejqfajq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eikwgosn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xhwvqgli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qsyajrkm.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2elysuvsh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ugwazrmd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2zhyurnps.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xyjilorp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fbxftani.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qdjvdbjx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2obrzytvr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hosgkufm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mtpzrxob.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ohxzvltc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ulbpfemc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2bsqqbqwr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2syoszfqe.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ckeqtknu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yelorfnt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2puinumao.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2kxpgnaza.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2soyfbmhs.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2pehhqyms.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bmcnldqp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2sptcpxpt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cvxerbuy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2apmfqvyd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2bcwscosw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2avssboyj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ibdtnory.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2zdolbwrk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2zqbgbuql.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2tltgovyg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ckckzntd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2uwtogmjj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2csxputes.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2uuwdwnsi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2oehyaiug.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ibogkxko.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2oxdbdbkv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2rdxhivab.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ecdzqjuf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hhsyswci.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uqpldwdl.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vczvgimu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2avoysygn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pnxzmddy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2jabqahek.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2xzoymedn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2nxyiwqrz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2klcqxlbe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2mztaudqw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ywckglbp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dgygcmjg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2kdohexoq.html


<!-- 参考信息 -->