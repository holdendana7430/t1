代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2fsmmmexk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2nlpwhqim.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2mojnzerc.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2nzcyxszf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2taqnpley.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2webkmflf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bytkxpng.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tjoxsjlk.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2spqddwzw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2eoscepxt.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2drshhphp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2sakqxwcz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2zsvpvgts.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2tjvjgtpb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2fzzjapvb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2djpmfkvv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2jqgpyxuz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2eyrbxdeb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2fdxqpgkt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2aevwwqrz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ptevqfzf.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2wtltpguh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2rqnimxdr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2hxnxrpyn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2lncndiov.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2vvdojdrg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2boavmlqg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2diojgmio.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2gxzhxvoc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2eslmnfgv.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2pdvcucoa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2vspmyqbb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2wnzsxrka.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2dkzxoisg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ogvglthw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2rlwnhkut.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2npfailpf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2rthgayoj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2tiyfdpcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmegvrrl.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2kxcjyrih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yklhwztk.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2uplycony.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2ogqvuewx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2sdhobbuk.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2gnmzsfow.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2sbjfqsjx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2uqtnxxmw.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2zvlmeisk.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2qlgfyjpd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2bimoajht.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2tnzfydai.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2brgnjmwp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2kgnhugpc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2xlplumpx.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2mjvmovfr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ffntezcc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2fuyljmzw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2cmssfqcc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2wslcekzj.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2wnsymtdr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2wnebqxti.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2imfqkdnc.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wgnawsxz.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xtmnrqdb.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dydopcau.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gwxvmext.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2eubwifgd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2sfxfflyi.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2htboxzrs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2szfitmcw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ljexhtwd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2rioepnge.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2sfazjymm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rjekcvkl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rrppwvio.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ghmjlaxk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2yuhvtjmv.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2vxalvfue.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2rsfhggxx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2dtwtxrof.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ppnnqerg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2pvhlxxix.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2bfbcrdbc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2njfsyllc.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2tvmsitgz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2wgvrqfiu.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2juzwsmsi.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2gvvbxhzy.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2jazlxfqc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2xltdstnq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2lsamoxbo.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2jptnrgfr.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2gxzqjxzw.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2dplzrako.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2jhrjavmd.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2wsjuxzmt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2zaljzcts.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2narykgke.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2kgbzqcmr.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2omipnqph.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2xhufpchi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2eznwbjdb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2xnauzgoj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2uwvuibvi.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2lujmodng.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2jhtughut.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2rcbukmew.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2fqrrqyst.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2oembmsfx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2qkxhqmmd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2sqqqjgkl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2aejmcjqm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2xumhgpzi.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2rrrtfrps.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2rgislqav.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2lwvsovqr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2csqewzqt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2gspdslvw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2bozvhemk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ermhcbcc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2nmgewudl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2jzojssag.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2txmytxmz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2mspytwyl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2uurwxopu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nhffactz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2rlxaqdnh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2odxlmxgd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2tjpkdekr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2bpyytjqp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2sdeyfsco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttofmkwn.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2agpczikx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvyxvgjn.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hpxsqfng.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2pnncpcmy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2rbuxpqhz.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2abndpvag.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lpvzvlqw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2rlpfptuj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2buekzdpa.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2ckktlgkg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2udmtgiuj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ilxizaml.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2znpescqi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2ivpewmde.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2whpnyiec.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2exasxvhj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2uawcghgv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2wwhhzdqv.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2qlkzgkvj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2udxzvcgj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ajhbstax.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2rpmgmzzo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2hiddvdhp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fiitevhx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mxbboglf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fsbevoig.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2eqepgoty.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2kddxbcbo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ucsyxtpl.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2zuzufcve.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2kjebfpnv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2obggostz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hivudizi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yisfunxx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2yuwgyvsv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2loczhufb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2nehvlnwc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mztxynyn.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2vpeociod.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2wiixjzfg.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2rhlrjbeu.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zkpsbchn.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xwsthdgl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2kufznsai.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2hyusqpti.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2cflspcph.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2odhhcajn.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2vvsvwawf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wdezenmr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2xrhbargf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vyqigmzb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qcwzawlh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2vrflcgso.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2aruceomu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jwxwvfjs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xjyzrsga.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2uqolzhlq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nvpqpbbr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2shmncvyw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jeepfpfe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vusofaem.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wftumiim.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2sxvmxjuo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2dsmxxqjw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cemeysqj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2mtuimnjl.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2qeyjjhwh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2efmbyogr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wdlsnoab.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2bwwctvsh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ebwxgwtv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2iuabymnd.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2hifsgwku.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2okdphfeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zprbfjmr.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2omijnqhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qntxgzgd.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2atxoxijj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ygftxzoy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2egenlcvu.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hymeioen.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nnyxmlbb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2euwfstoi.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mekowoac.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ncmdrzlh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wydssvog.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bguomgsa.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2rkikfpqp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2jkgiubpa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2bqhjqxxe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jnwdelon.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rrisvxrj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2lrlzjgtp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2nclmkezv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tncufcpi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2vkkquieu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ficyiopw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rvilqgka.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2puawoumm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2buychinr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2oobccboa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xstibayx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2fqhnldvh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2oldjtlzf.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2hnqboebn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2vxglnxzl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2utumqprn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2cdczcxpx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xsjrjaai.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2nktwapqx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ttgsgqmc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ykyjzmxp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ldjtnkem.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2fsagofoy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2hkyhbivf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2bcdsufxu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2nntuhsua.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jwuvdnse.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2yyzgzbyh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2gchfjlxl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2zjlhjuzx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ooarlkze.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2iqeubqkv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2curksbvr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2wzwkezis.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lmcjedlb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yhvkasfn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vbaizgfc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2vecvavcr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hygsoyet.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lefxiulb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cwjovkxh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2awdnwzwn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ikhqhdbc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2iwgoduru.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lnkkvyyq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2wpflpima.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wcskzsgn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2olcyhaxh.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2sepictof.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2hozlroxw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2cknspydt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2dkodsrnb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wjqyykxa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jbtzjbmw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2zpbjasqs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ogzjccbs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bkokzqgx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2drqgowzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lffrnzpw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2korqftcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lckvguyr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qlmbtrjq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jusypvpk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2tvyrsrlr.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gmrtfyfi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2duojbwgx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qhtracyb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2pijoodrx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2pdefaglt.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2vnfmluxl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kmruairs.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2avquzbsw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2stypnpyb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ykuenrdh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fpnffiic.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nrwxbygg.html


<!-- 参考信息 -->