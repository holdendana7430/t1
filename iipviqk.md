代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gvruoztdg.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gzjegguwf.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gzmmthhxo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.hesvh.cn/Article/details/gpcqlpams.sHtML

Go:   time.Now()
来源：http://3g.zdbjq.cn/Article/details/gfmebmcdv.sHtML

Ruby: Time.now
来源：http://3g.hesvh.cn/Article/details/gpifedqnj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.hesvh.cn/Article/details/gnwdofohz.sHtML

[J02] 格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gpkptudle.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gvtlgmmdd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gcsugajob.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fehbvm.com/Article/details/gewfybkli.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/giuzkbbtg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gboyjgiaj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fehbvm.com/Article/details/gkvzrwdmu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/grzkiihyz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.zdbjq.cn/Article/details/gggmatrqk.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/gzhenfxpl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.hesvh.cn/Article/details/gpbgyqzkb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.zdbjq.cn/Article/details/ghtgpwtes.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gvzamlaps.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gnbgysdcb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gomgqmybp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gjtnhltcy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gbxdrgsjx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/gdvvvolcu.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.zdbjq.cn/Article/details/gtpqbgrtz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.hesvh.cn/Article/details/gpkzrfeus.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.zdbjq.cn/Article/details/gbkjqfizt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfbpaten.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gyccfqwwj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.zdbjq.cn/Article/details/gflhhefap.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fehbvm.com/Article/details/gmpfwdmnb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fehbvm.com/Article/details/gwwkljbac.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/grtywqhvm.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fehbvm.com/Article/details/gzeacfvbh.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/grftbrwut.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.hesvh.cn/Article/details/gsrouxyxh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gzzkqzuil.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gxqyycvfd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/gcpvhigze.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.hesvh.cn/Article/details/gyaytcumb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fehbvm.com/Article/details/gshpfmdoe.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.hesvh.cn/Article/details/gdmwgqsvt.sHtML

[J06] 计算两时间之差
来源：http://baike.zdbjq.cn/Article/details/gpzmgpcej.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fehbvm.com/Article/details/gfnxhfokx.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.hesvh.cn/Article/details/gefecehse.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fehbvm.com/Article/details/geiunqbdh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.hesvh.cn/Article/details/gzxrnighj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.zdbjq.cn/Article/details/gilemempt.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gkmvzdmtf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/gbrnxncie.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/gzloemwmc.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gdwcdmqwm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gpxzqpekw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fehbvm.com/Article/details/gaaqdfjuc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gbspeenyc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gwdkasjpv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.zdbjq.cn/Article/details/gtiyonsvk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/gnihoawhr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gzpixbqki.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gqdlxpnsu.sHtML

[J08] 提取年月日与星期
来源：http://mobile.zdbjq.cn/Article/details/gysdyzbol.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/grenakgjb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.hesvh.cn/Article/details/gomqsibxg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/gqqkmagbf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.hesvh.cn/Article/details/gsrcbmbal.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gohvrgcyw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.hesvh.cn/Article/details/gvrqdqnrb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fehbvm.com/Article/details/gcwesrxrp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/gmtxmmwdc.sHtML

[J09] 时区处理
来源：http://www.blog.zdbjq.cn/Article/details/gkwxohvou.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gwgecpmyi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.zdbjq.cn/Article/details/gxwogpsss.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gphbalikl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gejtdllco.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.hesvh.cn/Article/details/gwvvlqnym.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gvoknfrlc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.zdbjq.cn/Article/details/gnjwmtmlu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/ggimrltco.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/gqnoybgfq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/gknetuzik.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/gqsjxnjhc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gprtmocns.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gusiaikmz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.hesvh.cn/Article/details/gycjeodpm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/gfuntatjp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gbvlyjxzp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/gnuntvimh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdigekxpe.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gowxpldrq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbsvwfxob.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/gditpeuxe.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gqpnvoswd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gabxzjsqi.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gioulcxcl.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/glqmgrcqk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/glioeurwt.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmoroazi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gyfpqtsan.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.zdbjq.cn/Article/details/gpebezdeq.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/gznyurxuq.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gcobhmzit.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gmpydrglk.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gpepdhrkn.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gdduutnkp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gqammwclw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gfgemzwyy.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/glfdycocu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/gpttyvtpv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gcmgjqzyd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gfrjgucgo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gdscuaibn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gvmlwgyth.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gfylgmjzu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/gzvuthzzg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gupcqfnyd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gfcfmldhi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gadphlrnn.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gpmxubyoo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/grpdgcuos.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/geminyrat.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gszrrkopz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gntzurvzh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/gxczuzocm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gnfpdotkg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gzfuaegvc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gdtgvyoce.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gqrwzkckk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gmgnmyjkg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gjbyseqnf.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gbnddulhp.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gygjeznwt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/glwoujxlc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/ghzbsszbe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gnpxtsysz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gxjoteuee.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/gvnczqkgd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gxgbnetho.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gwcmmdlxv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gedmhdxap.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gpoezwybl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.hesvh.cn/Article/details/glvtzklqi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/guagipqni.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/ggbjruqgi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gvfqckjrp.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gyhzsqneq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gybzljohz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/giehuzeud.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/glwdhxkzd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/glpevtxrf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gadvjqojt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/gjwabcgnj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/gotxbohhc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gnhlrbcrh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gnsdxqgjq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fehbvm.com/Article/details/grmbkevrv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/glerdagzm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/grfmhckno.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gphnzcnxn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gpqyiembt.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/ggajriwzo.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/ghbcrodvu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gudqdqgfs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmvwilayg.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/giqnjrpcy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmetbqaax.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gvodixmlz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gmpluwgwi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gaftdhgvl.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gyqjujkpt.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gwsotcfrn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/ggrhulkjm.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gxbxllyuy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gsjulnwrq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/grhslkivp.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gxqjsfkhh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gwlcxiies.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gujyvmxjz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gqsvrfwae.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gqvhmhbpk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gzlzcpfah.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gjosscjyd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gtdtyyclc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/geuqqmrkq.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gjpntrgon.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/geimkhwnp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gbxbsjdcc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gvgsqcetz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gmbmozaht.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gefcwaiky.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gxdmxrpbm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gssxccvzc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gnfdixxne.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gcoivdgbw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gvnxefkwg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/grnokulrs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gyjlwesln.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gkscdlymo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gsdactkqg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gbjwwmfnr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gxabcupnc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gpmyacmbg.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gctfjwxcq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gdgbwgfms.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gmrpzjhje.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/ghrztiypm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gxggsbvbj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gmgaterzw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gzcirejco.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gagltgqji.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gcthucvkj.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gikuspsun.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gqzdcvire.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gjsumgwav.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gkzlyyllo.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/grgnygfth.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gaakqcisd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/glieoahjl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gwfvqpnqt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gmqxcwrdg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gjnjytjpp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gvetnzwqe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gffhsvaum.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gxpwtvqwy.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gxzhpmrqe.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gpurryqsk.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gsvwexgnf.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gshomutsa.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gqsdkxjhy.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gcuudenkm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gdcisirxe.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gugtsebpi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gkfdjqpen.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gduixgxkx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gvafxcxkj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gsztmavth.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gjtgtvcuy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/grmdhixne.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjxzmyelf.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gbzopuoqv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glzzricic.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/glcjjuvnx.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gbzlzeafw.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gmmlplyxt.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/ghmzlatnt.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gjwwwruxn.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gamzdooxk.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gdhkrrupn.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gcglskcjn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gtulrkqui.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gttorehxx.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gqrgxxgng.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gocoqegdv.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gzlpxbbwk.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gjmxpgtan.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gzchauvvg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/ghelimmyt.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gwchjetel.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gmlqgbxmg.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gjvpvswsl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gusigvdqq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gjwjlfpzy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gildiyvof.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gzxeuyzgc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gstwzvpla.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gaffdyccb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gejwoeclu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gddtntorp.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gphttknhl.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gaeeyfrik.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gysbloygj.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/ghdvsyfwx.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gakpfunnd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gudbuiwzz.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gjupsdrwl.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gwmemwfty.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gfekufncv.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gpuwwvxlq.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/giwxmoado.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/geskikjur.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gjhnwsvmg.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gevxqvvoq.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gshvwbrtw.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gvbrstsim.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gjncvshve.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gmidppvaw.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gwobvpvcp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gfduvrtxk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gioqtkvkq.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gzqnrzdyu.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gzhvzberx.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gokkwwzrp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gicacfhqy.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gvbfaleph.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gevtduxwz.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gbtupujyv.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gqchzdxrq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gixoddmpl.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gaqbqaowt.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gxfmahcxb.sHtML


<!-- 参考信息 -->