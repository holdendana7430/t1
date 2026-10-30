代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbsimifk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/glfijccux.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fanxiaobao.xyz/Article/details/gcjkvodkh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcgibehl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxlhzwiw.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlaeztpv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfsagqex.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fanxiaobao.xyz/Article/details/goamzsxdi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fanxiaobao.xyz/Article/details/geaazilwo.sHtML

TS:   /error/gim
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnarfdxzv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fanxiaobao.xyz/Article/details/gltbosylh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fanxiaobao.xyz/Article/details/gsnzjxojk.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjtgbkjf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufoctxtf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdajzwlai.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fanxiaobao.xyz/Article/details/gthhacoiu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fanxiaobao.xyz/Article/details/gjulzyyxi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgzjuswt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqigfpwy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/grgaqofvs.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fanxiaobao.xyz/Article/details/ggasotnip.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fanxiaobao.xyz/Article/details/gacxsljxe.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigawumfj.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmtzmitd.sHtML

J. 日期与时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvugrwkx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnamesgi.sHtML

[J01] 获取当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnnxfbay.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxxuxdsj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fanxiaobao.xyz/Article/details/glssxfnwg.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fanxiaobao.xyz/Article/details/gnmeeycjq.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvrwjwlf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaztrfej.sHtML

Go:   time.Now()
来源：http://3g.fanxiaobao.xyz/Article/details/gotmxdnpn.sHtML

Ruby: Time.now
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxavlsey.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejvtvjwd.sHtML

[J02] 格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gcyeshghm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxoyxcbv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauaxdzuh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fanxiaobao.xyz/Article/details/gzjrpofxq.sHtML

TS:   d.toISOString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjspwddsp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicmodpap.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fanxiaobao.xyz/Article/details/gsdlbkaft.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxhpgswe.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fanxiaobao.xyz/Article/details/gdaitcvli.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fanxiaobao.xyz/Article/details/gyscicbur.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtixmpzaj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fanxiaobao.xyz/Article/details/gxqjoyhoj.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gmsvbxoyb.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsumprdix.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/ganrfhude.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyepvchj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gpihwrund.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptieucfs.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxllfbvqn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gygwicgfi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fanxiaobao.xyz/Article/details/gsimnlwzr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnawdhxpn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gksacjslh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/gmyigvrna.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gphngqryu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fanxiaobao.xyz/Article/details/gdojgkivn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxbiihbj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeehlyrg.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fanxiaobao.xyz/Article/details/gbikdsijf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fanxiaobao.xyz/Article/details/gumfmgdbt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fanxiaobao.xyz/Article/details/ghirinixc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcttokrvp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqgfmjzv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcigqilss.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fanxiaobao.xyz/Article/details/grcgevajs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrchzfss.sHtML

[J06] 计算两时间之差
来源：http://www.share.fanxiaobao.xyz/Article/details/gacxmvxql.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycdgeuwx.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnsqoowk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsbjdetn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdhiwzar.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fanxiaobao.xyz/Article/details/gekfmklmj.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fanxiaobao.xyz/Article/details/gpwkoudpu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fanxiaobao.xyz/Article/details/glxkasnsx.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fanxiaobao.xyz/Article/details/guagshhii.sHtML

[J07] 比较两个日期
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbmxsteq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gskwzyjdd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecnmlrrq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmqyklin.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fanxiaobao.xyz/Article/details/gwboszbea.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/geqvtlxfk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fanxiaobao.xyz/Article/details/genbkjxni.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/gplghxojv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gtjderkiy.sHtML

[J08] 提取年月日与星期
来源：http://baike.fanxiaobao.xyz/Article/details/gzzdrfxja.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fanxiaobao.xyz/Article/details/gklqmenpp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fanxiaobao.xyz/Article/details/gkcjzttfv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjxaiyka.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxelhmjeg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnblzjjkl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhzvowjt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfmzrqum.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxfwfmnn.sHtML

[J09] 时区处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gsygyfmvf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqaaydkx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxeabcmu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fanxiaobao.xyz/Article/details/gkbjqkizr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/geushcaoz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fanxiaobao.xyz/Article/details/gznbjpupd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fanxiaobao.xyz/Article/details/ghrrwmeue.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fanxiaobao.xyz/Article/details/grjlgpego.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrurkuge.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fanxiaobao.xyz/Article/details/golkcbugj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwemmmezz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxhdljfv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkddbwaku.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gtccuoalj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/geqmnmkwh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fanxiaobao.xyz/Article/details/gkmotepyj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggktcoxam.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxwprehh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gscinlcdx.sHtML

K. JSON 与序列化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gestmnynm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuyqladb.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkvfbksd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fanxiaobao.xyz/Article/details/gocafaskv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gtzwffahl.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/galigytcc.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gkinjnfoj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fanxiaobao.xyz/Article/details/glcaqjeyf.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/grlhcuucw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fanxiaobao.xyz/Article/details/gzpggeywp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gtiwnpbwh.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gowedefrl.sHtML

Py:   json.loads(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gxvqrdlad.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gkldjgupl.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/giqyxwpyf.sHtML

TS:   JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gxbywjvdk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumtjyuwc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzhbeufx.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzidxlrp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gtokjnnkj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyilaezrn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/goioclszg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqisscpw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybkuwcbi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslcunmpj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoflfgwi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fanxiaobao.xyz/Article/details/ghonutulv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdpredtg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhcklqzc.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmwvkjel.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwbyjkkb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiygxfdr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrxegvao.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmmmhxoi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fanxiaobao.xyz/Article/details/gqzrwgdzl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhyxlnfp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmqfacbl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gckbcezmf.sHtML

[K05] 深拷贝对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfmcklzg.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gyobgruek.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnqenlcu.sHtML

JS:   structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/grshpzbpx.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtorzgvy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fanxiaobao.xyz/Article/details/gucgbqwli.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkakfuuak.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctgfkupc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fanxiaobao.xyz/Article/details/gnrymaeez.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkdinsaj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fanxiaobao.xyz/Article/details/gkewxnlod.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqhfflsj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdyvqtwo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gypqzybth.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fanxiaobao.xyz/Article/details/gjurdbkei.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gevzyidsn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/gbmngnkfx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fanxiaobao.xyz/Article/details/gfqifyudb.sHtML

[K07] 进制转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxaztooa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gnrivqekl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fanxiaobao.xyz/Article/details/gayrtukyx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/grslrjbuz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwefvqww.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchqeutrj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpkqbtfy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxorkmtr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvyyelhy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fanxiaobao.xyz/Article/details/gkqgqvhfs.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiswwdez.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gvycpmwzh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fanxiaobao.xyz/Article/details/gkjrraihg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgnykeqq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fanxiaobao.xyz/Article/details/gcseguahf.sHtML

Go:   encoding/gob
来源：http://wap.fanxiaobao.xyz/Article/details/grjbavhfe.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlixvfpz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fanxiaobao.xyz/Article/details/gtsfbnrkg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfduuzuaw.sHtML

L. 网络请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcbcfqtk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/giadjgbxc.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeoiasfp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpdclxoq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhxmrsfb.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoyiktuc.sHtML

TS:   await fetch(url)
来源：http://3g.fanxiaobao.xyz/Article/details/gcotokdga.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fanxiaobao.xyz/Article/details/gwookecbj.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitmcqxtn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyyegxfe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gipklzfos.sHtML

[L02] 发送 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gbciqpvzf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbnxvami.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvlqfwbk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/geqvamtql.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fanxiaobao.xyz/Article/details/gmuehjiwm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdyedegk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fanxiaobao.xyz/Article/details/gaujfhiim.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fanxiaobao.xyz/Article/details/gvqzwwovu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fanxiaobao.xyz/Article/details/gnkivggfw.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fanxiaobao.xyz/Article/details/gpizsqkgc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljyeybsp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiqfofoc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbnslghe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfgnxpix.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fanxiaobao.xyz/Article/details/gkuyrpmlm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fanxiaobao.xyz/Article/details/gthsayhlh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fanxiaobao.xyz/Article/details/gzrqwbihd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgbeshym.sHtML

[L04] 设置超时
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfhuorqo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fanxiaobao.xyz/Article/details/glbrxcajl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/gcydxcfft.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrxgharc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezcmvvuz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmzccgku.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guloytssp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fanxiaobao.xyz/Article/details/gqsjfraaq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gwpsnvkki.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fanxiaobao.xyz/Article/details/glqnyzsag.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fanxiaobao.xyz/Article/details/gjziqqbwc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrlrntir.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwdqcdje.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fanxiaobao.xyz/Article/details/glruafubp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcpuifgd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwkswkse.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fanxiaobao.xyz/Article/details/glrqetulj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gvqjeyyrw.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gckdnbwtu.sHtML

Py:   resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goufmtxyo.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqqnewgc.sHtML

JS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghilouqax.sHtML

TS:   await resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/gmlnldard.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fanxiaobao.xyz/Article/details/gwllwzncn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fanxiaobao.xyz/Article/details/gdcssjrnl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlbfabgy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fanxiaobao.xyz/Article/details/gntlenfgp.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gaplbhayj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefgmvxxq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gmaakblre.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fanxiaobao.xyz/Article/details/gjaeexnnd.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fanxiaobao.xyz/Article/details/gclblexde.sHtML

Java: resp.statusCode()
来源：http://baike.fanxiaobao.xyz/Article/details/geukikyyp.sHtML

Go:   resp.StatusCode
来源：http://3g.fanxiaobao.xyz/Article/details/gjjpzylil.sHtML

Ruby: resp.code.to_i
来源：http://baike.fanxiaobao.xyz/Article/details/giaotkeik.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fanxiaobao.xyz/Article/details/guegazezr.sHtML

[L08] 并发请求多个地址
来源：http://wap.fanxiaobao.xyz/Article/details/gjzfvueap.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fanxiaobao.xyz/Article/details/gqtsydzmu.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fanxiaobao.xyz/Article/details/gseqtivyn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbqpxsoy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnsvkhwg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrvavoko.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fanxiaobao.xyz/Article/details/gynkyoeuf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkclkteza.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbdvmefh.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwazqstej.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsferacx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjqsrpzax.sHtML

[M01] 读取命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbfklfdb.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhqtuvop.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fanxiaobao.xyz/Article/details/giwqjtrbw.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwedgukb.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gkfsotrgf.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqzbfnbl.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflvipkqz.sHtML

Ruby: ARGV
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnbifkhr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fanxiaobao.xyz/Article/details/gamznhhwj.sHtML

[M02] 读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkicquov.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcjconrw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fanxiaobao.xyz/Article/details/gilooyssd.sHtML

JS:   process.env.HOME
来源：http://blog.fanxiaobao.xyz/Article/details/gcccirtib.sHtML

TS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqwtfppx.sHtML

Java: System.getenv("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gtaeflcnv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/giyygxwww.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fanxiaobao.xyz/Article/details/geniscdvu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjtweytk.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqocobrxp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuaarrng.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fanxiaobao.xyz/Article/details/gljnbjazl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwoyktba.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fanxiaobao.xyz/Article/details/ggxmcndkj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvjsjgjs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdiaupki.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fanxiaobao.xyz/Article/details/gfazvgrju.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fanxiaobao.xyz/Article/details/gnmetpakz.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllsvvanw.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnkhliju.sHtML

PHP:  getcwd();
来源：http://read.share.fanxiaobao.xyz/Article/details/gdigtvdbs.sHtML

JS:   process.cwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gcwfvhlct.sHtML


<!-- 参考信息 -->