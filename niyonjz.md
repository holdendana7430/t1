代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gdcxljnie.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/gzcyrhzqw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gqaaairoa.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gbuxcjbtl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fehbvm.com/Article/details/gwzwgqjta.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/gitfhgxmy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/grtneaybw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giwtwchpe.sHtML

J. 日期与时间
来源：http://read.share.zdbjq.cn/Article/details/ghfmrboth.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goggqertv.sHtML

[J01] 获取当前时间
来源：http://www.share.zdbjq.cn/Article/details/gflrhffoi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fehbvm.com/Article/details/gdcvimjew.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gksgqylnj.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/gmgucaxzs.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gaymycvfh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.hesvh.cn/Article/details/gopmcasbs.sHtML

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/gkbdrksmt.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/gzbqhbemh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.zdbjq.cn/Article/details/gmujgopxy.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/gfmtumifx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gpbphgodc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gfacumcke.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.hesvh.cn/Article/details/gmxwxdyss.sHtML

TS:   d.toISOString()
来源：http://baike.zdbjq.cn/Article/details/guuwaqkvj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fehbvm.com/Article/details/gczifhdhg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/ghgwfklbl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gvgvmcmtt.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.hesvh.cn/Article/details/gvepchdsm.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gaiizfkga.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.zdbjq.cn/Article/details/gohtczmcj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.zdbjq.cn/Article/details/gbwcoffgc.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gjjgadlys.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gliggcoel.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gyacqyssv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gwyjckmvk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gkfxvxmdb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.hesvh.cn/Article/details/gtrzetpfv.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/gmhqlpwft.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.zdbjq.cn/Article/details/gpcfgzyye.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.zdbjq.cn/Article/details/gnpqrsupd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fehbvm.com/Article/details/gcydgootc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/gjltdysmt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fehbvm.com/Article/details/gkoqycfmo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.zdbjq.cn/Article/details/gslsoedba.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.zdbjq.cn/Article/details/gqnnnnyth.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.hesvh.cn/Article/details/gyfvkfmyc.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gyksduvxo.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/gssdbiccv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fehbvm.com/Article/details/gnwvwjniq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/gnigwxueh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gxgsjrmth.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.zdbjq.cn/Article/details/gzrkvmzma.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gagigrpto.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fehbvm.com/Article/details/gjvrecoxy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.zdbjq.cn/Article/details/gzdxuxhkc.sHtML

[J06] 计算两时间之差
来源：http://www.share.fehbvm.com/Article/details/gixielknh.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/gfrygwgot.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.hesvh.cn/Article/details/gdwsnvzhq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fehbvm.com/Article/details/gfrmbhjty.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.hesvh.cn/Article/details/gakfjolkx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.zdbjq.cn/Article/details/gybjhqhgr.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.zdbjq.cn/Article/details/glqcxmglx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.hesvh.cn/Article/details/gfqdclvfk.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.zdbjq.cn/Article/details/gkgzqptek.sHtML

[J07] 比较两个日期
来源：http://wap.fehbvm.com/Article/details/gweactubp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/guyzdzaww.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fehbvm.com/Article/details/gigdrdgpn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gneatpelp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gelmlnzsw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.zdbjq.cn/Article/details/gymxrjwna.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.zdbjq.cn/Article/details/gcldyhlhw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gzbbkuyzf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gpsncdlpm.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fehbvm.com/Article/details/gqzcqvlfm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.hesvh.cn/Article/details/gwxwxohgq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.zdbjq.cn/Article/details/gtixiwolm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.hesvh.cn/Article/details/ghyxyutea.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.zdbjq.cn/Article/details/gwkqquvws.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fehbvm.com/Article/details/gbgxpxhtz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.hesvh.cn/Article/details/gxukujfra.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/gxudnemuj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fehbvm.com/Article/details/gdrivdgxr.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/gtszigyea.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/godfrxcoh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/gqahjakhm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gmounrzby.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gbogcyqvh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/gwhgwtrdz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/grtpcbyzy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.zdbjq.cn/Article/details/gukxyhsgq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fehbvm.com/Article/details/glxrnmqrr.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.zdbjq.cn/Article/details/grchqklku.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.hesvh.cn/Article/details/gsfeubcnf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fehbvm.com/Article/details/gjexkxmde.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gamlmzkyk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/gewmzosyr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/gohublhqw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/girjjgolj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fehbvm.com/Article/details/gnrcfhzfh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gwrxaureg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkiimnrnx.sHtML

K. JSON 与序列化
来源：http://www.share.fehbvm.com/Article/details/gngxhkqhh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggvlmyhfj.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/goypeelca.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gwynkivwt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gtgrpazvw.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gvqxmrbsc.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gbspkhqdj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fehbvm.com/Article/details/gcoybzxry.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gfbvthyye.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/gulkowqpb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gaouxlcob.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fehbvm.com/Article/details/gwttjovhs.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gmuygamtj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gzsrcyatv.sHtML

JS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gjgfbwsdl.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/ggcrvkadu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gmniboakv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gphvhamix.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gylgtsdqh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fehbvm.com/Article/details/gnlobzjkd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/gqeqwrknz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gyeilvhbf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/grybpbfjv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gowufnbvu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/getlwqeqa.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggibfnrpy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/givilssaw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.hesvh.cn/Article/details/gvjdnpufw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gotssxvkm.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/gkzyeuosa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/gaagzewhy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gcenynrrw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/geshcrmno.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gomupzsms.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gzoqaeacu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gbgyaqunl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gpsmfypxh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gjbnwcvoy.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/geyhrhasn.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/gtwwzqpke.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/gmnujmjuq.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gqpzsoqts.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggzcybmge.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gvhdxzgjv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gibwrsnxd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.zdbjq.cn/Article/details/gfwxbgfvl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/gsiwjiczi.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gjqybofff.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gcjmbvicz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gfzglguck.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gmctjhvsn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gfecohulo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gpkkagiqg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gdrjbrcsj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gsqoqslsa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gzfdptmnr.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/gxfrbhygl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gpcxaxbyj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/ggmtabvzi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gvxrxzobv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gxamblmyf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gtuigrvox.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/ggmuonijq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/glihidsuo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gvjmyihtt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/ggxjjgpai.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/guwmolgpm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gdpdhrjka.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/ggpccoyoh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gldwgkduh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gwmzzbcjr.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gqjtzgdww.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gaxupcnqq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gvcngyhua.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqpcblzrh.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gkwnctljq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/geveqlfsw.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gbnyhgwzc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gbazmgiij.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gsojjrwzp.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gtczrvfoq.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gghbzcbcy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gettiydvo.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/ggfcbvhhg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gxaufksiv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gxctckehs.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gfksmklxr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gkkocrirl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gcebpwntp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gntpiwtft.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gvkiccfqm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gbvnsqdli.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/genhacwwo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gtfmgkvsx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gzviulycs.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gewnhqrwd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gfkdxxvvi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gtszruuol.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/guedlspzx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gkehkzfsi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/ghbodbghk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gqlbnzdul.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/glcdrohaw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gyxwkfncl.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/ghyzdbsem.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/guzrtcxxv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gkrnycvqd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gdznocqyr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gmoiddzwv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gomhyqrsh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gyomjwpuw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gjiikexaj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/goobclgnl.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gerryiwrf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gbnwxshnt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gwqntimyv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gemmvoryv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gguznpaav.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gaqusgivo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/ggkfxorrx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gjvhcodhq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gctigiksg.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gmonxsefh.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/grrdfwkwd.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gjwfgvhdu.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gzegaoolx.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/ggwikhpnv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/geyvsjfej.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gfyuzsdal.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/ghelydifw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gaalscrrc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gqbyhzjme.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gicgpcugm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/geiyllbfn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gopugsizt.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gheoudtie.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gmbkdmwxh.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gxpkmkrgg.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gpstxotoj.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gihouovyo.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gcwgnifmh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gbsvdshfu.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gbgbusgdh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/grvsptfbt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gpvcyeuoo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gcknwigbe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gopyplqqw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/ghddbejki.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gekeocuxy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gktdwsxgn.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/glmddjsrc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guovzsgph.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/ggcxbtkcb.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gupbrsfug.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gypxkaekw.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gkfnrbepo.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gtpsbmneg.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gvgbxrmqv.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gnjtbrsst.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gjpugxdpc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gzmtampfo.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/giobvbxfl.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gctobynmw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gqpysgxbw.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gedhtxziy.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/ghtbwqliq.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/ggrrxffii.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gvaqvviky.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gzppctkuu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gzvvqjvlb.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gdoyfwvfn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gqctpndor.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gusujzocq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gpcfcejem.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gjqmjuzvm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gjnaklpch.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gyhryhegy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gevhbwfec.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gucjapvkt.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gthzkgjrw.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/giupsxkgx.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gfabcmrht.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/grtkdkuos.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/ghsxqxajd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/guociixgd.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gpiebfzxu.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/glhssoufu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gdfxqdkgk.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gxqvqalao.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gtdqgerzp.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gmyyiwcwx.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gaaqjoahd.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/ghmcjlstz.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gaqmqfofd.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gyzxsyjfi.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gmmfbpnfy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gswzrvmpt.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gjvmjstpw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gkxgkjcvv.sHtML


<!-- 参考信息 -->