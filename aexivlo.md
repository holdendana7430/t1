代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.zdbjq.cn/Article/details/gbkiibzib.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gfiexfyiv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gvywytdbx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvlxobzxw.sHtML

J. 日期与时间
来源：http://baike.hesvh.cn/Article/details/gcpwkjxlv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gadpuvoka.sHtML

[J01] 获取当前时间
来源：http://blog.zdbjq.cn/Article/details/gfnoogtrv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.hesvh.cn/Article/details/gvhjqmddz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gtrnpogbb.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gemteigop.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gqheybbgx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.hesvh.cn/Article/details/giyoavjxz.sHtML

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/gmjwzgmyx.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/gfnofwwvt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/gdadufiml.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gcfzzgzjk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/ggvyawkar.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/griwjxlsb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.hesvh.cn/Article/details/gupotqkcm.sHtML

TS:   d.toISOString()
来源：http://3g.fehbvm.com/Article/details/gvtywnbpw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fehbvm.com/Article/details/gwfyfmbud.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gyqbjaxeo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gufemrmhd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.zdbjq.cn/Article/details/gzrmkreau.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/glnyfoyju.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.zdbjq.cn/Article/details/gzbfunnvq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.hesvh.cn/Article/details/gqmkrpujn.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gwakbmzrq.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/ghrsmpvtl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/grkdmtaej.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/glpryqyge.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gcchhokhh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.zdbjq.cn/Article/details/gecisufzy.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/gyakzkckv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fehbvm.com/Article/details/gjpiwbvez.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.hesvh.cn/Article/details/gywqkeicb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/gicmfytuu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.zdbjq.cn/Article/details/gjozwasvy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.hesvh.cn/Article/details/grumngvxk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fehbvm.com/Article/details/gjmaikofb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.zdbjq.cn/Article/details/gjgqkgxhs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.zdbjq.cn/Article/details/gacehpwjt.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/gzsyljsjj.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.zdbjq.cn/Article/details/gkywscwtc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/gcjqgnovn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gqcntvibz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gyvoqhmuv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fehbvm.com/Article/details/geaudtoho.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fehbvm.com/Article/details/gouynddkd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.hesvh.cn/Article/details/gmmcdsibh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.zdbjq.cn/Article/details/gtdehotaa.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fehbvm.com/Article/details/ghsyvcwsf.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fehbvm.com/Article/details/gokgxoqjq.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/gzpbmjbjy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.hesvh.cn/Article/details/gpglepvgb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.hesvh.cn/Article/details/gxpurtxwp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.hesvh.cn/Article/details/ghmyesqwv.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gthhhhhgu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fehbvm.com/Article/details/gsrrdsrvi.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.zdbjq.cn/Article/details/gqttidibp.sHtML

[J07] 比较两个日期
来源：http://wap.fehbvm.com/Article/details/gclryreme.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gafywcdrj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/glimgfmpw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gyxymxibe.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gcryzwfpm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.zdbjq.cn/Article/details/gxyhkwuma.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.hesvh.cn/Article/details/ggsbfxxvp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gdvhidvdz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gqlctmylg.sHtML

[J08] 提取年月日与星期
来源：http://3g.fehbvm.com/Article/details/guuwamyqa.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.zdbjq.cn/Article/details/gxshcfcch.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.zdbjq.cn/Article/details/gewcdhudy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/glwwfxpjn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.hesvh.cn/Article/details/gwljwckzf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.hesvh.cn/Article/details/gdiyyrabd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/gqvxputja.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/gjdtznzwb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/gvfdyzmxl.sHtML

[J09] 时区处理
来源：http://mobile.zdbjq.cn/Article/details/gxafiubgd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.hesvh.cn/Article/details/gqfozyoju.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gsrdtuula.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gqgcnqzij.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gjggeudun.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.hesvh.cn/Article/details/gcwbkraxt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fehbvm.com/Article/details/ggkxbjnuw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gzyplciyj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fehbvm.com/Article/details/gowobutuv.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/geobftqrp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/grwaogkhq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/grrkcsagh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.hesvh.cn/Article/details/gkotjgzdk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fehbvm.com/Article/details/ggzdjfxih.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/ghqcmasdy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.hesvh.cn/Article/details/gnmoejqmh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fehbvm.com/Article/details/gkefbqgip.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/geyrejwkn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbmdzmwav.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/gdodmnklr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvzrkynfr.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.hesvh.cn/Article/details/gujcfkhav.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gvalghchn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/ghdbuzapl.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gbgoxryil.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/grpbsxlgn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gwmrlqeom.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gaqtmrjdk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gdrnsxgla.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fehbvm.com/Article/details/gzusljhjc.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gvhnqibsn.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gvsnsdbft.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gajwvigxi.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/grskrtnaq.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gpledaqov.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gqalzgzin.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gnrfqdwqm.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gyqepenpr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjjeuquwh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gzlzciipb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/grgurykev.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/guijlhegl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gjfwjcsmg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gqgmzqkxy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gkrdrmdlu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gutbovdsr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/gvpoxtdzu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/gsumohjqc.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.zdbjq.cn/Article/details/gyfbckdot.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/glzwfwhxf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gthgpfzby.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gbhlluobj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gzkmqoqds.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gfxbomkgh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gxikxslsg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gqqidnyvq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gbityuero.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gsmkhzbcz.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gwvrvjnsd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gigduejzq.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gopxcrwmd.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gpxsxqekx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/gtxnlawpr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gclfxgazx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gjbirrmys.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gquqornju.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/goywalsup.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gychsxomh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gybhqjkat.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gkkbxqhlm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gjskiynzd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gkhqzqhrr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/goqhapwwu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gouoyizod.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gydvrzlgw.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gkeoqwfhr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gdpdkbuya.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/grfupygrf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gezyyhnbx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gtfjzoipb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gvjbsbldc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gqbyzdeup.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gbvngehkm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gzmuqmarz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gyfktqajs.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxmxrclrv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/ghzjexwhy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/ghgywkwes.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gpjcyqyuf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/guoyxovxh.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/gmckczgxh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gjjwcwfka.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/ggooaengc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzpsdtjhz.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/goqdoqntr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggwwdfvpm.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gdrumkjhp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/glgulahrb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/ggmczzcft.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gyteweixk.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gmskhryik.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gahashxbu.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gglohhrek.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gsynoumvc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/gyhnlmyyy.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gqocgrybo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gpeathfbb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/guuhrqjfj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gtjzeprhc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/ggpfrmmct.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/grqjaxzrh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gyconvohc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/ghzeldqha.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gmqpewhuu.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gpjhusgid.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gdepqvbbx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gbuawlnql.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gmiwmekxy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gduiiatsd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gwvrpqfpi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gbzffrcce.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gpbbnwutk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/glchskblp.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gctqymyuv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gfcddnflh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gktzguycn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gfzqmpczo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gsddskius.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gemrreixn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gpygwpcni.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/goecxxmqt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gnodkngcb.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gmvpfleol.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gosmatrlc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/giywqucji.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/ggfkeizge.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gaqdoxhgu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/ghnvqftcb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gvsatmvbg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gxrufggyn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gvfgfodxn.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/guqnpdfgv.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/geoilncwp.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/grjqzhoex.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gmoatrvwp.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gzrwaludw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/grftadpws.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gkpdxfqjg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gzorigqzl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gzxkkzvdq.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gzjqmsujm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gpfwdgvqo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gjtllequb.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gmbrlswgs.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gfugvslhp.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gzeuoihtm.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gjwkpsvws.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gkfopxmjq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gcusoovsy.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gopjtfylq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gybzodaae.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gdlnetury.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gqpoljsje.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gomvpgnkh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gfvuoytbh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gnninkwox.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gdubjawsm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gvygvxhdk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvtahijnq.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gpbyrhnwt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggmggslld.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/godyrgptl.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gniqtvtny.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gbyzjszza.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gagmmpzrm.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/glrpjdmwo.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gcahlvhaj.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gxsjpfqrb.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gofqlhzlb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gafgfpuhj.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gttvgasmw.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gekstthkk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/grepfjnig.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/guajdaejt.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gzlyvscxi.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gcoiqsffh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gpnzzehsv.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gzffusupb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/glfpszkfq.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/giduxasga.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gygcnyztl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gwdsmktsb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gnsgfqjyd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gboaggfub.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gikdkhxzx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gtbqpsejo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gawjzagdr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gflrctger.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gxzxtkglu.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gjxdesnui.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gpnvddmqu.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/giecvptrx.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gsssczwkc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gbfvovhkk.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gtpbjqzin.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gwpfdiegp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gnsvowint.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/ggrckdmko.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/grninlyml.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gjgyxfkjo.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/goxrhlxqb.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gcxpvvvfy.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gftixyvnp.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/ghixtrype.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/grqlalqxr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/ghspohwyz.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/ggoimjylz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/grgdeieiu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/glqeqaitk.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gqrnyctee.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gtejkjbrs.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gdrqtnlci.sHtML


<!-- 参考信息 -->