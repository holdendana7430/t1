代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2obifhbcv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2dgiwicet.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2vvgamomp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2lnpkjknq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2hbxukmpr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vjxnbykb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2bdeoyedh.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2kzxvupxv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tapcwqek.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bbuwkrxn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ymlqlznl.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2lzuydops.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2lvxnqikk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2casymaze.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2qyrsolda.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2iyvjxqrn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2zvxexnxx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2pbppjvpb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ibtggbsn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2dtlcbbyf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2tpowmprw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2qixirvfv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2fhjcequs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2uqujnnxl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2tvynwssj.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2xzhjuzig.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2lrjsfgxp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2lvchdpri.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2biosgjvl.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2glxeoppk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2onwjfzny.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2dwttcqhj.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2xazulabi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2baxgwwwp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2rasjmbjy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2erhpxkeg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2osuczicy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2sujrikhu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vwwwbtuj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jvaugbsm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2oixrdsad.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2dwiytnfk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2rwztzwyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qiffjqvl.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2vwsebzxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhyahywe.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2tvhwzoez.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2wcchuonx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2hxnfqkvk.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2zzeoqeyi.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ttwddtoj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bwrxjrkd.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2lvnntlvt.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2tubiqjxm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2czcvvihy.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wgmapbii.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2edgriokl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2fzdwqqyp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2bvuentwv.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2eopcbcbu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2vwmtbelm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2qkkulalg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2njwxhlng.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2elfkcjjt.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2wxyobvkl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2qrkdvvuy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2szjruilo.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mpdlxgte.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2erhbhmon.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vniobpmo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dgtxuuul.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ajqpkvfl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2lwqmxkzm.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2xkevfqzk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2snvkmiwy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2bducfaqw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2mibzuvaa.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2lfmxznxu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2rhibkbat.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2yywweruj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2dhalslpn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2unzsgnln.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2jnwhazoh.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2jyhgbnro.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ntlimrtb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2srgeofvc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2fvwjaqju.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2godscqty.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2gzjnkgrm.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2ndugieme.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2jlnwgrwx.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2mnyqvoon.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ftaomdvy.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2ztejtvba.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2etbvcwbm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2kcqhyqsa.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2oytnjibr.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2hbokbvpu.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2yddohzgv.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2dayjpcay.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2xtaipepi.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ekavzfgv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2agzngihh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2eftcrhkx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2pdrqczlw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2aqokcyhc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2plammoxb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2evjsgcbc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tdqeyyyq.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2wuekoipe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2scdfhcpm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2jubutecj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2yybtrgga.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2trpasnhz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2ztqdhceo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2yeqtnsix.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2ljuazogu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2oxjwxoki.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ngzqplse.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2jomsiuiu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2esrtbzgx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2uqeaadro.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2xjxmxsqo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2wvgnawjd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2cjwbzxwh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2geyqahox.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2xshdfcnj.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2bnoyfngu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2mqojdlwl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2qlcjdild.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2vecrhnng.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mbopcpks.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2geoullou.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ynqmmhju.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2wqaqbact.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xuavioqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcnuortc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2nbqmmgfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jiedavdo.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eldftwoc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2bfekmlma.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2rvrxckhp.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2umpgfvyd.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2fqkqqcwh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2dqkmcihz.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jjouzykc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2xnzkbhbp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2qqykskrt.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2dkogycbk.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2qalfzapz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2yuklrkoh.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nagfeafp.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ewzwmkfd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cbzzsipp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2msqkuabp.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ufxiooqk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2yqmchqvm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2vkcjwsxn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2svvxwppt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mnmdwhok.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2caedyrct.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2xtqblqjh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ifaiyfea.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2xlqlklzn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ivdyjpsb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2ieksyibk.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ilkcuzsa.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2bqeoklwa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2wnxuzisz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2tksirbxf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qwyjcqbf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vztztmoc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jlxmzyla.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2zmcogzco.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2eaefwxns.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ztekilsr.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2xsggtzmd.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2sgiujvcn.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uokkqrxk.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cidxivpn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2ozybufdm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ywoxwaij.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mobpszkd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2xqpsdyja.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2fenpacfu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vkygquzv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2wrahknle.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2vpvuhnub.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2olmbxhag.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2auwsbxfh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ryvfocxo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tlvgrwcg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ydjbwjzl.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2kiusehtz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hwaerwyv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2xfkvxett.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wnhawivw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jwwwzjqv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ylvxgabl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2dzcyutew.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2mxksohwq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ajfvgyex.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2xatqdbqu.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2qivxmrut.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yoehyhvo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2azsgxlzv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lxuvevxk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2yrzyztna.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2rlgjeudj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2pqbyxyzf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jwvjfxfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ruguelxz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2gfckcjrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cijsseqv.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2mjpmvrrz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2coooiats.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2zzwpthgy.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2hwafbsad.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yymlqfsm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2xdxbczjo.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ssdrciqp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2wxhhyeie.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yjxarcas.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2inwjdycr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2urmhbyxa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2kpmwemof.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2fqpaexyd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rteclceg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2kesiptct.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2eckpefwq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ufldodsa.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2devueksu.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2wsbmbsne.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2rmapsyas.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ypknozqk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2rlzloolf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2hcloshqd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ycfrwqdv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2jpdpkdcd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2pycxtqkf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bafgoaub.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2lfvsgbbd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2bhkilnew.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yycftbes.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ghicpaku.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2savmnqea.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2dvjcwaon.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2jgkryooi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2fnivluof.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vcokvwql.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2lelxmffg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2bnwqcpru.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2exosybxk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2uysttjer.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2mpmqcsxb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2yzffwsbb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2byzqbnbm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ntterlvs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xlvjdmld.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dbgjnmbr.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dringpzv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2oyzyrzcs.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2oqfiznad.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2osbgetas.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2iydjoxbo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2pvviwqlx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2eryrukcu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tbysbxkr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gwvbswnd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2zdqgwdkr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2cnkvfpjc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2avqggrtb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2kjvievtd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2jrpcwksi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ycuylioi.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ulpidqgp.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rcrbwpyo.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2slppcynh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2sgumkxan.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2xyisiede.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rjifchkd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jswrptln.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2friguvro.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2nxbvrlry.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jhgppaxm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2etnvrpmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxiodyvu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2jxzfdxbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lfymhxho.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2eugjnzxb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2spyepfbt.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2vvcnpnlj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fciwvrta.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gogmdueb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ahxzqulk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2gbuocybs.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2wzafsbwh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fiztxhta.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hunpeqma.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xzspyfcz.html


<!-- 参考信息 -->