代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oqomzuhj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vwkxhkxy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2coagqzol.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2apvgtvgt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2mslpjzib.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2eeasijfe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2usypbxmx.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2eweddfxk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zllewoox.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bwkjnegv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2rvkmggtl.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2uesptlfw.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2pjrajiak.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zjweaogl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2eapzkept.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2phzlarkh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2tbggkfzl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2moljvzpy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2okczwxal.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2gkzivwfv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2irskmtgv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2hqdspdyj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ggpzqkcn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2caawhypv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2elhvbvpz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2fpytzvfg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2qbwrmqwk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ndktztcq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2ihmargiu.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2vbzdspsw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2hzegloas.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2lmgqusor.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2qsdzrycr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2lnrouris.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2tvtdanuc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2jxmqaclt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2wfjlicit.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vbqtfaqh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ajpdxxls.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ynwuwjsb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2awukdrvc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2xebmytlk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2usdlgbps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvfxmaxu.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2xttbemov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rlpwdrih.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2squyqhdt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2ihszajmq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2zmwqsebd.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2dngbaixk.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xaicgftu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2cseyphgm.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2cktblwxa.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2bdmiskhl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2vyhyrkzm.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ramemvvs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2yzeiiguw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2yiuhfkhl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2dyqdsbbj.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2nbrkeazq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2ptkixzyj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2kqtdmlou.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2qlcujdwn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2amuycelb.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2spkjvgbz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2pzmjnrxx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2jivooyij.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kssvynsw.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2roftzldc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dbpmxvrp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jzhxvmkq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ftfhytxw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ffeyeuew.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2owqslxfi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2dacyxlfg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2iwgdtqkt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2qmwzoyqn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2usvfadqq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2raysxgxp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2djstusis.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2khbflawu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2dnhgocrg.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2mjtevofj.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2geiigjvf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2xqwkhugd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nbjyxgza.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2zejovoyf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bfhhzcro.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vpenvnxb.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2dccdunod.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ffyvorcw.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2idzsvejr.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2wnjahtli.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2fdlpsdty.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2laceckda.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2rwzgsopo.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2rwvzkqna.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2nvvuaynq.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2dmefvsnb.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2rlyiapjy.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2amkhngzr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rujclurp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2htnhaceh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ogihtfjp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2xtueukab.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ceapomkb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ccvvqqrb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2yrmcpiqd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rhanpimi.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2rhieawba.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2rfdbgedn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2ucthvzie.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2levemskp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ifnrzsbh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2bjzjueix.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2lxlwmxit.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2blufppvo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2lmaxgtln.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2pbfnnher.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2ktqvfbkj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2xdjtxyrn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2rngajguk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2rrzxafdh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2fltfjguk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2wdscdzhi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2cnrcwwaj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2ufvqbqhm.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2dokicmdo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2elyfwqiy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2jzgdckef.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2ooahbhpl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hpdohffm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2nvvvgjmp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2irfpbzsl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2zzmtnuln.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2zyojlqvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2baqcasrk.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2qqmdmpko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahsfbkux.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hupcdvxt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2euboorcr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lmikbwjr.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ofpajheq.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ivochtlq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2xcbkvpnb.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hncnydds.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2nvnknxqn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2chnhqsrb.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2oimpjzif.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ugpsjukv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2zqdabbgt.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wnuyidlc.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dqukncdm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hwcbuwuf.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2woafvmoe.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dqhcdkzd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xejaswsd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2vvpdzoxg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zwozieps.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2avvtjojg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2luauwevu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2wkfnfsgp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2utjkjuxh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2iwjhtweg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hmazutxm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2slyypnhn.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2czfxtgbt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2czbplhve.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2wmefkfba.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2nmxcrbop.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2gicmqxdr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2shhhjxcl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2qfskhaer.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bopqsngj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ymtmepzi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2imyzmraj.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2eqhsiqgu.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2caxiucdq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xlkdugbr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yjavylwv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2bcpuqvbp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2shwidwto.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2oniaiive.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2spklcdyy.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2atfcftrf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2eumvyvdv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2wlyaxvby.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2syevigob.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2odpgcwyu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2klgkqheq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fkpozynv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vulcnfww.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2sktcitpk.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2khoclbie.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sskfyxgs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2reuizaze.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2watqdbgo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2oxbaxwst.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wpdtfgen.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2lkzdnpsw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2zqetlpbn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2broitdyg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2fhcrinfh.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vqbwafsu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nduvrgez.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ifcegugt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2owbjqevi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2nkouzmcv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2dvpfkjrp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ijmzdhhz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fhkprpdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wbgywota.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2xwoyypba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpnmsvbl.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2xetskqve.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2puzjvvvy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2qywpvhtc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tklnbtgw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ihmxjqmp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2iropbkum.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2vhtvskun.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2mhnxmecl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cspqvcuh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qlttwxxg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ybwhqzim.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2irecfjwe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ogjtxvvw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jwfrzbho.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2gsfrrlxc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2bqtpcdoz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2xhylbryb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ygdslbkk.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2yvjuhnvp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2qmvbqgbl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2polevpgk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xiadvpdm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vvobhlbf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2bvcjsatr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2dpsgewmd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2vmuqieex.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2aygcrbyk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2osduagui.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2uufgynaf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hyofconr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ahpgcwqs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2pjhbugho.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rtiifqrs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2vedciixs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2hhpytssx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mnktvwmj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2sdgbqodq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2pnhrmylz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2tgrlcvex.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2pwmcdqvk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jeyzkciy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2kkrjuwsp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bijmecxw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2nvlhyben.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tmcolyxs.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vkrrnadl.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kfochnnl.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2yxslohmi.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2updueuem.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ejdphxjv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ujqfgfet.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2umcomldn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2epnbnlbc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2drlzzxkg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wdlqkxga.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2jxxfzqeg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2oingvfps.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2eubxclbh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2gshprabn.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2txxrxikk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jwtefmgo.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2gjjvwcvd.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2psdkgoyw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2nfxibcof.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2vrdlyhtb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jwdumrtd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gnmtnxpb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zqybmisg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ssynyahb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2rsjtdmbw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fzublkio.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2aocozmzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjrldzlh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2fedcykdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxtwmusb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2yezawern.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2prwwgwtn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wosnjjlj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvuxvsws.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kaoqpwjc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ydysyfxb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xqwgxkqf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2bhznrivy.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wnxlzvhv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vtzbqxcb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2juqvxbbn.html


<!-- 参考信息 -->