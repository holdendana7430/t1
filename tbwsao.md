代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ufbkhxhn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3myebghit.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3wdstltkf.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zfszsxgu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3leosqbsa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ysojcfxn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3wqnazrsh.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3hmtshruf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pjwcgrhn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vlymubpy.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3uwhmkpzb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3mrwtfxzo.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3mpgbdhzc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3nbqwxxam.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rbocdwzo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3yarfdvde.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3akuftebt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qgrrxubc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3xsqsbttj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ggmzswij.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3wkwymutj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ovjdzbkr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3kvljbcmy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3vnsavthk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wuuyrfyk.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3ukkyjxxi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3vuegfoxc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ghomwzke.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3xpajhksz.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3youbdvwq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3zsnlqxho.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3uhnxblpe.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3difdjhtg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3fdjutnbh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3hgnvmqlw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3edmubcls.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3rwevdmpx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ijsdxrwb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3sdriujez.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3xyshmdat.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3fwpcowhb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3jyvnhqul.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3gjynpkot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wfcpmzsp.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3dmjebdkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oshhhsqy.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3xuxzavjd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3ycgmwhfn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ftppweor.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3lehfeyuh.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hhujuqef.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3soursdye.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3vycidttp.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3xsdaubce.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3nowwjtjg.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3maawurkr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3mjtaamxp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3cquajfqf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3ddjzdhxz.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3hineguck.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3geqfmqcf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3uvzgufuq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3tnqikehf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3nohocyfo.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3yeidsqxp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3tfdvhhba.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ofgzrgsh.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bmublrrb.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3illftoqv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jdmptvnl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pfzpbxpq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zduyayir.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3zfeqvshp.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3qktpssxc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qaonatwe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3rdoamzhs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3wjqzbqpm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ttjpdvbb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tadgsawd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ksgqwett.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3riqghhfa.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jmlopgtw.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3zmthdiej.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3jhqihdfq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3wwppciav.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3bmllzjoj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3cwrovgrt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3nourstxp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vwjtfctl.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3dgykhvwl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3rhprjpva.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3nsaudpuh.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ulaezwqo.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3bgxvvyfb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ipmvnoww.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3afgkvosv.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3deiahlfz.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ticclvin.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3oovbevdh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3sumosxph.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3fsntzlxw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3agaiogyf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3xqmiiraj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3zhjsvmqs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3zbqdcarn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3vevmkkyi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3jiemradr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qaxbdsxb.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3wkauifla.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3sslmzkis.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3sfukmkwz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3hugklypq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3tcumvovi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3utomtovv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3lzuljsob.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3tvgjvmuy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3qyrmvyaq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3kvhdvhwi.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3gpgyqhzl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3ehqtoudu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3ypzqbjvi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3wvnzysfc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3inqpnpig.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3hxlpbqcx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3spsyoqkr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3toggkzap.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3hmxiztcd.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3fawkyfdv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3twgzwnbx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3juegvuhu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dculwaxo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3gpbcvqwb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ehevbogm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3vpqlrizb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3kicjbdoo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jabfdwoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldzadbig.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ysvznmsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iezhxokn.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lswmgzqi.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3hqzlktbz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3voklvygz.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gdrhlkiu.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hhmfgfme.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3vsmyholg.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nrzeazpp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3uvabnxkz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oosjsube.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3dkkvvklr.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3udebfdks.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3vsylpvlx.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pauxfvgh.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3efoouejk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3noqwmilq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3amnwntkw.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3nssmvgzx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qsmqdtwm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3rkkhdame.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3vjddlsny.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3rzeqmsal.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3cjxjxpxg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qffeefrb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3yxljnoux.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3mnyubfce.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3qbeagklm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3stqxihmx.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3cldqtxii.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3eyucbklm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3captpymj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tlmvxhsn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ksazkwne.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qoozetuu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3gmlidlpt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ufffmbfu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3rczvczuo.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3jtwksoyg.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3vkvdtbdh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3wybbgjsy.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jaeqswgp.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rmrtwnsc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3tcozsfhy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3zhwpqsxi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xjvqkxor.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3qeavucnd.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3rqmrszvq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xknnhhkt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ztnwibxz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3wlujpqkt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3punhwhdt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kncabdbb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3eakxonma.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3isbcqkbr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3etffzsbs.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3uiwyxojn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dhrgmmcr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3rvopntvb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3offsrmds.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ecflzzhs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qonqwimj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3wlynoter.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3dsmvljjv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3taekjshf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3dnywubdf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3uuphaatf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dxukjfbx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3nzwglmgh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yzxfglgs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3iqcszsac.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3gifpzmwu.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3awwngowd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3wgedesbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmqzpzha.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3pvsdmbaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxcsbydt.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3xbzdgyap.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3hhksrcbo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3popxuzit.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3tsfjzdwu.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vfyxxjxn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3olhzexgt.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3vkfpjlnx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3wyfdjdiq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3oopdhqzw.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qfllcffr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3zacxpaoh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3vvvtaqpi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3eyhwfvhy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3kfarqktf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ssupkwhn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3crgvptjy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3onupivvx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gbqssnvv.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3kdbdknvm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3maaknqxa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3yjibtjos.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3exyynntc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rbwrvsuc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3wbryojyv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xnqssmcz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3fimyicvh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hmsgutka.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3vqjkihmf.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3tjeqhvej.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kjggiaih.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ihppusso.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3twljlkce.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3tjanyphq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ykfdfxtf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3xtipowpq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3htqboenj.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3txnrfbqm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3wzudsrqw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3apraxhao.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qhxwdjrk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3leufpagr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3vklaqszf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3mpnjgbvg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3sbicjykw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ntjqeizp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ldyaiilv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qarlkhbz.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3zfilmbnp.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3iczgtcsl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3iwzauemq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jxfbxasx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3qdguounk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3hzcqhkes.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3tkbvszdr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gkjrlzqr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3dggpcqpd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3yqlxwwnz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3izqessad.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3corohbdl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3tezzvxkd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3znllaybl.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3dbrobrbr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gawfvwyi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3pilkgmoj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3nbndyprl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3nwbxrhae.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ysapvhry.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mqzxgjai.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3flrssjwr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ynuetnyx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ppgqjqpq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3swvtkshr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3puxmibvx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3tmgeqlvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3auejklec.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3oqcmwuvb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gltgzcuu.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3fnnkrzvj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3chivwtbu.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nscnoduy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dxmxygzu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3aozbmigt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3gnednszy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bwnseivx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mpqioeul.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bhpzfhuh.html


<!-- 参考信息 -->