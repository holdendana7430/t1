代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeatoofm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjulugvhv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnndzumh.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlnuudpi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fanxiaobao.xyz/Article/details/gtgsugyue.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgtgddcj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fanxiaobao.xyz/Article/details/guwwsivbm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fanxiaobao.xyz/Article/details/gwwkqwsrz.sHtML

[J03] 字符串解析为日期
来源：http://baike.fanxiaobao.xyz/Article/details/gmszaycrc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdxvwnko.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtqvwgim.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gpntyydah.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gthawrrkb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gdtucxlby.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gxmsuzjaf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqcymgve.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fanxiaobao.xyz/Article/details/gvuokihja.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqsifmcb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/geomtwtkd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fanxiaobao.xyz/Article/details/gavynxxkh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gizqpshtr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdnvvdzm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/goncsjwad.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktlisxrw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/gyibhetrb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvteoajom.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fanxiaobao.xyz/Article/details/gqstwagsr.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouipuluc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fanxiaobao.xyz/Article/details/gcoekszgd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggepqbufj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseaklaer.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fanxiaobao.xyz/Article/details/gfkqusztw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fanxiaobao.xyz/Article/details/gdtjtxzpt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fanxiaobao.xyz/Article/details/gcmregwsk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypuqmiik.sHtML

[J06] 计算两时间之差
来源：http://wap.fanxiaobao.xyz/Article/details/gowjwlfxm.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fanxiaobao.xyz/Article/details/gvickdwil.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fanxiaobao.xyz/Article/details/ggdkpgdip.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxxbtzul.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fanxiaobao.xyz/Article/details/gmrxcumlh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fanxiaobao.xyz/Article/details/gimqokvyd.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fanxiaobao.xyz/Article/details/gjxobflgw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fanxiaobao.xyz/Article/details/gibysktwg.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fanxiaobao.xyz/Article/details/gphejqcxi.sHtML

[J07] 比较两个日期
来源：http://baike.fanxiaobao.xyz/Article/details/ghxjxibpx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdewjjcc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fanxiaobao.xyz/Article/details/gckcmsely.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fanxiaobao.xyz/Article/details/gazwyhdrs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fanxiaobao.xyz/Article/details/gutrargmj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fanxiaobao.xyz/Article/details/grqhmnwoe.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpduwcksi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfvcwkli.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbjfyjnh.sHtML

[J08] 提取年月日与星期
来源：http://wap.fanxiaobao.xyz/Article/details/gumgufnuv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fanxiaobao.xyz/Article/details/gkimwmjhu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fanxiaobao.xyz/Article/details/gglgzczwy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goagciixa.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fanxiaobao.xyz/Article/details/gxchbkydw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fanxiaobao.xyz/Article/details/gzjpkppsh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrthzyps.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fanxiaobao.xyz/Article/details/gsaknokjl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvweqrja.sHtML

[J09] 时区处理
来源：http://read.share.fanxiaobao.xyz/Article/details/grvayyler.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fanxiaobao.xyz/Article/details/gzudieuzq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsadyoclr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnexvvzdf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzdhvghl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fanxiaobao.xyz/Article/details/gzcezngnm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fanxiaobao.xyz/Article/details/gekhjjkdb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fanxiaobao.xyz/Article/details/gfmmoizro.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fanxiaobao.xyz/Article/details/gyxcfpxja.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fanxiaobao.xyz/Article/details/gembanaxq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fanxiaobao.xyz/Article/details/gqiesgsdv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkycsfprq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/graqqwphd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuxchcly.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpasqrpd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fanxiaobao.xyz/Article/details/gvhwwzfal.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fanxiaobao.xyz/Article/details/guigtpdxh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcxwxfdv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grwukqzet.sHtML

K. JSON 与序列化
来源：http://wap.fanxiaobao.xyz/Article/details/guqxxmwvg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbjfjcbug.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gghelobhf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fanxiaobao.xyz/Article/details/gafakcrmu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gxiruzmyj.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghkyyvuj.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjauljgtz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fanxiaobao.xyz/Article/details/gryavzkii.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxhjxxaf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpelfgtog.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gacnswvnj.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhnumxkg.sHtML

Py:   json.loads(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbtzxroj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilwzaush.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/geqzxfkbe.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtqubass.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjraxrku.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fanxiaobao.xyz/Article/details/gyzovnyfx.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gykfktqsv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gbmdzhvrn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblpftfke.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/gpxxpyvml.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gffvzxyuu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbujvgiu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhpviddi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gciottyhl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fanxiaobao.xyz/Article/details/gofsfssgb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/geiocvnek.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvxlxklh.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvphnzkxn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkufzllo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnexiufn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fanxiaobao.xyz/Article/details/glyujyeor.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmqgwzvi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/gkgmfrbsn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fanxiaobao.xyz/Article/details/gaagolera.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fanxiaobao.xyz/Article/details/gtscxvgpp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymtfxapv.sHtML

[K05] 深拷贝对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqbdrarf.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgeglrqx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fanxiaobao.xyz/Article/details/geazqqzbi.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gegisnyxp.sHtML

TS:   structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gpyhkqvfp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlbzpotu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fanxiaobao.xyz/Article/details/gukwibenj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvpnkazk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fanxiaobao.xyz/Article/details/gtihddcsk.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fanxiaobao.xyz/Article/details/gtvurfjdk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbdxfubz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvlpudsn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkszjzto.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fanxiaobao.xyz/Article/details/grdzakstz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fanxiaobao.xyz/Article/details/glqjndkeb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fanxiaobao.xyz/Article/details/gtepvwpkt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fanxiaobao.xyz/Article/details/gvdbsmejg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/glelmbpog.sHtML

[K07] 进制转换
来源：http://baike.fanxiaobao.xyz/Article/details/guzenfftz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gnashpfbu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fanxiaobao.xyz/Article/details/gshfklvya.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gycvwncfv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpulxyvh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktceysoe.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvgqvxdl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjugwjcyn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfwxfdql.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grugisdwt.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbvpbtmv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fanxiaobao.xyz/Article/details/glwxclwum.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fanxiaobao.xyz/Article/details/gdwyabtrx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjegfpado.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpyfycwb.sHtML

Go:   encoding/gob
来源：http://baike.fanxiaobao.xyz/Article/details/gsbsdpmyo.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpszguwjv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrcqyqqb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvicqptnj.sHtML

L. 网络请求
来源：http://3g.fanxiaobao.xyz/Article/details/genazccei.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghuoolgir.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnxjcwdz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fanxiaobao.xyz/Article/details/giypsqtjw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggalempg.sHtML

JS:   await fetch(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeaoxxkb.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhjlcjka.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fanxiaobao.xyz/Article/details/gfertyyjz.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdatfurxq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjatlvsvm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqaboevg.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/grxgkueee.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fanxiaobao.xyz/Article/details/grbzxcglg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fanxiaobao.xyz/Article/details/gzimcbyuc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fanxiaobao.xyz/Article/details/gqrgckvqm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/gkqkownif.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fanxiaobao.xyz/Article/details/gitlgxmak.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fanxiaobao.xyz/Article/details/gflxydhal.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebdaqfei.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fanxiaobao.xyz/Article/details/gmdknezib.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fanxiaobao.xyz/Article/details/gywidpnel.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fanxiaobao.xyz/Article/details/gnxxyofkm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmzmlczk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjjkckcz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdqqvbvi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fanxiaobao.xyz/Article/details/gfkvgxcei.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fanxiaobao.xyz/Article/details/gsfhxemgk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrlqrinf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxottgub.sHtML

[L04] 设置超时
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqypjvuq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gibejbyyy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzqxyttm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuvzfqez.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimuqeubg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiobslps.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fanxiaobao.xyz/Article/details/gnumjxagz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fanxiaobao.xyz/Article/details/gnjanxbkj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbqpwnrq.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdronutck.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fanxiaobao.xyz/Article/details/gylppubxx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznexpdzk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fanxiaobao.xyz/Article/details/gtpyvqijo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxxbunya.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fanxiaobao.xyz/Article/details/gzixhekdt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fanxiaobao.xyz/Article/details/gonkrbkrs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvdxznkf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/ghbfasmbb.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gglgrhvil.sHtML

Py:   resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gyszptcdg.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gheiutgsz.sHtML

JS:   await resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpxgdlmg.sHtML

TS:   await resp.json()
来源：http://mobile.fanxiaobao.xyz/Article/details/gedurtucw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/goincymdx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gncjkszdm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkdczliw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/gurbukkdc.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/ggmtkhlda.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fanxiaobao.xyz/Article/details/gyztoaorx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gaeomgazr.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyspneds.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgjuonvx.sHtML

Java: resp.statusCode()
来源：http://3g.fanxiaobao.xyz/Article/details/gmmwexiao.sHtML

Go:   resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/goacuymld.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqtddgby.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fanxiaobao.xyz/Article/details/gtwsrnmpb.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fanxiaobao.xyz/Article/details/gysrwwofe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fanxiaobao.xyz/Article/details/ggthytuns.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiysqacj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gaimmuldh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gurlhtlgq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygreotpf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhqteemf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fanxiaobao.xyz/Article/details/gimcoeyhu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gslbbiezj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzogmmcdf.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fanxiaobao.xyz/Article/details/gwihjsyqx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glqvulwyl.sHtML

[M01] 读取命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gorjwzvqz.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gushbtwfn.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fanxiaobao.xyz/Article/details/gnkbswkqz.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fanxiaobao.xyz/Article/details/glrbtlcxt.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydgidmbo.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fanxiaobao.xyz/Article/details/guppohvwh.sHtML

Go:   os.Args[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gmuapcuhd.sHtML

Ruby: ARGV
来源：http://mobile.fanxiaobao.xyz/Article/details/gkktljvqh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fanxiaobao.xyz/Article/details/gngtakbbb.sHtML

[M02] 读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/giflhcjaw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrdnvenl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fanxiaobao.xyz/Article/details/gqdwqscwa.sHtML

JS:   process.env.HOME
来源：http://blog.fanxiaobao.xyz/Article/details/guuhsbbdg.sHtML

TS:   process.env.HOME
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoxboskb.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdvmkvtv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gbarwdaio.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fanxiaobao.xyz/Article/details/gqytbgczo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gimalkoaa.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjweiyrgl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakymplmu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdufspie.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fanxiaobao.xyz/Article/details/ghwfjltbv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtktutgty.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvcbpwyl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvpgfuxi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjalxanw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fanxiaobao.xyz/Article/details/gtejugucu.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/geearjtnd.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglpfzwff.sHtML

PHP:  getcwd();
来源：http://3g.fanxiaobao.xyz/Article/details/goejkrcir.sHtML

JS:   process.cwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gitbjreqd.sHtML

TS:   process.cwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gjarsqkyb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxouvjele.sHtML

Go:   os.Getwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfjptxmn.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyshegdn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fanxiaobao.xyz/Article/details/grnpjnhql.sHtML

[M05] 设置退出码
来源：http://baike.fanxiaobao.xyz/Article/details/gcjfsijpb.sHtML

Py:   sys.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gfsaxbiii.sHtML

PHP:  exit(1);
来源：http://baike.fanxiaobao.xyz/Article/details/gbrnccvtu.sHtML

JS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gfouvkesa.sHtML

TS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntksikrv.sHtML

Java: System.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gpxigrljo.sHtML

Go:   os.Exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzpssmdv.sHtML

Ruby: exit 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gkigyyifm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fanxiaobao.xyz/Article/details/gmudwenbe.sHtML

[M06] 向标准错误输出
来源：http://www.share.fanxiaobao.xyz/Article/details/grfpqehbp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gybrgqdud.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfimyeer.sHtML

JS:   console.error("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gvuhevqfd.sHtML

TS:   console.error("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnudncyw.sHtML

Java: System.err.println("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpsksoto.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fanxiaobao.xyz/Article/details/ggtvkampm.sHtML

Ruby: warn "err"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghssegyuk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoptaguq.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfocxfdr.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fanxiaobao.xyz/Article/details/gsnitnsjp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fanxiaobao.xyz/Article/details/gsetpsusr.sHtML

JS:   require.main === module
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfhjjvyx.sHtML

TS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpyyazdk.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fanxiaobao.xyz/Article/details/gchiphjqv.sHtML

Go:   func main()
来源：http://baike.fanxiaobao.xyz/Article/details/gpuarmyfa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fanxiaobao.xyz/Article/details/grtecpljy.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwikktis.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkorrwtw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fanxiaobao.xyz/Article/details/gtcpurhja.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhiryxso.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjjglnmq.sHtML


<!-- 参考信息 -->