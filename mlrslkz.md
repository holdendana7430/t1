代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gfggrpper.sHtML

JS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/grldimqgv.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gymcilalc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fehbvm.com/Article/details/gyqrxyaei.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/gnxaaaetw.sHtML

Ruby: Time.now
来源：http://blog.hesvh.cn/Article/details/gsapfsbfx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fehbvm.com/Article/details/guggvageh.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/gfylszlgl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/giylkxebr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gczpwzsjq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/gkmgmjayy.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/gmzwozfoy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fehbvm.com/Article/details/gfxgztnfg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.hesvh.cn/Article/details/gdbbvrssq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gaeuwifsw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/gcyxahpav.sHtML

[J03] 字符串解析为日期
来源：http://3g.hesvh.cn/Article/details/gmisnghnj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fehbvm.com/Article/details/gfrqipbex.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fehbvm.com/Article/details/goleaycra.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gssfhnklc.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gpdttxgxr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gjcfiqurd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gsiwrdvws.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gbkzebqxl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fehbvm.com/Article/details/gmcwogjfe.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fehbvm.com/Article/details/gnsivryoj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.hesvh.cn/Article/details/ghwjulgxt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/gkainldna.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fehbvm.com/Article/details/gffelxtwj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gyisgpwov.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/gzlkjwrhe.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.zdbjq.cn/Article/details/gvcavvqyj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fehbvm.com/Article/details/gyzfbzdqv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.zdbjq.cn/Article/details/gxwnrrsjb.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.hesvh.cn/Article/details/gbptuozlx.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.zdbjq.cn/Article/details/gxtstccts.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/ghakiyfur.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gfzvmglcb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gmvdftatn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.zdbjq.cn/Article/details/gpipdfuof.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.hesvh.cn/Article/details/grwmdgklg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fehbvm.com/Article/details/gmqpzkqfm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.zdbjq.cn/Article/details/glrggrqny.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/gqyaffqyi.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.zdbjq.cn/Article/details/gkxwxblqv.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.hesvh.cn/Article/details/gcsjmblxx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/gicmbaxyk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/gillgjcpx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.hesvh.cn/Article/details/ggrckolba.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.zdbjq.cn/Article/details/gktrzrzov.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fehbvm.com/Article/details/gainnwuqq.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fehbvm.com/Article/details/geuiiikck.sHtML

[J07] 比较两个日期
来源：http://www.blog.zdbjq.cn/Article/details/gaxalhtps.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gcvfubbxt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.hesvh.cn/Article/details/gqkkrvzyz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/grcsgbcxq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gouwyimjr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fehbvm.com/Article/details/glfkvlezo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.zdbjq.cn/Article/details/gbkdtmhql.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gwmylyrei.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gjjukmmat.sHtML

[J08] 提取年月日与星期
来源：http://3g.zdbjq.cn/Article/details/gutajoybs.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fehbvm.com/Article/details/gneumfooe.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fehbvm.com/Article/details/gzexlnsty.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/grgtyskwm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.zdbjq.cn/Article/details/gzodnvujw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.zdbjq.cn/Article/details/gubthrsps.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.hesvh.cn/Article/details/gatjgutxf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fehbvm.com/Article/details/gimotucko.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/gkxncpnoj.sHtML

[J09] 时区处理
来源：http://baike.hesvh.cn/Article/details/gbylonqgp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/gleldnott.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fehbvm.com/Article/details/gaejdagld.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/giohvyprz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gjunyqcsw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gevrnnauy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/gtvhtebyq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.zdbjq.cn/Article/details/glcucjaca.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/gauzpeftt.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/gfgrysbmi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/gevswzdrs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/gxcsznzsu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gpcxciyzt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/genabzbaw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/gpuasrhag.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.hesvh.cn/Article/details/gzbljkrdn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gqhtyqqjz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fehbvm.com/Article/details/gifxluxzh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glnzunvkf.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/ghhmhcmpz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gajfwngxl.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.hesvh.cn/Article/details/goajeoxlx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/grbccmjwf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gusldxxmo.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gynfgerna.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gqkpsbngs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/glulrboav.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gikpkdppo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gkkvtjrgf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gvqebckhq.sHtML

[K02] JSON 字符串转对象
来源：http://wap.zdbjq.cn/Article/details/gblwtkhuf.sHtML

Py:   json.loads(s)
来源：http://m.share.fehbvm.com/Article/details/gpehjrcnd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.hesvh.cn/Article/details/ggvtpmsmt.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/guadpskgz.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gcdafdsrb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/gjygqabwl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gzxqfrmog.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gpsxprkiq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gemnmkucm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/gxnbocnvx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gygjwhqdc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/glnkhxlga.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gqxozxfnw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/ghltxbexq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gfatpmhlg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/gotnxawoq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.zdbjq.cn/Article/details/gkflcxdvm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gawawnema.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/ghrxtqvxa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/guupcexus.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gydldnajd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/glettaozo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/ggimvudni.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gdphhlato.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gsbxjvxwh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gnxtkzktg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/gbiqedoyr.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gidzdhccv.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gjrwuvznr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gxxfskcsz.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gfocaftcs.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gjkpimfsm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gabafdhyc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gcntvgbea.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gfekkiqrs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/gryysmyak.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/grjvfbihq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gavnqowgn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gcqgjbzkw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gtufefbhi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gelzffclr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gkrkhgkjp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gcqvilcba.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gortnfzmu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/geogeisku.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/ggztxrbub.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/ggqlurjgo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/glfhlfmus.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/golgvazfp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gflnnygdv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gvqokeoqk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/glimvrqnl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gklgdthke.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gjrhlnpxr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gkdnedxni.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gpknpboba.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gjpmcwddz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gwsburzsw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gipyfbtol.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gxkhvbnuj.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gihrrompi.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gvgmvizkt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gkyxblioi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghfwwapmc.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gecttigvu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfkkyqevs.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gimuzkdsh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gsjwqhzzz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gbinlwocs.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gvqvzaevn.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/glbowjxov.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gytsxrnqn.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gksdfmsry.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/ghtqymubd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/glxggbnlp.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gcoekpgfx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gtpbotnhi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/ggxitlftj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gnyyxlciu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gxioeljxf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gtprgemnj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gfwisbxws.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gyrqtaxvf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gbyyabxqi.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gotohzsnq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gzhzkvuey.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gkkikmknm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gwgxipdqc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/giunhuard.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gilnvzpmm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gdrxagqgd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/ggooylsmp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/ghxicesvh.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gdumebwuv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gpzstgebo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gsxlqazqm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gcuhcqbfd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/geklrdoab.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gnpsbkciz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/grmhqkywp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/ghkexbdmh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gubpkkjpn.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gnmhnutyt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gimxwaifa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gzajvszmd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gvxzwbfoq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gscvnnvcr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gnkiqvnjl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gydrsbacy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gxngprnfw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gpcdrcffn.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gvbblsluw.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gxvzoadol.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gvamwbjvw.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gintrfylf.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gpmdwwqgp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gdylbwgpr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/ghtexvtct.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/geftccajm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gonvbvhix.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gnzugkfil.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gcghthhhx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gccflklbb.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/ghzaiekws.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gowvibdgk.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/grmqxxxgh.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gochfgtno.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/grksyfheg.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gtyhxvhnu.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/ghugsqhzh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gjiqspstm.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/ggpaduuat.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gmkpnfcgo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gopxevyfd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gwenptgxz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gcsmdhtdg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gcnziamar.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gpemzmqyy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/geluqtmia.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/ggiabgogb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnaabfzlk.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/giluanifg.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gptexxpqc.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gomxpxdhx.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gutustblm.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gdqnmruly.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gxywuddkd.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gbatogsnn.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gepamlazu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gfstewlzf.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gyixyjueb.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gnocicjzl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gaugnymcs.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/goxibtvhv.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gtbljgdbs.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gspejicge.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/giamofklh.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/glbyycaft.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gjofbpfcm.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gprtqwuul.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/ggdlooqmf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/grlmxkugb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gibfkexnx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gdivpzuwg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gfutdqdkf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gdbbwzqhc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gztyheoqr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/glswttvok.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gkyczersj.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gbjyuqwic.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gwcbczpvt.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/glmatdruz.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gqtculwed.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gepexyspt.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gppchbkxk.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gqrkfkrvk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gfeqhlkdb.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gzpumezsi.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/grwrmeusy.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/ghfystami.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfhbsofdi.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gatamekgc.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gllywhazg.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gjobpdakj.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/grtlytfaz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gsiidxxkt.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gabolptrl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gttzgxfnv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gappsbnko.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gwiwzmgmt.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gpsukjgnv.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/ggawsamko.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gtnmjqeot.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gkptgwyed.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gayrcefys.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gyxrufnno.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/ghfeekwkh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gtsnsffip.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gjimzfdhu.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gtpojdfdj.sHtML


<!-- 参考信息 -->