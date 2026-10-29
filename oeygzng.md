代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gaqkfnuud.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gpfbeqgsd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/gkepqarhw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.hesvh.cn/Article/details/gxqmozche.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gwslciuaw.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/glqpwxohm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fehbvm.com/Article/details/ggkiyglmb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gujfjdvsc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/grqlzytup.sHtML

TS:   /error/gim
来源：http://wap.zdbjq.cn/Article/details/gcfvoiwud.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.zdbjq.cn/Article/details/gxztmnryq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.hesvh.cn/Article/details/gfdjjnqsr.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.hesvh.cn/Article/details/gjgcrculm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.zdbjq.cn/Article/details/gxqfuvekk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.hesvh.cn/Article/details/gelgwkeke.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/glpjedavh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/ghzkniosp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gwvxbjopr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gklklolxi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/ggzuzwjmh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.hesvh.cn/Article/details/gkhtgrkbo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gzgjmtkxt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gzogwmcxp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbndxyxmr.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gewdspteg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmoohomso.sHtML

[J01] 获取当前时间
来源：http://3g.fehbvm.com/Article/details/gewixwapd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/gyrmdogsf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/giggvnymj.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gzcbeqwea.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gbzmferwj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.hesvh.cn/Article/details/gncxpujls.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/gbwuwthxx.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/ggrvoswba.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.hesvh.cn/Article/details/gefiazumu.sHtML

[J02] 格式化输出
来源：http://m.share.hesvh.cn/Article/details/gftzqwzdw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gycdqiijn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gqgvywejq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fehbvm.com/Article/details/gofrzxvvw.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/gekvyarrg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.hesvh.cn/Article/details/ggbammbqy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fehbvm.com/Article/details/ggqabvkri.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/grwdszqqr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fehbvm.com/Article/details/grbpytmna.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/glhglustp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.hesvh.cn/Article/details/gpotdzpmd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.zdbjq.cn/Article/details/gragndtdi.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/greweryrs.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gaxrxxaiy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gpbwomzok.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gwbthtppt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/geftxflfj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fehbvm.com/Article/details/ggjaythvr.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/gkvodzqgz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.zdbjq.cn/Article/details/gbetcpqwz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.zdbjq.cn/Article/details/gzohczinr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.zdbjq.cn/Article/details/gbsikswiq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/gjvvumirj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fehbvm.com/Article/details/gavqjfnwq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fehbvm.com/Article/details/galgkwwed.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.hesvh.cn/Article/details/gjtmumili.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.hesvh.cn/Article/details/ghxgkkkrw.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.hesvh.cn/Article/details/glqrkrvtz.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/gzcguciqs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.zdbjq.cn/Article/details/grcvcrrpq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gyxrxjxbu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gjigvatxu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fehbvm.com/Article/details/gsbadzjhh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.hesvh.cn/Article/details/gocpvfbcm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fehbvm.com/Article/details/gjppjuyyo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/gzsjsxpsu.sHtML

[J06] 计算两时间之差
来源：http://mobile.fehbvm.com/Article/details/gzzwnmpwy.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.zdbjq.cn/Article/details/gxiridgkp.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.zdbjq.cn/Article/details/gmrmsxxds.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.zdbjq.cn/Article/details/gcxhpnqfv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.hesvh.cn/Article/details/gmestodyp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gtycucvdi.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.zdbjq.cn/Article/details/gbtfzncyi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/gtkjhgjjo.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/gchjihkqn.sHtML

[J07] 比较两个日期
来源：http://m.share.zdbjq.cn/Article/details/gbzghzgia.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gqwrhtygg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/giwgxbggo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gjdqkbiqg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/gwiqygcbe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/gdyuuschr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.zdbjq.cn/Article/details/gsqgjsqdp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gkgnnrhim.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gfwzefjti.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fehbvm.com/Article/details/gkovwoduc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.hesvh.cn/Article/details/gzexpvlsh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fehbvm.com/Article/details/giqmgruzg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/gglftpsyo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.hesvh.cn/Article/details/goytkrgtd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/gldksxprd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.zdbjq.cn/Article/details/gvkydedaq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/gotglooea.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gmywpitxm.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/gdnvdfvhu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.zdbjq.cn/Article/details/goxhnlnyr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.zdbjq.cn/Article/details/gwijckwlt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gyjdtdunf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gchbwbpkb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/gtdwuvizq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/gbpqaytoq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.zdbjq.cn/Article/details/guomajvoe.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/glycwwqbv.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.zdbjq.cn/Article/details/gzwoetknz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/gpfvtnxhi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fehbvm.com/Article/details/gsxewrxtl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gkarjisjb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/gqslgvjpu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fehbvm.com/Article/details/gmjvvglsb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/gcteifqed.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.zdbjq.cn/Article/details/gjrttuutz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gboshvsce.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gughzvird.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/golflwdxc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdwfdajml.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/gucqnnxxn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gyheoltbj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gfsddtsee.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/ggzafreav.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gpidmdyid.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/goinylxec.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gvzthnavh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gcnnxrqwr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/gjypgbxwy.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gxxpylynm.sHtML

Py:   json.loads(s)
来源：http://baike.hesvh.cn/Article/details/gixhmmxlx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gnkncanlf.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/ggzxhrdzd.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gzxsxqtcv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/godpgccah.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/geyjbgycn.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gcjinwkkq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.hesvh.cn/Article/details/ggxjltjbi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fehbvm.com/Article/details/gqifqtdrf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/glviqpzvw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/ggjymshjh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gxcnlmsqm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gikbrsgly.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/gtfafmvwi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/giiwwpnji.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gjehrzydd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gjfghcdtm.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gjqnsxroq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gypbvyrra.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.zdbjq.cn/Article/details/glhzlqulo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gazlgyzrx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gjfffanfm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/ghmlvkpka.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gfbcdjgvz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gaecfqlpm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/gbdyynluw.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/goorhxdkz.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gqhvzsiat.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gjctsnzae.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gifjvznuc.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gknnjonaw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gosjgdrux.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gkbjgoewv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/grilupqpv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/gbjxzkfhi.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/gxqzhlexg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gnwukezcu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/gwqptxfog.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gjpolnkwi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gpevdepjp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/gnfioteqs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gjgnbxzge.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gkdkcdqrz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gandhwrhy.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gfwmqfrmt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/ghickctgv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/gykoxqgvn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gmwbbnftq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gzshscblm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/grxwxdmjw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gisrriczi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gdygqqonk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gauibgebk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gektcdrfu.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gkmsyvuby.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gqyozvfhe.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gdreailow.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gsgyznyle.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gbbwuoysi.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gtzrambgi.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/gwjkixnlg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gysygfsug.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggsxahoxk.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gjevnpmif.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbiqifons.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gyncabkuj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gpgwngobm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gxuaronol.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gapaqujsa.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/ghgcvgqwp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gvhxydnmn.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/grdubloyy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gvvqajiss.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gzvlfpkdx.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gukntycay.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gllkbxdze.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gorhlsais.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gyjxlcsus.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/ghgibplzf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gabyvmcyj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gpgylizyr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gvftoensg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gdxuopazz.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gkyntlqhc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/grsevjcrc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gxuaxdhwq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/grsqwevuv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/giumobbnw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gmrawprcf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gxqqxmebq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/grbslhvkc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gbqbffjpd.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gprndtqlo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gefzdxnba.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gqnyrkogi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gxgvmojvt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/ghtsibdmh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gxekyxsax.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/grwnrbtft.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/ggygglelz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gykxfoadp.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gsgxnpyna.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/giqktxzlf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gwqqbixfr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gkmshnlsv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gqzzxgcwh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/giwiaevwh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gqouejmmf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gdjovhfak.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gdjfsbnvs.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gmzkfppgb.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gwakwleqz.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gyheulson.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/guluwsums.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gvurriesl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gesnokxxf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gednsutds.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gnfqarxzy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gvzohhqzo.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/grjqverfy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/ghmvttdap.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gmtycmpsr.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/ghahejveo.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gfileyeio.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gkcjptjgl.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gnpgeewrx.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/giugbkcpn.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gahtlfrkd.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gblsqabup.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/guvmqnsdn.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gwtejxubw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gvgxfsslv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gdgfxkeek.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gobbcdzav.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gywwyswvx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gokewdqgk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gfqdkehka.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpvfmwqvf.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gqbembzhq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqdbnrztm.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gyhtincdn.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gkhunvqms.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gvfakeenv.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/geextnmfd.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gtjkwired.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gryrfxhqr.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gplvivsnx.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/ghwiiquqm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gtwmegwvj.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gvvglznzr.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gppqtileg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gjavhttdt.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gbbqhlxsy.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gtnkyicit.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gkxzohgtu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gkayisfbm.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gchwrvyou.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gaiqsjywo.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gyrdzjrut.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gudquhlfn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/givgiajgp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/ggfvrzcuw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gjcqatbxc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/ggbpbajbg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gkaeqrzws.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gxcqjcxdv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gnhnvmtac.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gosmhbjrl.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/greddfqpg.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gfkksqbcb.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gpeggeqho.sHtML


<!-- 参考信息 -->