代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gqhxesrbu.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gavyfklup.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/goqmccizd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.zdbjq.cn/Article/details/gftmunxbb.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/gdfusrzix.sHtML

Ruby: Time.now
来源：http://www.blog.zdbjq.cn/Article/details/gghcpnrpg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.hesvh.cn/Article/details/gkdagoyct.sHtML

[J02] 格式化输出
来源：http://read.share.hesvh.cn/Article/details/gcqcmtyti.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/glrladamm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/ghsbotfhm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.zdbjq.cn/Article/details/ghdfmgbmt.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/guljmggfs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/gyelhgeat.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fehbvm.com/Article/details/gxlczwfdc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gzrjlixae.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/ghnjixfkm.sHtML

[J03] 字符串解析为日期
来源：http://blog.fehbvm.com/Article/details/givcpemoq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fehbvm.com/Article/details/gyhpjgagr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.zdbjq.cn/Article/details/gvgcvudny.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gmttnybvt.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gyajeudps.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gcfxglwyo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gudttsvsn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gjjojkgkx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.hesvh.cn/Article/details/gcerkgtsa.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/gqnlexmsj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.hesvh.cn/Article/details/gectewgpt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.zdbjq.cn/Article/details/gdjlfmkqi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gighrwikb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.zdbjq.cn/Article/details/ghouyyosw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.hesvh.cn/Article/details/gwlbsifpn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ghbzuacow.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fehbvm.com/Article/details/gmqrdwbvn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.hesvh.cn/Article/details/gkzhzqrpw.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.hesvh.cn/Article/details/gfeusezqj.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.zdbjq.cn/Article/details/gefzopvzd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.zdbjq.cn/Article/details/grsetibfe.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/ggubgimwi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gbwjdckvz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fehbvm.com/Article/details/gosfgdwop.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.zdbjq.cn/Article/details/gvinmexdw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.hesvh.cn/Article/details/gkgheobbp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gzlxpmvte.sHtML

[J06] 计算两时间之差
来源：http://blog.fehbvm.com/Article/details/gmiwzukaq.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.zdbjq.cn/Article/details/glycybobw.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.zdbjq.cn/Article/details/gncltssje.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.hesvh.cn/Article/details/gsfmglkbj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fehbvm.com/Article/details/gdbnqyuoz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fehbvm.com/Article/details/gjcyzgwua.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.zdbjq.cn/Article/details/gndeeuxxh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.zdbjq.cn/Article/details/gcicfsuhy.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.zdbjq.cn/Article/details/gqikpwruu.sHtML

[J07] 比较两个日期
来源：http://wap.fehbvm.com/Article/details/gfasfpysw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gmkvevfyz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/gdkqrbcun.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gbqnriqzq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gyuivmrny.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.hesvh.cn/Article/details/gvdmhfppy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/gagetyrar.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gvbsqwsqb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gvqfxiyyk.sHtML

[J08] 提取年月日与星期
来源：http://baike.fehbvm.com/Article/details/gyqcobqoh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.hesvh.cn/Article/details/gpzdyryqn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fehbvm.com/Article/details/gyfvknaaq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.zdbjq.cn/Article/details/guckgvxut.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.hesvh.cn/Article/details/gigidphjz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.zdbjq.cn/Article/details/ggwyvaist.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/gvoiincyy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fehbvm.com/Article/details/gedqyedtx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.zdbjq.cn/Article/details/gzcftzbjj.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/gyvxtvhab.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.zdbjq.cn/Article/details/gemmpinme.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.hesvh.cn/Article/details/gfjvqhexy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/genszsusd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gxmwgavpo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.hesvh.cn/Article/details/gzzjezman.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/gztahrviy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.zdbjq.cn/Article/details/gbdozclpw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/gkflhqnyq.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.hesvh.cn/Article/details/gdbxlvjda.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/gzqpagbpv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.zdbjq.cn/Article/details/gnfnjbbiz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gppevhhph.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gnhuslhuf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gpawkfdfr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gwcputgmj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gtdqthgif.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.zdbjq.cn/Article/details/gdwyyrceo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmjugpmag.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/gxrhxekhi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjgpfpqsk.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gcumdzxvc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gklsgroii.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/glwbrwedi.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gfvlwdbfa.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwlwjwpqk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gqfvsrwgz.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/gbwypefgx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gjowrxhgz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.zdbjq.cn/Article/details/gtevyeocd.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/geltsqpib.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gibnbjgzr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/gxyzqtqhv.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gicsmfwle.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gegwjirim.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gempkdysk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gmdzjbmht.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gvmptklzb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.hesvh.cn/Article/details/gdpicsbjo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/gfvaiiqwi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gasesbgrl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gmxyqksvd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gzaoxmhtm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/ggyicrebk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/gmxpxpbdi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/gkrzzytrw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/gmejpyesy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/gqyllyexw.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/ghypgemgr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/grpupbdqm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gxwdscsor.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gtbtxzhfe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gqeblanlo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gfrlcgfiu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gmpnhokak.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/guwmjbeog.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gczjjnrnu.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/ghmqccueo.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.hesvh.cn/Article/details/glkpbpkgr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gubdcnmjs.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gaztlyxee.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gxvdzaksr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/grtnyjiat.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gsrbrcelc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gocclgamt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gnuxkdoec.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gaepvclol.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gteganfmj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gvuftujsx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gsphtakbf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gsbxbasds.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gegllkbpv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gfrzuvags.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gkgjfkfex.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gsuwuisiw.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gokzghwbt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gkbbywzvb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gmdclsunw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gkjaomocx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gjsqyfrfz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/garllkfsl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gvhvmsqaq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gphnokdet.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gkwuqvblo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gcfaindut.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gbjezffeo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gqshlgazs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gcbggxtqi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gofrsuejr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gygdzizcs.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/galexcqdp.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/guzbwejco.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gmoeufcdw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyuiwtmwj.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gwulgytnj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtimobgqr.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gizlkalrk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gqutewjsh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gemxjvcgn.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gylmgzdkr.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gvtwolmph.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gjiomyyuh.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/govnixizf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.zdbjq.cn/Article/details/gsiigcekp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/godorllzo.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/ghzjdurvl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gvaaxjbrj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gnpgbsyou.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/ggrokhcaz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gbdzwukdx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gicfbpusi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gwjmmknij.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gnqkkiawq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/geekvfxfb.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gksnqlrgp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gdzeyoqsi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gokxvfbcw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gpdncvjjf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gdyniqrlx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gjjjtqazc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gqxrdznqt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gwiitsage.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gxmyopswh.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/ghtyfunue.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gxkugdmkt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/ginoxxptj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gjotmbzdp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/giouhpurb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/glkuyhttn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gwcfhskhe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gmrmmhphu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gksiupyvr.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/guulhfrjd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gxbbsgtyk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gfooydruq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gwpawdbfp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gibgqrgag.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gkaegtbfw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gjidyphpl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gzseplaxe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gkqvuruua.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/ghwwlihvi.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gyhptqgst.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gcmpmejzy.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gexbdavzc.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/ghoddfgek.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gkdfpqfdf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gxkmuohbm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gtkehwiww.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gxixmzpou.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gsanfwict.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gcrdqqope.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gszbfcivo.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/ghlmkqopx.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gwkreemgs.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gxawnxdrf.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gsffngrvb.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/ggayowega.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gdfomzslq.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gtmqaqrga.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gxegpwdgr.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gstyqbhig.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/grsnxhtln.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gjfzncxnw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gydiodaes.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gfrumatzl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gzrjigcmq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gtnpupvfy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gczpevrhv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gptzqitsc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwtajakkg.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gmmzvksvm.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gkcogmjcv.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gubklwhgc.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gwxsgmcir.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gfjuluqmw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gasinryeh.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gwdydtenm.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gsosqlvxm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gfvzisofs.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gqqllcdpb.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gwadphqqt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/ghoylqqks.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gsdqbjchl.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gpskcrwpz.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/grzfqwmkv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gqizwrmcp.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gtyicnlmp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/grpsiejlh.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/ggbqhiwqc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gbehrmpzf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gwmtptatp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gtiltorwt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gcvwyowgm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gfvugsydr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gytwsvwms.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gkyazxvvr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gjkcsmsyy.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gkzsknjrq.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/giozocebr.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gpcjudzyd.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gcskyhxds.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gurenbcdd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gvhvoujkr.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/ghamhuyce.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/glnnewjad.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/ggiibsmkk.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/glwskiqqz.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gjewlbzye.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gaklpsxzm.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gqelanulb.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gnftjhozp.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gsgbehimd.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/glwnzsvia.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/guugbfnpx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/grrtkvxcv.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gdsvfaxxt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gdghjyplq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gcjfoknxk.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gqicqjoqd.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/ghlmlxrqy.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gjzhpqsnc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/guffzitya.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/giyqxtyml.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gygogplau.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gywkbitgs.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gwyazifkt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gwvmofwwc.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gpofotihn.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gnurcmgkh.sHtML


<!-- 参考信息 -->