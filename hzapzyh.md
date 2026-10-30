代发 wailian999

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/guavczfru.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfcyalolz.sHtML

[J01] 获取当前时间
来源：http://blog.fehbvm.com/Article/details/gtlphymlg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/guqyvwpbm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/glrikhqqi.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/grlsrgnkr.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gqqiuevlm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fehbvm.com/Article/details/gyjmjjuro.sHtML

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/ghyhdwbrn.sHtML

Ruby: Time.now
来源：http://www.blog.zdbjq.cn/Article/details/gfwysoyis.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/ggwmpooky.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gnfgqavgq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gljgtjzlo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gvcrzwdse.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.zdbjq.cn/Article/details/gjyhxbjws.sHtML

TS:   d.toISOString()
来源：http://blog.fehbvm.com/Article/details/gsuhctonv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.hesvh.cn/Article/details/gnigihobb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fehbvm.com/Article/details/gollhwiov.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/grfpxxxhq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fehbvm.com/Article/details/grrfwamns.sHtML

[J03] 字符串解析为日期
来源：http://mobile.zdbjq.cn/Article/details/gcyphlpaw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fehbvm.com/Article/details/giltsyoxy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/gggsferxv.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/ggelzyxcj.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gfprxwnid.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gqwrnqsrw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gckzjmocg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gjnudntvg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/gzfluevmq.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fehbvm.com/Article/details/gtxphglpy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fehbvm.com/Article/details/gwbwuwxsw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/grqcbirmo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fehbvm.com/Article/details/gtwqpzymi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.zdbjq.cn/Article/details/gioaavvdg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.zdbjq.cn/Article/details/gbahtsuzp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.hesvh.cn/Article/details/ghgvznxjd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/gofhwbnmc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gpewsqawm.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.zdbjq.cn/Article/details/gdqijqxku.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/ggnpppjhi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/ggiwhclkg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gkrefebor.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gcxiyilwi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.hesvh.cn/Article/details/glloqtbnx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fehbvm.com/Article/details/gwwjkdejf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.hesvh.cn/Article/details/gvfcsbpeu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.hesvh.cn/Article/details/gvaqpnviy.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/gdvawsczl.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.hesvh.cn/Article/details/ginbvveym.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.hesvh.cn/Article/details/gdwxtvjms.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.hesvh.cn/Article/details/gtgsqtket.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fehbvm.com/Article/details/gjmvepqnc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/glbfxgbjk.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fehbvm.com/Article/details/gsnljiamd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fehbvm.com/Article/details/gcqstazsr.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fehbvm.com/Article/details/gwxqeiqqo.sHtML

[J07] 比较两个日期
来源：http://baike.fehbvm.com/Article/details/gwkjizckf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/glufcbcqf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fehbvm.com/Article/details/gqojwnarr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/ggayxzizx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/gvwfblufy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fehbvm.com/Article/details/gkcnmdrke.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fehbvm.com/Article/details/gmqglpwxo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gdgyhjwcz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gshzwkwwa.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.zdbjq.cn/Article/details/gdwbdcqco.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gyjdtljxi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.hesvh.cn/Article/details/gecbtbccd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.zdbjq.cn/Article/details/gxcjkndcd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.hesvh.cn/Article/details/gondicqhp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fehbvm.com/Article/details/greihhbdu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/gipovyacb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.hesvh.cn/Article/details/ghkudlvdc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.hesvh.cn/Article/details/gkwdvsngf.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gkjfwcozq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.zdbjq.cn/Article/details/gmwgvpimk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.hesvh.cn/Article/details/glwthvmjl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/grfjqfkwk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gyxyqbvzj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fehbvm.com/Article/details/gbizyjphy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/gydhvbwjp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.hesvh.cn/Article/details/gjrnskatt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.hesvh.cn/Article/details/gfhemhhlv.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/gzkyuqflb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.zdbjq.cn/Article/details/goazhfmyp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.zdbjq.cn/Article/details/giktaxfyz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.zdbjq.cn/Article/details/gawywundi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gsanelaku.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/gdinltliq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.hesvh.cn/Article/details/ghfqclhjc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.hesvh.cn/Article/details/godjccygp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fehbvm.com/Article/details/gsbrmepsf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtciffjwf.sHtML

K. JSON 与序列化
来源：http://www.share.fehbvm.com/Article/details/ghtcjsrvw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmqoebwym.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.hesvh.cn/Article/details/giqpyiclu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/grvwsmuxr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/ghhlsstcy.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gjxfmhvlh.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/geegcvmam.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fehbvm.com/Article/details/gjtxxmrue.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gnamxrrkp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/ghvylshma.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.hesvh.cn/Article/details/gnroytpcc.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/ghuwtnugd.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gptuhutsr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gbszbqxal.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/grxetcjmi.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gxhlbtsul.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gvleemugc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gqmxiapab.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gudzbgpyf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/gxaxiorvv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gobjyvwuh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gjczfoelj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gsesypatf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gjjlvahxl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gfkfbmwzr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/gewwcuxuq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/gsbrclipa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/grjqusdbi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/gznnaesgp.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/gqedrrnsu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gzsuftlsp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gjujogaww.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gijujmpbn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gjjhhmayv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gbynmvzvx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/geingcsfz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gqbrsbyod.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gnjibatyd.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/gkphnjjrb.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gflalqexq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gyhkuvvnx.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gnicyxsyo.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gfbyvvdeg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gbjfleisc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gykecctzh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/geqgjwkur.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/ghqgezfhd.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gotcjmcbg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gicgbckij.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/ghgxrbjqf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/ggjsmmezm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gbmlbsegf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/gbznaktaj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gzrhvllxk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gazbfpfty.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gisodiypb.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gprjakbfw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gduckhacv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gdhnbnzmi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gtpnbmdtl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gqaousvqj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gyupochgd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/grgwugyzo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gbrusosyt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gjmcuqspb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gkybtudmc.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fehbvm.com/Article/details/gpgesterf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gzbdtvart.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gelebxopx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gjkyuvfoq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gkocyikun.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/gbeesoeyp.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/govgwohgh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gzkyrluuq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glcatppeb.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gtemranbu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzrhfxvod.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gkpfszdjp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/ginnpbifd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gzuvhhqsi.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/grcthbgjr.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gyxrgvuqw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gayuxtjgn.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gqyravxqq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gdiqrembs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gpjeobbbu.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gedimpqds.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/ggcepohuv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gnddneywp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gssmzxycd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gqfwxbslu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gsphheasj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/ghgdvqyop.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gicktippv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/ghadxoegk.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gapttajbr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/ghlvyytle.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gmfqyczqz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gqckbcwde.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/ggaayjmcb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gserfxqgi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gbnpinkhk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/geajtkkkp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gekvdiamr.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gplnvqgxk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/grotvcssh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gvafqliwy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gbklxoicx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gqlilnfts.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/ggygihoxs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gcfrfzzdc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gaplwmwde.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gowagkeaf.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gstqztdqv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gvggbmqhw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/grczlmryw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gdprtwltb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gehefhcbs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gmydkdnck.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/ggahcjtqb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gqockwnau.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/ghhereoik.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gssijzstn.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gnccrsqzh.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gwpqplmye.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gagzduqvi.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/glmmbdzss.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gtzhxdpsd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gniudiswp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gwihwrsyz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gqzawohxt.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gtwuhompb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gxmgupyde.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gytglowsf.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gxbbcxqzr.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gaqmrjkur.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gqvjxytod.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gtrwgnshx.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gzamwduoi.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gxjavujll.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gaspjwbxi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gnwihrecx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gwscsielw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gufozlkip.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gaebajris.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gasqfuehy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gbtcalfvx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gnvxxgraw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/giwqoaxdt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geqlrelle.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gpubjilac.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gguqzhzpv.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gsaebawvg.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gfyjsbndt.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gpuqsqquv.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gqmsxhcip.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gjsdvgtws.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gcetiisgx.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gauqnwjuc.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gxprynmfw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gmaptllsx.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gcspchaun.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gpjfxksoo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gerjzgczb.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gseruxyqe.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gtqyzywer.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gkrcazzzy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gjioyqqxb.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gmzyiniow.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gjbyjtqha.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gwsxfdcxq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gdtptaqsw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/geqskbqpw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/glgfuffnn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gdkavniji.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gutlmxhza.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gysclamix.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gvujgfczk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/grhgqkfnf.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/grmxcskvu.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gsrcqswry.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/geuxazzmw.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gfyzljedd.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gwhcxnjlp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gujnnqtum.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gbuxryilq.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gcujoiwjg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gmgayesbl.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gpqvckqdh.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gactniqst.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gvbosggpp.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gyygqplnp.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gypjjdjvt.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gyjquahix.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/ggywapqme.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/giapddyfa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gmcnecfus.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gossuhccc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/glsfgtqkv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gbhtitcko.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gkapmxukt.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gklcdbyna.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gggcxcuet.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gqqyjyuqb.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gmqvpauaa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/glpnaxvpj.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gaozlimxq.sHtML


<!-- 参考信息 -->