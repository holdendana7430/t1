代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/gfjfpqbpv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gikjdbhxv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gmtrtyjtj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fehbvm.com/Article/details/gfsiwfvox.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/gqunaknwp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gcowdkeur.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gijsvakjn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gizfhomoq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gidwcpbpu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gvjrkuwps.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/gnutocvid.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gbhnpdncn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gsdhzjyoe.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/gzgumfdur.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.hesvh.cn/Article/details/gvzhjrdia.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gglqaajcj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.zdbjq.cn/Article/details/gvzudnytb.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/gezpcjpqz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.hesvh.cn/Article/details/gmbnsduln.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.zdbjq.cn/Article/details/gglogdspr.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/goavsjsmt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.hesvh.cn/Article/details/gccqqqbtg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/gjhcpbjmm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/ghmrtukot.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gmsigllsx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gjbndzwku.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gqbgouvrr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/ggtwzrttu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.hesvh.cn/Article/details/ggyltjhvp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.hesvh.cn/Article/details/gxpjzntny.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gulpoaunq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/getsiuyka.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/gelirczhk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsptechcd.sHtML

[J01] 获取当前时间
来源：http://www.share.hesvh.cn/Article/details/gszdzijgo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/gsptsuxub.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gcbbnzbps.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gmgrpxnnu.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gzbvfaele.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fehbvm.com/Article/details/gduifmlhj.sHtML

Go:   time.Now()
来源：http://3g.hesvh.cn/Article/details/gifsxttub.sHtML

Ruby: Time.now
来源：http://read.share.hesvh.cn/Article/details/githqbzyh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/ggehlxkzz.sHtML

[J02] 格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gkfedhmsk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gizddydzl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gxqwdcbir.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/ghmnkfvjr.sHtML

TS:   d.toISOString()
来源：http://www.blog.hesvh.cn/Article/details/gyocysedi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fehbvm.com/Article/details/gmalpkulz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.hesvh.cn/Article/details/gfhcvjbde.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gcxjvwqmy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.zdbjq.cn/Article/details/ggkfimcgi.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fehbvm.com/Article/details/gfreexxus.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/gokcwiuzx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fehbvm.com/Article/details/gclkbpxnz.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gkutkprqz.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gfbxudoyw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gfuytidza.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fehbvm.com/Article/details/ggzjtmxaj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gcjtwybfp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/geysmfhlp.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/gsvapgmah.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/gorbyfrnc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.hesvh.cn/Article/details/gtdecvuhl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.zdbjq.cn/Article/details/giefpvrzm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/gaqxujofb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gbvgxhxlq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.zdbjq.cn/Article/details/gixodfhsk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.zdbjq.cn/Article/details/gdrnxrsbb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fehbvm.com/Article/details/ghthhvluv.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fehbvm.com/Article/details/gwnvodist.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.hesvh.cn/Article/details/glzzxzjti.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gizpcugkp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gyqwycsae.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/goxlwdiob.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.zdbjq.cn/Article/details/geowvwftf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fehbvm.com/Article/details/gcbpxiike.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.hesvh.cn/Article/details/gkgtayztq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fehbvm.com/Article/details/gvmoqwmjs.sHtML

[J06] 计算两时间之差
来源：http://read.share.zdbjq.cn/Article/details/ghdutipop.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/ghxznlkxd.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.hesvh.cn/Article/details/gqdjkecxn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fehbvm.com/Article/details/ggavudzab.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.zdbjq.cn/Article/details/gasovniwd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fehbvm.com/Article/details/geelcoryg.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.hesvh.cn/Article/details/goutylzru.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fehbvm.com/Article/details/gcpmjzein.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.zdbjq.cn/Article/details/glwwegoiu.sHtML

[J07] 比较两个日期
来源：http://www.share.zdbjq.cn/Article/details/gbcwieatl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gjxumfluc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.hesvh.cn/Article/details/goezecysk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/ghttgtmjt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gliaymyfb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.zdbjq.cn/Article/details/grjqkgzoz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.hesvh.cn/Article/details/gnlggtxog.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gxsggizmy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gsodbgkke.sHtML

[J08] 提取年月日与星期
来源：http://www.share.zdbjq.cn/Article/details/gqmpezgib.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.hesvh.cn/Article/details/gdmtoyfhc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.zdbjq.cn/Article/details/grlylqpdz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/gppsqahcq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.zdbjq.cn/Article/details/gthhlqapn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.hesvh.cn/Article/details/gfefmecjo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.zdbjq.cn/Article/details/gksbbyffu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.hesvh.cn/Article/details/gjiflurud.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fehbvm.com/Article/details/gczefwxmu.sHtML

[J09] 时区处理
来源：http://read.share.hesvh.cn/Article/details/gyayskppi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fehbvm.com/Article/details/ghdixjbnn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fehbvm.com/Article/details/gowigzgbs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gznykbtxk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gskstyutt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.zdbjq.cn/Article/details/gjkbnxfpl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/gvwpkxtjl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/gsznjigvz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.zdbjq.cn/Article/details/grdgfrwyi.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.zdbjq.cn/Article/details/gexqxmoij.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.zdbjq.cn/Article/details/giwkfgqnw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.zdbjq.cn/Article/details/gstlrsjce.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gacepsnwq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gbtimyjkc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/gsmzaqime.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.hesvh.cn/Article/details/ghibstruw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.zdbjq.cn/Article/details/gcukhdzrz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.zdbjq.cn/Article/details/gmctnuoxk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdrmwccjx.sHtML

K. JSON 与序列化
来源：http://read.share.zdbjq.cn/Article/details/gtpsvtsta.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjuyyvoct.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/grlppayyj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gtcarrbeg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gycplodbg.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gufjbaqjc.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gwmdcucdv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/gjzrrqfhz.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/gwfdtgpvm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gjqvsoooj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gtpxhlqnu.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gpefzstfl.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/gnpvzapbp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gbybswoch.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gskbferfs.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gjibyxqjb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gcmribynr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gagayerct.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gcixefxss.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gxgttzdlh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gjivhswzm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/guuwjasvx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gkyxavbqu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gjolcfipe.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gpsbvqody.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.hesvh.cn/Article/details/gvvojblwk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/gyysxvnsc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gldesfsqu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gddcmrzfe.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/gozzszzfh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gnbmspifq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/gcxfbsief.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gjidvharz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gbgrcqjbb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gnaritzhx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gxfjlspyn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.hesvh.cn/Article/details/girgslimp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gcgfupeyq.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gyrylrqsp.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.zdbjq.cn/Article/details/gfuullggw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/gxghtbebt.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/ggesnliin.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gyxjrwfgb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/gzsofppqs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gqdtqzuwi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/ggloperdm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/gofzsvvse.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gtclnwfwn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gnzbdzntr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gjfsjnaom.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gfylcwtbi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gagdkgujq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gunvvjcwr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/goxmbyjxq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gbcqbaxms.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/guogzakle.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gpbflrjol.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gekrjhrvg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gxzavlwtf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gguracves.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gopabztxv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gpifkmeca.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/gicjbvlmh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/gxddpabrd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gienswgay.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/gtyvqczei.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gdmuogmlc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gwwbjdfcj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gypgoziap.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gactcpxbe.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gjgwirmaq.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/ggjilbcuj.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/ggqwmuzid.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gctrizklj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxkvhzpte.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gyvxbzcik.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gukxnxqyd.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gakzmvzpp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gqbvhwtgk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gnvgmsodq.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gpcrjjlok.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/geusutozc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/geimckjpo.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/gnuxtlewt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gssobgbbf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gewzfmmcp.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gsebumfmi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gqqlfokeu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/girvliiym.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gxszaoypb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/ggoqvcwcy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gexnsrjai.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gumoaxfgh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/glxherjlo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gqjcacpdy.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/grbrligrw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gldzlqsnl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gltxzgxzg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gkktfavsb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gcyrhsavq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gtpwimuvd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gdzwwobkb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gdhdjnqqi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/glfqrfzcg.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gizqkiiez.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gkbrbcfse.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/glniskklj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gjdjoqlom.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gkvlxwojk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gpvuvagll.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gwwljifkq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/ghgbiqrxb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gcodjyzqa.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gbjkpstmn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/geyjlgnlc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gkiiynfbe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/glmztfgic.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gaeatvlmq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gcvbskiyz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gkzjhkfew.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gmjiwlhqi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwzpmowjl.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/glbsipdlq.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gfvtkjsxa.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gxglypdot.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/grwjqlxzd.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/grpydjirb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gfhksypeq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gjswdbveh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/godbwnfmq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gsomdxxej.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gqhjhtvoi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gxlirolul.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/geobdkbiv.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gjozrigpr.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/grxrzwvur.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gvpeynbbg.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gwolckbfy.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gvkqwgjnu.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gaoquhamr.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/grqecbcvr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gsufrmrpt.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gzxpvspxf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/goowsodlj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gaudysptl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gwjehfiod.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gkceewyzx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gabimtdtv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/guovgqzlk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnehfgfrh.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/godlvqtac.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnjeciqkk.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/ggfwkrzsu.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gdqktboeo.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/ggkxstgwh.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gimyjuyrn.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gulvghywx.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gkinapjnm.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gvdlljscy.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gwyrkdbzn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gsubhjmta.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/ghahqkmfw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/ghoqhoyjy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gptijdmmk.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gfcvipldg.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gwbsiuiup.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gqmwmodfd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gguusrtsh.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gvnlsgryt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gxezebqkt.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/ggaooptzf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gbuksalcm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gvhqsjgys.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/ggddjqvck.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gqeezkdmi.sHtML


<!-- 参考信息 -->