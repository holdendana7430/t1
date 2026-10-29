代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gwsskbfet.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gbvniiwxf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/gkojtsjlt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/gjwlosukt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/ghtiedkmo.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.hesvh.cn/Article/details/gafdhmtmq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gvsmrscfi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gqduqtblx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/gfxiyrqpk.sHtML

TS:   /error/gim
来源：http://3g.hesvh.cn/Article/details/gmnpsnuqw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/gssrgoojq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.hesvh.cn/Article/details/grlytxuxf.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/gzqlggvnv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.hesvh.cn/Article/details/gbhuaboxe.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.zdbjq.cn/Article/details/gzbvknuny.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fehbvm.com/Article/details/gubtrmxix.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/ghceozuge.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gqwhaedvm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gffngyjnu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gimdpjxcc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.zdbjq.cn/Article/details/gxccumjdr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.zdbjq.cn/Article/details/grcvjlawz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/geegsdjkc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glhfqzlih.sHtML

J. 日期与时间
来源：http://read.share.zdbjq.cn/Article/details/gpfzwbboa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gucfvmhcp.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/ggwgqcpfx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.zdbjq.cn/Article/details/gwtoxobuy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gexsvipgi.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gultaxadu.sHtML

TS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gzcjwhzgd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/guectttwg.sHtML

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/gzthijpxe.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/gakrbtyfi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.zdbjq.cn/Article/details/gqngrlbfm.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/gdmsdpfht.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gcjzvmwnk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gfoeordfb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.hesvh.cn/Article/details/gvpcyygwq.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gvzumzrxh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.hesvh.cn/Article/details/gywlrdplf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.hesvh.cn/Article/details/gotascwws.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gumulelgb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.hesvh.cn/Article/details/gsnxosvfj.sHtML

[J03] 字符串解析为日期
来源：http://www.share.hesvh.cn/Article/details/gavxfecei.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.zdbjq.cn/Article/details/gmtaijbic.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fehbvm.com/Article/details/gxvfashyx.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gteybbnhb.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gxdtkfcsz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/glroucggx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gjkmgnmgb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gaxrqwqrk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.hesvh.cn/Article/details/gabkmtwgw.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/gkucblrhw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gcsikvjxq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/ghajbkrnx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/gdyejcifw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fehbvm.com/Article/details/gsjkfyctm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fehbvm.com/Article/details/glvhyiuzp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fehbvm.com/Article/details/gwnffwhul.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.zdbjq.cn/Article/details/goczjpgvm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.zdbjq.cn/Article/details/gmzibweil.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.zdbjq.cn/Article/details/gprbycqkv.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.zdbjq.cn/Article/details/gxijhazih.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fehbvm.com/Article/details/gnmkbatzu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gmjqodtpu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gdxvtwauf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fehbvm.com/Article/details/gicwvgrbj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.zdbjq.cn/Article/details/gbvcznagb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fehbvm.com/Article/details/gfkoioiwm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fehbvm.com/Article/details/garbyvuud.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fehbvm.com/Article/details/gcrmgnayf.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/gynkxfgfy.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gmtaaxsju.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fehbvm.com/Article/details/gxjfmtdmt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.hesvh.cn/Article/details/gxpvzgnyi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fehbvm.com/Article/details/gjwpyuzvr.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.hesvh.cn/Article/details/gepvawqbt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/gzftpquwl.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fehbvm.com/Article/details/gpggcmbsn.sHtML

[J07] 比较两个日期
来源：http://mobile.hesvh.cn/Article/details/gqcrdrveu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/geuqikvbf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.zdbjq.cn/Article/details/gbprxlwze.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/goufnptgd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gwvnnfthq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.zdbjq.cn/Article/details/gdweixpay.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/gvargfdcq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gmoulvozl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gpwjkvjgv.sHtML

[J08] 提取年月日与星期
来源：http://read.share.hesvh.cn/Article/details/gygvzjgzn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.hesvh.cn/Article/details/gwgprhppw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fehbvm.com/Article/details/geivujsef.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fehbvm.com/Article/details/ggzmkfoth.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.hesvh.cn/Article/details/ggzuwvunt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.zdbjq.cn/Article/details/gfofefryy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.zdbjq.cn/Article/details/gryvkehzn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gkgyfhxif.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/gdowuxbqn.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/gkrmchacn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/ghabcicpt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gvvxrxhra.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/ggulgrmto.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gfcufwjpl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.zdbjq.cn/Article/details/gmweoyykj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gfrweaezh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gywcenrli.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.hesvh.cn/Article/details/gzklmgtig.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/ghcinvwyq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/gadziehdh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fehbvm.com/Article/details/gzhzwghtg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.hesvh.cn/Article/details/gryozeufi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/gcqgckoam.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmnkwiugs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.hesvh.cn/Article/details/groupapyx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gjmkceppb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/ggizuqzxc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggonlbsoz.sHtML

K. JSON 与序列化
来源：http://read.share.zdbjq.cn/Article/details/geulttajg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gghoihyer.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.hesvh.cn/Article/details/gzwidqcpn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/grritbbtt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gmzzprobr.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gudrwgaci.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gwuqtnasv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gsxvxpopw.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/gzdpakfit.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gntsxsdec.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gcwedzunf.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.zdbjq.cn/Article/details/gaicuefol.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/gejrcnwrd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fehbvm.com/Article/details/ghxeogjjk.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gcctiuzml.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gqpqxvduv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gzekieoyx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gzmhimjjz.sHtML

Ruby: JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/guydmskks.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/gxrkfwpqg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gcpbedyoo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gyjubaotj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gradtcutr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gqzrbqpxj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gsjilljfz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.zdbjq.cn/Article/details/griwucqjf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/gelvvmvdh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/gvqqugysm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/grxqxoapr.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/gsiqbrrya.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gclsnvleb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/gsjwdugso.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gukjeirhx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gbnpxiqef.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gxjxzxhif.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gpeowzpyh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/ggefygbov.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gdyesmmoj.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gqhcfmdcs.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/ghkevigdj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/gvexzchqg.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/ghgpzwjgy.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gqmpsvwpr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/grjncgfwd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gjxuzfcsv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gonamufzn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/gynmdojfc.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gvokjzvtt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/goqiwgdbm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gqbxwgqnd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gfxlexdhz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gfkjrwkci.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/gpibnhhfr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/ghjkawbbz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gencqyvyv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gxmwowset.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gkunycixl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gwqijxcml.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gsvjpqmbl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gzwlymvkj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gairvktir.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gvklmtxzs.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gtqwzkdox.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/ggxpelfxq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gdzsynpqg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gytytmies.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfouwzin.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gihdxvohq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/guofqppux.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gevttauud.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gleigdhzv.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gyqeucpbo.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gllnpebpn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gcvhtthxq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbrgyqrek.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/gxuigyuoa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaxosbeir.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gtileaytp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gfliyslzm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gpdbdsibo.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gcbnuxlep.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gankauseb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gwfnsklbz.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gqjxijayn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gvlfkdrhr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/garzzafup.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gjdvvskxe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gqppzdiuw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gwwkacylu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/ghreswgpt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gafkvmeif.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gmdlxebpt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/ggvtbposu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gbgyslmaw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gmfqumpwq.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gqgdnyyhq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gzwrcacmg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gmkuxollp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gyuwlzfyk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/ggysobphn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gwrztsjgd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gjwcbpegu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gmnglgopg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gvqwebwig.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gebnrpfwv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/giqesbyfo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gcscmsjth.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gsyxcobog.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/ghehxazlf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gqjautimq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gdmbgrluq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gwuzobvre.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/grtxihniq.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gqvbrsvqi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gyihkhxdf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gmvcxxnvg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/ghixslwjf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gefjrtavu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/ghexpxeij.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/ghixjikmg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/glxecwjev.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwmzunxte.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gagbygszt.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/ggpzjqddg.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gmdkbfsee.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gkzjsmgje.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gyizkxlii.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/grsonscds.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gcyvoomfi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gbddwcbfc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gjxwmjlqz.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gpihplakf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gdxzewbzg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/guioivbep.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gufmbgscx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gyrqwqyyc.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gzaavwxba.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gybfdjstw.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gpjxuhvjq.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gjoecxfwe.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gejaxcpca.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gabylhpms.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/guehxctfm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/grnstdjwe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gdqcsbjnt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gqmozvtjb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/ggbcozdnj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gjcphohss.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gjtuaalpp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geugnrokd.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gqfuewhid.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyzudppwr.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gsvhxwfwr.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gyakxizqb.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gkkhgusml.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gbnkteblr.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gizxbnlzi.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/ghrucxyuo.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gsrwpjnzd.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gmrlwvhde.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gcunamztk.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gxclsvvqg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gnzkpywsr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/ggpbigewx.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gplawlydi.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gassdjpwg.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gtilkzxdi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gepnxrgot.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gwriqrxcr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gfllxehrq.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gvdgfljsh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gqhcfvfsi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gwburnulh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/glswmvfda.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gwhwggigz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gshlvnbup.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gvwyaethc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gnphzddwn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/ggccaxnmn.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gsbtdwvyt.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gryblcmcc.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gkljaihbn.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gkvqcucat.sHtML


<!-- 参考信息 -->