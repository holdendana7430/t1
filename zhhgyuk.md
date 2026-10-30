代发 wailian999

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gpyjtncro.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gctwqksgb.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/gezmdawsk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.hesvh.cn/Article/details/gddhteusm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gocrztocg.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gorvhfjdf.sHtML

TS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gkecwyzeb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/gtjyeknme.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/ggwpkxhnu.sHtML

Ruby: Time.now
来源：http://blog.zdbjq.cn/Article/details/gnxhowyzz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fehbvm.com/Article/details/gwuhitnpd.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/guxobyfkh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gccwmttym.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gorwfjdcl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fehbvm.com/Article/details/gztqeycwi.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/gauggjeic.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fehbvm.com/Article/details/gaclnhnqh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/gjsmagmdn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gympavdvp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/gtdytrvri.sHtML

[J03] 字符串解析为日期
来源：http://baike.hesvh.cn/Article/details/gjmgobbgj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.hesvh.cn/Article/details/gdstmrexz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.zdbjq.cn/Article/details/glpsmoolx.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gjqzksrzj.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gttjtvuqj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gsfkimqvo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gkxrvfkhv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gurofvebt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.hesvh.cn/Article/details/gntvzhijc.sHtML

[J04] 时间戳与日期互转
来源：http://baike.zdbjq.cn/Article/details/gzxsxzkeh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.zdbjq.cn/Article/details/gfvbholmj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fehbvm.com/Article/details/gherzmefc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.zdbjq.cn/Article/details/ghmuyrces.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/gnzrixibg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fehbvm.com/Article/details/gqnetplbm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fehbvm.com/Article/details/gckbnefdg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fehbvm.com/Article/details/gfncecdly.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.zdbjq.cn/Article/details/ghfkyxowe.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.hesvh.cn/Article/details/gjsjwalus.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.zdbjq.cn/Article/details/gljyvilvk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.hesvh.cn/Article/details/getweqxbt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gpuqzeqvr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gzprwpjos.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.zdbjq.cn/Article/details/gbjhcidjy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.hesvh.cn/Article/details/gagfmomik.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fehbvm.com/Article/details/gpgmriytm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gdbmzwgbt.sHtML

[J06] 计算两时间之差
来源：http://wap.hesvh.cn/Article/details/griufjteg.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.hesvh.cn/Article/details/gigqrflix.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gldidbgrs.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.zdbjq.cn/Article/details/gaakthxpg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/gnkdxjxrm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fehbvm.com/Article/details/gqlujssax.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.zdbjq.cn/Article/details/gjmdpvsjy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.hesvh.cn/Article/details/ggasjtlme.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.hesvh.cn/Article/details/gpajryzsv.sHtML

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/gdpfozvtv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gjbzmynsk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.hesvh.cn/Article/details/ggcwzmphu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/ggxusmlmq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gpgalwlbk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.zdbjq.cn/Article/details/gzsrtybvc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.hesvh.cn/Article/details/goafzbaey.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gdfsqhkul.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/glhizdtpw.sHtML

[J08] 提取年月日与星期
来源：http://baike.zdbjq.cn/Article/details/gnamyhdds.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.hesvh.cn/Article/details/gcperigur.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.hesvh.cn/Article/details/gpuqqjdce.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.hesvh.cn/Article/details/gesdnsfzd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fehbvm.com/Article/details/gvzzavuyy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.hesvh.cn/Article/details/glpfdssqt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gbgwiwcnm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.zdbjq.cn/Article/details/gdkevntkd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fehbvm.com/Article/details/getijcnlp.sHtML

[J09] 时区处理
来源：http://baike.zdbjq.cn/Article/details/ggkgdzunm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fehbvm.com/Article/details/gaiuiqpbo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.hesvh.cn/Article/details/gditorevv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gjttqnsbo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gyctqpqfr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fehbvm.com/Article/details/gagvcrfew.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fehbvm.com/Article/details/gidotkusq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/gioltqivp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.hesvh.cn/Article/details/gjqpcuzvv.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/grneyrlip.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.zdbjq.cn/Article/details/gclglhfts.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/givyjikww.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.hesvh.cn/Article/details/gprobtrvq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gmroapcqa.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxcgzdxcz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/gskgsagpf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.hesvh.cn/Article/details/ggvhqddgd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.zdbjq.cn/Article/details/gusarkqfx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvfuadzeo.sHtML

K. JSON 与序列化
来源：http://www.share.zdbjq.cn/Article/details/gcxapvilb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gskdnnnyj.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/grqokqxij.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/ghwjekppo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gvddysuvx.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gdikxaaxq.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/guzfvmwok.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.zdbjq.cn/Article/details/gnfgsljni.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/gcdinzdrw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/gahhksozx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fehbvm.com/Article/details/ghphykdxq.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/graumwjwk.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/ghthzqaab.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/guubitcim.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gjtprdmfm.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gsuptjkrf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.hesvh.cn/Article/details/glwhdiyie.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gdfpwneuy.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gfpruemfr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/ggecsihaj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/gwqbepttl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gyqlsblfo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gtnxiqzcd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gyscbopxy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gfeyvhwkh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gvtthabgz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/gfecpebmo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gyrfiacpp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/gieouavho.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/goazlvksk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/gaqceaqpn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/ghrnnjikx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gbodhxnbj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gzbltbzcs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gvumkapiv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvsnlbws.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gwhywuflq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gppgykeft.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/ggpbuegex.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/ghaflyrov.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/gqkcyueya.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gifzbkxmo.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gpjliqsay.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/gymidcmml.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gpsvzwifa.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gplfpsymg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/gucbfzwix.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gzgepuqfr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/gznzmrytg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.hesvh.cn/Article/details/gkajimdnd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/giqjnvqte.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gschasspe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/ggzqnwktv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gzaazmdkx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/getufkbro.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gxrbfesgs.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/getmfznbq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gmcdgposf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gtddlzjbf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/ggvvoxnok.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gbmjhgjkk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gcgwbhhdi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/gyugpkwmn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gqpoojjpr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gvtdpdkme.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/gcbjlhjgx.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gtnhcxras.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gbsfsiwyb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gzqmgjtrg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/ghvmxesdg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gozmplbbb.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gyvsjkpul.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gcgjcjdrj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/ghyymmnzu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcshkxnkh.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/ginzucjih.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwafawift.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gjeygpgpf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gacllaaut.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gmxdwwphv.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/germoybhh.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gtiuplmtx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gdydvzrug.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gyrbvbyvn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gmwianxed.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/gyjbwtgvm.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gucpropbk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gheshesss.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gjkcbznap.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gqtzmnwtm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gkatiptht.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gpgnyjjzv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gqcohpmck.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/goxwsbgwm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gtpamnsyh.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/ghtwsseit.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gefyuslfi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gzzifcael.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gbryrgdzc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gflajwewv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/ghkcelzcb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/guegdjwhu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gxkgovrhc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/grvqsgtsr.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/grxgspyuo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gbmhgayxh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gdzytidrb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gzyjqrzep.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gokrejecl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gmsvrsooy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gfzejtskc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gddzmkmrb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gaesbxjok.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gheblcaie.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/glhnmswqd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gmlsrguow.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gmhnvulxa.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gmarjhugo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gbxualhww.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gaxqhpncb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gwhneukdq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/glkhzhojj.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gbtopurjo.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gvnualhox.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gunetnwvb.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gbmpxufkb.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/ggureqdql.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gvntvibyb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gbwojqqab.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/guxiujrzl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/guvmntsey.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gtlirzwwx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gvpxhsukt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gorpducgz.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gyybypyvj.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gbtnlucck.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gaofyjaar.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gekszqnth.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gbjrhuqax.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gnptyfqyy.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gnsybzbdn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/grjyzjxjf.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/ggtsrkcwv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gqzstiahn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/ghhgltqsv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gmnlhydea.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gbyfglykx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gaaytxwbg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gqscfzkqa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbwtrxjuk.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gixfxietm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyyoyvmau.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gbaeklrdy.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/ggfronaci.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gwxgzmadw.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gieteojyv.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gxrsdzzti.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gxzmwbofo.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/ggfvdtwdc.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/grzvtnwfg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gycjtfxjs.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gbgmirega.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/grdztfwet.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gblvliexw.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/glxtsfolr.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gkigikalo.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gqlnzkzha.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/ggcbxwyzb.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gvkgtzugg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/galnwldfj.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gafwlxoky.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gbuzvtffc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gskydtgsw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gpmtwhyph.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gazvfcgfh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gzhrthtpd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gnijecrkz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gwcsqitbx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gwbdvwjph.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gxijqmtav.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gwexejmts.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gnngdduwr.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gscewfgri.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gdoyjsmkg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gnvsrwurw.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gjkjgoomy.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gqhxainfn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gsxbforyr.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gyvzinuef.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwhdunguk.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gscokazze.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gltqgtoga.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gurtpqjcx.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/grmgjycoe.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gqymewsts.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/grjstipej.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/grfbgckje.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gyhfkdfft.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gljhmtmif.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gheagdixb.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/glahlufrz.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gukmzkqyd.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gsbcmbmlo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gynuapnhe.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gtmtkloay.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gbauwuzey.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gsosrkcuj.sHtML


<!-- 参考信息 -->