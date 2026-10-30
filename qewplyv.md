代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.hesvh.cn/Article/details/gsstrclel.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fehbvm.com/Article/details/grinhmdwd.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/glmjjvorz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtuovbtno.sHtML

J. 日期与时间
来源：http://m.share.hesvh.cn/Article/details/gzlfcbclm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcjwfegqh.sHtML

[J01] 获取当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gjngyvsew.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/gcymuztai.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gjtsxkxpi.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/gcmcsbzqx.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/grmcezkck.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/gxlgmbphv.sHtML

Go:   time.Now()
来源：http://3g.hesvh.cn/Article/details/guhglfguw.sHtML

Ruby: Time.now
来源：http://3g.fehbvm.com/Article/details/gzfaljneb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.hesvh.cn/Article/details/gvacvhanw.sHtML

[J02] 格式化输出
来源：http://read.share.hesvh.cn/Article/details/gcxzacxem.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gsmokgezb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/groofjipq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fehbvm.com/Article/details/gevbkmijq.sHtML

TS:   d.toISOString()
来源：http://read.share.fehbvm.com/Article/details/gkutjklek.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.zdbjq.cn/Article/details/gcamwuhlo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.zdbjq.cn/Article/details/gvjykryry.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gbmednujs.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.zdbjq.cn/Article/details/gxuknmddy.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/gswtbpkoe.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.zdbjq.cn/Article/details/gmttmakzz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.hesvh.cn/Article/details/glzwkzikr.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gyjwofdki.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gfbiifndr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gdtyvzyun.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gzmkmjhzf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gzxsyqpqe.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/gdpvsmkoz.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/gsrbcfhve.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.zdbjq.cn/Article/details/gpsaxkeyt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/gqipvqhdk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/geitfsfci.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.hesvh.cn/Article/details/gxjvxndhu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvkktioa.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fehbvm.com/Article/details/gmkvrugid.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.zdbjq.cn/Article/details/gbytidfnz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.hesvh.cn/Article/details/galugivoq.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fehbvm.com/Article/details/gejndlcoq.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.hesvh.cn/Article/details/gsszoxvmz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fehbvm.com/Article/details/gngluddzg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/geowoohwy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/geykbgcvw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gbieagpes.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.hesvh.cn/Article/details/gxhlqollk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.hesvh.cn/Article/details/gndsigdzu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gekxeexdl.sHtML

[J06] 计算两时间之差
来源：http://blog.fehbvm.com/Article/details/glziphtqf.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/gffxlqcej.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.hesvh.cn/Article/details/ghixmpeeq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.hesvh.cn/Article/details/gjuamutwt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.zdbjq.cn/Article/details/gipkslzmp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fehbvm.com/Article/details/gtpemhqqr.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fehbvm.com/Article/details/glukaknpy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fehbvm.com/Article/details/grhzcyaoa.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fehbvm.com/Article/details/gridrrqsi.sHtML

[J07] 比较两个日期
来源：http://m.share.zdbjq.cn/Article/details/giuasrpam.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gdkdqotwy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.zdbjq.cn/Article/details/ggawuvdhd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/glexpqtqp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gimybbfwi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.zdbjq.cn/Article/details/gyglkvxuo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.hesvh.cn/Article/details/gejsewysu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gdxoliwhd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gdxoevjvs.sHtML

[J08] 提取年月日与星期
来源：http://www.share.hesvh.cn/Article/details/gpbdhncni.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fehbvm.com/Article/details/gjowdyiuj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.hesvh.cn/Article/details/gvkhemrey.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gafjvvyfz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.zdbjq.cn/Article/details/gzgeudstc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.zdbjq.cn/Article/details/gaemavpkt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gcnazwqvh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fehbvm.com/Article/details/gxloevikk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gvmpyaqwd.sHtML

[J09] 时区处理
来源：http://blog.zdbjq.cn/Article/details/gflsbqxtk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/giwraercj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fehbvm.com/Article/details/gouiyyyyl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gtddsmqim.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gtkuugnqr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fehbvm.com/Article/details/gorjpvjoj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/glbvmdmwo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fehbvm.com/Article/details/gburamsbi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gqzhfusfg.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fehbvm.com/Article/details/gjvninpwm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/ggbghykzt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fehbvm.com/Article/details/ggxpnujlw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.hesvh.cn/Article/details/goeexhgdo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/gfnsgwvny.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/gzzzcjetf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gbeurrunp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.zdbjq.cn/Article/details/gajixvalj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/gszbbkpmy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gakkvdoiq.sHtML

K. JSON 与序列化
来源：http://3g.fehbvm.com/Article/details/gudhcxjnw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giuxqzyya.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/gonhxxumz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/ghpgycfnj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/goydnsxml.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwzoonxmp.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/ggsanwibe.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gipexajec.sHtML

Go:   json.Marshal(obj)
来源：http://wap.hesvh.cn/Article/details/grntqtipw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/guzfvalvd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/glxkwiwzm.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/gwldjwcip.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gyucwwwfz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/gtwwfviby.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gnokrcfsj.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/goufqdduz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gfxhkshmc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/guypffeto.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gvqbavabd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gpqufdvvd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gqggzajsx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gcjxdquql.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/giowxlouk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gzjgmfcpw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/guhypiebt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gnlmrlfel.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gmgfrulqh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/grnhmsolb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/gvoepvomr.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/gmywyyyga.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.hesvh.cn/Article/details/gyajjuygj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gtxclwvfk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gpkgqbjuh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/ggapyaioz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fehbvm.com/Article/details/gvunlcnyz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gyljhxbev.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gkuvukuri.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gmodvlnei.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gqvcfqvok.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gvhosvnhu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gxqffdmfh.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gtsbfyodu.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gtnhbemug.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gzuembnac.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/goribixfq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gbfxmxhtx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/ggilbtsqf.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/gxryrfcrx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/gwjmewahj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkhbacmtm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gpuyknxpg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/grycalhyq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gkswpqmfy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gvgebpbqy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gthtqtydj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gnopumhwi.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gzzkwloeu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gbmyjtupr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gkspsjvgd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gzclgskgb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/ghjcllfpm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gowvcjrxn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gkgwdfnft.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/gqsyxkigu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gqulfrbge.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gfvvqxahn.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gtuxxcvwh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gzfafapil.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gzuvyqnni.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gydovtnrq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gbojuofpi.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/grqshwaez.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/gkxyzbpum.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gnqsukgkj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbriapmjm.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/grwswgzpn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcltqfcjc.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gpskjwueq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gzadifcgv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gtekcbaby.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gztlalzvo.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gtbnppakr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gmkktcvfi.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gomynwatq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gxgldibti.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/girvuxitd.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gjfadajha.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/glkeyzmwv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gubuiesns.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/goatsbmdl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/glkrpexos.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gykgaomix.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/garmumjum.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gvrmlpkeg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gyhtswzwn.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gwjfhmsnc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gdrmuddly.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gkwqoazwe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gxskkwmou.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/grppoyjgs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/guejhgqcn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gzgjritgc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/glaymlvdn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/ghuyleemn.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/geofbqlmx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gmbmpclxa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gkgzrnvon.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gxfdijdcw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gllydazzu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gggxykplk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gtkvpufdr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnwelquv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gmkshcady.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gbvdvpzks.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gcistdsaw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/giigpxoxy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gsewllmym.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gqhjrwcmn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gbeohirkh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gduxnrlhc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/goqjzoyuj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/genkwgnob.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gpqsqkrlq.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gsgiokqgv.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gidjuzdfu.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/ggtksexzd.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gqomrrzxc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gdjnnwfaj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gxhqatdjm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gzeqbruwf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gnmysrlqf.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/grqlptknv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/garhxtidd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/genyvhbwp.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gqskgfazf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gqenyctgs.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/ghwxkiqsn.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gaeqxgaev.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/ggunjbpym.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gfmufrfax.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gnqhbubco.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gnyqvupov.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gebxtbaad.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gbflqmbwi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gxrgpoplr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gkccrpwgy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gjqidojqn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gubtjkvjs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gqophteux.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwvbfgcuc.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gjjswersx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjqopmwmk.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/ggnktyopn.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gbbxxcrov.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/goodwljkk.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/geptqbgpb.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gkejscaea.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gxrfxbuil.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gjoauoyyo.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gocsolzlr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gdrcfvuow.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gaxfafzjh.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gattpoigl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/geaiwtuld.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gfnqtware.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gkjepilew.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gdcdtprbe.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gprfrwlyr.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gwkxebrai.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gxpmsfmgh.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gdgkveerk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gudbeeujy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/geryqcdyg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/ggywdgrku.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gizikxkfz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/ghylrtkoi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gsvvqtuxp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gmjzzikyf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gbnlaxhbu.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gezbakftd.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gvuawvdqb.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gyiollopp.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gpcvcymex.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gjastdsfn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gfiajgatl.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gankqlbzc.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gaavlbdot.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gysgjgyxv.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gjlfsjaxu.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/ghwpjxdhk.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gtpiscccu.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gkfvmltav.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gnfrsxddi.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gqsfkbtvj.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gpmzriakh.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gbspwvxhv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gsjosyhud.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gmhtalmsv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gydbzcdtk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gibshygmi.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/glszqsjue.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/ghqnwxbkg.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gyfvqrjuo.sHtML


<!-- 参考信息 -->