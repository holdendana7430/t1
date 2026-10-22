代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yjefgxfa.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2usvcjadc.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2quwbtijb.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2sltozzll.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2cyikxawf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mjpxsbux.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2fmblsqgu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tbmixvzj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2jtqigywb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lzepslmk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gcsthphb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2kosakxog.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ictsdsui.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2gbaqlqdl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2osuvzzji.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2idxyhjnp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tltfeoie.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2qpjstxcv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2dqrjkste.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2dpqmoklp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2fozpmvsi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2vwursnum.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2mqeoocpk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2efebxpiz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2cgmacnlp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2dxgnztxz.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2rbfdrgjq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cjadlenu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ofyuiihx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2rhixjzoz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nbxpfogz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2kofblsdh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jejvyapp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2gslvyufu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ikelcdqa.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pqpkinok.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2zrgggavb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2axlduoxh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2gbczqtag.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fgtqbezo.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2atzivgcr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ofijaavb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vvellvlc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2mijgmxne.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ptnzbfly.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xtkbrbrm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2egdphdrw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2wqlvclul.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ebiphqyo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xkburykg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2jetiuytf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2tlfwtqgs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2uwminhrh.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ownfjqsj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2vrzithsk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2nzdvpbuw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2sjankyot.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2awfbbxxo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2pagshyzy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2ebvrupby.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2zvtwqoyk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2pdlteupg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zmvxdkwv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2swnagoav.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2puajxmkf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ctzrqkwm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2umltwszd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2rcgepzqh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2sbujmgbb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2krchpwca.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2quwioabx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whjctnew.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2kjauxnns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ailavpmk.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ujmoeyqb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2hnyceekb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2arehgsbp.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dkliiphb.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2sllzghma.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2njcqenma.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2qgkrcwfc.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2qdxgpyjy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2mocevppj.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gopsczpp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2dysrzyjb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2opluzdnz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2hgkytgdt.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2dlaandhq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2hlunrdpo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ysirkrzq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2kdqegmhv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2szamsytd.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2zndlguxr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2khbvvnmn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2encpxwgz.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ycchgqzs.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2iiieiyhk.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2arcecclx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rbigqetc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ykgqeuls.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ifodjcjs.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2egzdwzis.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2twvndcdn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2wabcavav.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2jjnqfmdw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2wqjhbmbw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ploxdyhg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2yyqytcsf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hnnukirc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2urhgmplv.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2wsqoncbx.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2vdvnkehx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2qyqebuhr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2nsvchnsn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2vpnurjop.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2nmuuwlrb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ejutwggi.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2kujftkfa.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ordhneqf.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2uerhzxcb.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ffsfjgye.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2ezrflfwp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2womuqada.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2xisbswsu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2rfkviwsd.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2hxehhrsm.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2qqxaoumc.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2njpogotc.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2hjcdsliq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2lqframmo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2gjzttcxa.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2maycywxi.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2oakvvhpk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2hhjaarxn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2qlbuvjgu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gxghoaxl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dtlynedj.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2tvqykoym.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2mgjkiocj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2xjugsnly.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2sqfhlqlw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2aqiunwcj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ksfylzkf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2azpsrdda.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2sqipfsde.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2xqyuwyhd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2vnsvomln.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2xuzlofmw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2qyftlzrq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2svormzyk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2nvdyazyg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2kwzpyhsk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2jhokdivy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2jvojkqdh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2aqxfkbwj.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2eymijnfy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2gvziomkg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2vitxpjim.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2umbwfgqb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kpkipdgy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2vhfecckd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2zpldacit.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2vkwqazmf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dmeqcbud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yvgkqoih.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2fwmcrffx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vvcjyxvt.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ggzkgzhl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2puzahbme.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2hsprjzhb.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2mcdsapax.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2osyppqes.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2cmiefhlc.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cdhtukau.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2vfsqwfbu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hqeompot.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2pjmatcdz.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2zgxqxfmz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2wdtklulc.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2auliytwy.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2cjbxhmma.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kllyjipp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2xcvdyykc.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tlwbxeip.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndvynxbd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2vdduiwzd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2txtjxknc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2dcfjjvfa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cxbtmdfd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2lurvjjkx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2duiobbdh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2butxztse.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2elxnlywp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2ehikfwmc.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2xsrzrybk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ikkvhiva.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2tedtckvt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2prkackww.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2jthmnmuu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2abrdagnv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2stoowxzt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cvmsiokx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xustgdad.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2nttrjdpm.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ynmoikvy.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2cfwpwnan.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tkhzpaum.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zeqprqpv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2ojhxobcw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2gqucazmw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ufkrtqkr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2cmumimml.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2aeqmdkss.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2sjsulbgq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2cabetvsx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2pdkcnqic.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qokcnxbf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mzquehnd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2imdmzwpa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2sqmjdpcm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2plseafdq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2rnqbaggu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ukhlwftu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2nioqzupn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hfjxwdnv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fgqmzgrq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qlghbibi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2imnjwttu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2xxqgtixi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2soxrzbqp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2zydtabbe.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2qoocqwqt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2szdyfzuz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zaxqgyyc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ncktutbi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2rblnhrkg.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2vlvsojun.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2kbjawqwn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2yugbynld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scoadrwp.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2gfdpvorh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2prmzrqec.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2gjuqlybo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2adeajpmz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2eoxtxdrn.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ekmkrvck.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2epdvmttl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2wadtxwgc.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2bhkpeofg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ufrjzofj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2yukmcyqv.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gfdilniz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2vheihaul.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ugdujzwa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2yoeerrsg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tckyxojb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2njmbsymf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2yyxqkjep.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2pbnwsrbx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2jammjtry.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2tmptqnxt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2odlwuhjt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xysoucef.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zvlfvpst.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gdchhgnb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2zeoewnzw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2haoqqset.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2nxxdcfvm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bjlhtntr.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2bjjkrukn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2hmcdrsko.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2cohozrct.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dvxycxjp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wlmojzad.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2kpmoqkho.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2zcuzkohl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2zjpgloql.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2naamqjmz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ofdqfmfq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2xactvmuh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2xrfspjqy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2nfxkloab.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zoixbyvp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2tpvczwkm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2iicrxacx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2xwtyvefy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fosgyutr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2gtggfsbw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2akzlojnq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2kjvottys.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mwhcbkju.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qjrukigc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2smrbeody.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2bhedvfeu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2deoppumd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2cqvctpem.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2dvtnptcy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2odbgbhvn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2jrigpudr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dwupctvn.html


<!-- 参考信息 -->