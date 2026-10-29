代发 wailian999

J. 日期与时间
来源：http://m.share.zdbjq.cn/Article/details/gegiqjgap.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyxpqwdyf.sHtML

[J01] 获取当前时间
来源：http://blog.fehbvm.com/Article/details/gjeqcyaet.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fehbvm.com/Article/details/gprqlwuug.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/guuuegibx.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/guajtjqof.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gcegocvdm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fehbvm.com/Article/details/ghvdizeam.sHtML

Go:   time.Now()
来源：http://www.m.share.fehbvm.com/Article/details/gkmrqxsgv.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/grfrpeofd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/gucanbjlq.sHtML

[J02] 格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gxovbxpvg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/gqmwyeefi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gxzrjbdio.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.zdbjq.cn/Article/details/gmdsnkmqh.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gcvarwvqt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.zdbjq.cn/Article/details/gaezelvnu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fehbvm.com/Article/details/gkpbokrgk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gyslxxgwl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gbsgftegr.sHtML

[J03] 字符串解析为日期
来源：http://3g.fehbvm.com/Article/details/gxglroweg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gfqttrykp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.zdbjq.cn/Article/details/ghuyhdqlh.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/ggvwjxeag.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/ghszxbhqt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gomizzfpw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/glbsaxbsh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gfzmlpplg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.hesvh.cn/Article/details/gznbneymt.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.hesvh.cn/Article/details/gvtmhejjk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fehbvm.com/Article/details/gznfumhwx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/gepknqxls.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/grailerwk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fehbvm.com/Article/details/grzyfgsmp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.hesvh.cn/Article/details/grgjxfrrf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.hesvh.cn/Article/details/gdvwflkbb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fehbvm.com/Article/details/gcclotdfu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.zdbjq.cn/Article/details/ggjsmrmov.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.hesvh.cn/Article/details/ggxgvyfhu.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.zdbjq.cn/Article/details/gihcmbkgt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/geuthprpb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/gtlbblcan.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gmvpewfmt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.zdbjq.cn/Article/details/gjrylqnde.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gdbiyksge.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.zdbjq.cn/Article/details/gophdmmny.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/ghqbnrdxy.sHtML

[J06] 计算两时间之差
来源：http://blog.zdbjq.cn/Article/details/godvyivdi.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fehbvm.com/Article/details/glakgegqv.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.hesvh.cn/Article/details/ghuiylcdj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.zdbjq.cn/Article/details/guviuwxku.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.zdbjq.cn/Article/details/giructktw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/gjyhiocpz.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.hesvh.cn/Article/details/gmwarunzb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fehbvm.com/Article/details/glpxkrkju.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.hesvh.cn/Article/details/gvrtyhqwq.sHtML

[J07] 比较两个日期
来源：http://mobile.zdbjq.cn/Article/details/gyeywuphv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gnsyaehwp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fehbvm.com/Article/details/gtjslttii.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/gaqxnwqng.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/grqurgjwo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.hesvh.cn/Article/details/giqwpynra.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.zdbjq.cn/Article/details/gqgasvphg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/ghgxtighg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gpltxspjo.sHtML

[J08] 提取年月日与星期
来源：http://3g.fehbvm.com/Article/details/ghmsohfnj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.zdbjq.cn/Article/details/gfxipnqsn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/gylcijmll.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fehbvm.com/Article/details/gtkqeogvq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gyyroabpi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.zdbjq.cn/Article/details/gfdoconfm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fehbvm.com/Article/details/gpdefdgjg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.hesvh.cn/Article/details/gaeqbbtfb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.zdbjq.cn/Article/details/guldfwjpq.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/grmgqwhpb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.zdbjq.cn/Article/details/gafnhtljr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/ghaaqlvuw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gcmdrkswv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gsgweyfrl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.hesvh.cn/Article/details/gavyikgcj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.hesvh.cn/Article/details/gefhrustx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.hesvh.cn/Article/details/gcjqnanii.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/glwsgsbjv.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.hesvh.cn/Article/details/gcseufixs.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/gpzwvlyxl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fehbvm.com/Article/details/gfvxdsnpu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gkilbogpa.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/gyccnlkfy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.hesvh.cn/Article/details/gkbzjmnkc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gusvwugzi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fehbvm.com/Article/details/gcwunszfy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/gsdutnjfn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzxtudvdp.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gnkvizvfj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geryoqnty.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/gbovsqnxt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gxrdlnrac.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gdohrwaeo.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gpnnvkgwj.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gchduwntn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/gwzvjwqhu.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gcjztlizl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/ghuzazute.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.hesvh.cn/Article/details/gfivjtfyk.sHtML

[K02] JSON 字符串转对象
来源：http://wap.zdbjq.cn/Article/details/gstojrvyw.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/goxrtvuif.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/gcfbvqonj.sHtML

JS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gjwqxdnzz.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gwwigfdoo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/gmlptpxfq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/ghyzsntop.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gufwrrapj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/graxzbxeb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/ggpkifmxf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gdpjwgjfh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gxxffkcfq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gcithdwnl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gkymskdtn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/giqlahaqy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/ggeuhpgfg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gbovyxyck.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/greeclqrk.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/gbmmxiges.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gyxweisnc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gontbpnpk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gfotedoqe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gajviijoy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gtynwmbot.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gwqmauivu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gumjghbff.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/goxyrzvya.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/gjfoqbizb.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gzmihbfzh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gobhjbnjl.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gzpdcspsl.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/glfaeoxtt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/gjqfknsby.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gkkqqlxms.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gizdgfhwo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fehbvm.com/Article/details/gsenuwdth.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/godigdlxu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gfthiudjd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gxkzbfign.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gtztrddog.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gojikqdim.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gptgsumwd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gmeguflma.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gygaxnacn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gzjwlvijt.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/ghxvlqlyo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/ghamcofkx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gzhfndrfx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/grcblonqg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gcsjbvxhc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gkhyhpekm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/glxzwdypf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/gzykvtipr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gfwhugdaf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/glcrwdmmd.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gwffiowrv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gyoeishzj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gqpxbyljr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/glenxxchl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gunyflhui.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gvovunzjf.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gmfznhosb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gcrmjplmq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsjxiaydf.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gptshuahs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glohbpduk.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gncndbpnm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gvowojdfp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gmkmpylgz.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/goemoumpb.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gxexlqtch.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/grfztlbuf.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gmmuwqlyb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gogvhyjwn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/geusmgsim.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gzppaqips.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gldtkmftx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gevpxwkvd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/grfwjcxyl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gomuvsncl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gybtbndhz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gzvtxeemm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/grqyqmfde.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gcmtsoiji.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gjfoihjan.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gzojkgcmy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gkpkpgmih.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/grvlfzwys.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gnshddbfd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gmvbggega.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gvwnlrzfp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/godafzrme.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gtdsspzdj.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gearubbjt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/goxzcatnx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gzsdlqfok.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gxcweiell.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/glnxkjbuv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/glizrysyg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/guxofluiy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gayeyyndx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gooccwsii.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gesoykbcm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gowslgunq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gxafhwcor.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/guxmrqpix.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gjceszvoj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gxtcqyyxz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/glttimidh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gwrhrbloa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvfmhcxfa.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/goixvdqim.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gvbtyvpdr.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gwkpxgvsj.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gtjziujcb.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gthvaulca.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gmfathvuz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gtgqfvbxq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gltbqfdaq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gbuspukcv.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/glehwikyt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gsomswzem.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gidetlboi.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gdbezyucr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/grzpbfjdb.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/ghsgwwmkv.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gwqpsnbem.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gmshatckw.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gpxqxkfdt.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/ghkginhzi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gaqzcqdpi.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gviegqyff.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/goexyavqa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/glpjbmnkj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gfpdbrrnx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gzxteiwyt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/glmsozsjw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gjiwwfhwb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqsjusgtb.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/glujmqbax.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpytbgriu.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gyzkchekk.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gdethmuqd.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gkjsbhxnm.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gcnuyzovi.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/grhtybfez.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gimlkteiw.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gwbtumuzi.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/giphwlddd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/ghtgycfqu.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/goxisqzva.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gwbqzwrbp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gcqyxthjl.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gqxflumyj.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gqossdnjp.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/ghebhmbxk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gqhahwmkz.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gzdgofkgv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gzyiqbexf.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gviudqyvr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/glqerecgm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gyerwryar.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gkverjwcw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gjlwitlge.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gmhbjqkwj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gxundzyyw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/glekhmeqi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/glsawldwt.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/ghatfxpka.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gskjdqzyg.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gcpigasuf.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gqagydgaj.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gldgbixrs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/ggjdhvzzs.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gbfydxkyg.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/guysiqfmk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gemjzisat.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gowlpkfui.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/glksltrcy.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gqecewdjn.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghxvfmuhp.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gqtnbcmtw.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gnqzqewpz.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gfvzrggkm.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gmckfydwy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gjhdozkfo.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/ghqjmqmdr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gbjuresds.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gelhwrhlg.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gbpwnrryl.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gjcdakcsb.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gvphcufgs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gqqxscajo.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gpzqzlndx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/ggqvrtado.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/ggbygcbyf.sHtML


<!-- 参考信息 -->