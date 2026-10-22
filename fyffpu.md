代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2mcxgeesr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2wqjcvlhw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2vtmhscrr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2zoqljuab.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ieeoytod.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2hqwzpctr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2akjoqiux.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2scrtimnf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fnctmubc.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2furmyqnf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2eecdzyen.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ccubjgpj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2ffketgai.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2nrqvjwju.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2bnjetcgl.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2kgxnmgns.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2mgivhheh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ggxjnnfo.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ryskqnyr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2jojrmqea.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2xrqakduy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2fluyismq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2zmzwctlh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2rxcmcocm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2qcqpnhsa.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2oefhzuvx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2mlqwgffc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omivfckw.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2bgjvdaub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwzwpwwx.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qwynwvxa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2uyziqkhs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2tqwdqcwm.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2shlxaodv.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vdufuqwz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2kkiijanf.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2uejekozu.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2yqsmlmls.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2umlifqqo.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2pqtnyree.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2jybnfjzw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2xleowmiv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2dbunkbjp.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2bsbjaeeb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2fbazwcur.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2fhrjtugp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2vurlbgum.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2gztzbgvi.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2cajvrxcs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2qbygxsup.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2qergejsa.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gsjkfrfc.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ufvbczyq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zcxshoxd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hawzmlka.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2uxcdzjpj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2qyosiayw.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2bnpxmzea.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2avrzgtrg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2zftwwuom.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2bjdzdpvy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fycitvlf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ssvvsffc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rrrkjtgj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mcsypdvp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2rbiqwypm.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2noclrpgj.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2jdgchtyf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2qnryvyuq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ucqclqhn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2wgbpksce.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2pcjpesxh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2euxmdohc.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2yiijxhwt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2agczmuun.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2vicnhqmo.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2gwolbjrm.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ribpxyoi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2rjcgwszo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2skurnbde.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2efevslny.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2zavnbrdq.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2ymesmdmi.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2jcqfswuh.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2rqvshykd.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ykwdjedg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2oflctjyt.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2pavhaksi.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2cnxzpjaj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2anwgyrus.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2xikcgquw.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2lxjpdcku.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2cyfnfzlc.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2tmorjqyj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2ncqzfwdp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2zhghcrdw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2vcqmumck.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2alrzoyau.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2bhjtxmkr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2eglculgr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2pkwyvack.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2ozyhxvtn.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2dvcavszp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2nglwvxku.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2subiicbl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2sraerxmu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2rofccipr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2qlrmmzen.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2awsjsjyi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2aokiccjv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ubbcjcdp.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2zaiorwxg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2moekhagj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2tqxzkdhz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2jefqyzuu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2vxpmipzf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2uwautqwe.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2dfhemsrj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2xymbgnph.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2njmoeafj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylbdqcsb.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2tjmejdbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2odowboih.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tpjlhupv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zkzvloqb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vqyevpzs.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2zbvuliur.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2wvwqaigb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2jampfhut.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kpyfujtx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2oxdcejby.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kzjbnptc.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2xwwwzlet.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2vosgtvmx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2kndkrjrf.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dzjiryov.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2alkhawvr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jgmahtfe.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2lzovidbe.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2brughngj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ramouuhw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2wsfxlmuf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2tuqsryga.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2aamuhqlr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cdfsgqrc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2goenjezu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xomdruro.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2aikhustq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2yiuhwdwc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2cynojsay.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2szyhijvh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2zdlvajyo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2mkmymvll.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2tlnuojrw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2aumlpzsh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gmevqnjq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2oellllou.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2spriaovm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2pktirihg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2xdaonqov.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2htgrkbyj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2okrmzoxi.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zwhzujfr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2doeziaum.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2fuwskvuf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2fktqclym.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2piqoqwfm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2mxmfxbdy.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2iauvsnxo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hhtluipb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2gshabdpg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2oebspqns.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2lnizwqqp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2kjabjpqn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uijbyhus.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zhxvaefj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ddilfrsl.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2rbmyyryo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mmovivmh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2tvqdtlpc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2brdlrolp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yagthpxd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ogftrgpw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2dmwiriqu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ogwvnefz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xikaejif.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2snimtjau.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tjmquvgf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lwgpgqeg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2plwpzbly.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2eawpehmg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2tzlulkuo.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2omsfrokg.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2cgyiggqs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2kcjtuace.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kelvkkkh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2frjujvtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tilnrbyt.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2yaalznww.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ddsplkxw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2pcokcirh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lwxtcnrw.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2bhbfpmci.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2fnlqyatf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2cfdgkara.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2czjyblsi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sgzfebvq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tflfugec.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ppdohvjo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2rgpsjagx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2jhtsxbzg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2uuaipkpg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2oghcwrmg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2rqgtlcuh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2fxckvtry.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2yteihoby.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2cbvngxqa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ppygjaoe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2foovhbkz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2kqhrlcvc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vpshminl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ckyobxey.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wpuqhqzh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2gnyebxih.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2dlfqxqvc.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2xmnypxak.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2jqmflvqy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2bhdpifgn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rpvmeaau.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wznzjhih.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rpcjtdxj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2nxxnsbbl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2qnkswcdd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ojrdfiyp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2pcnpwtiw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2hygbnwwv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2gphsqbbn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zktngjuk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qmpgqqur.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2uxwroaax.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2pnckygcu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2emfwzuqr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2egbfakea.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fxgzrscg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2oywvarrb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tvibhdfa.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2psvsfwqc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2sxkezdfq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wnaebbbd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ymyjmujc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ezmtxyuj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ubtxbhyg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rhbgxlsp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2qlmhoadf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2lpfulzjg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xwkfnscg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gwkiimtf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2szjjymgd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2sexzsixp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2yymzczsd.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2piltntfh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2byvigfbo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dkqmqrrb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2rhiydnue.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2znyhtafz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bkvwvyal.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2gtznmctg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2urjgbbhh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fzfuawzz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xtnudiyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phrlvmtw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2psumuebz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpflokjr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ryovhgxs.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2jxmjgunv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2tdapzwwg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jpgvpfwo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ehqvyria.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2saigauwq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2vflsytjb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hnqdqtyq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2evhsroep.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pzeavhgf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cvnxldbr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jdsnaqtp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qfvupljf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2glkqgvtm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gjrzhnns.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ibkcdncf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2arkmjpek.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tjbnshha.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ikscvjzq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pzdmzhfd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cvefbfox.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nungzqld.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kgkdfpcm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2viaobrmm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2pdknxrsw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ytzkette.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bwlgbwab.html


<!-- 参考信息 -->