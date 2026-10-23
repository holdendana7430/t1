代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zmqqpymf.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3mmuiqawz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3xqzuxvil.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3aqfhxsjj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3cqzftvxb.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3xngwxqot.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3jipwddkt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3yemlulbp.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3wkbqrmeu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3mzvqsmox.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3ttjmaquk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3xdirbtzj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3cvigicwi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3hdiwfsmc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3hhbbfigr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3lcwsjxvx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3kdrxujod.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3zokwagwc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3vjjsldkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blxzmxyf.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3xbfjhyfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yclqqgdt.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3taligmcj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3wihvyynz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3iveqvcua.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3otjqnjds.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tjkssiyq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ctgnlmjo.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3qpgtrryt.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3qrxhqimy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3skmvmjsu.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3cvdauunr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3qyxfnjjv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3fgpgpdng.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3tnhggnfj.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3iqmublmk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3taurbtxk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3pbpllntu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3pyxvmyvg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3ztkqkhsm.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3podxxpgd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3pxxpsyar.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3tffomcru.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vlelmqfx.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bsjvidkx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kbqbdoof.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kbqeoiec.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ajrjwptq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3bmjmppcw.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3grhnnclr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nlaooyct.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3ypvzhfrh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3qiydeojz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3sixbeiwt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3hldazgum.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3kimajgbp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3azsgbrgu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lhqfudey.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3jxvansto.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ufddhtbj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3igjslrxa.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3sxmukmhj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3mtddkrfx.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3twuaqwru.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3avarcdpl.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3etzahune.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3xrxxnhkw.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3mgwjmhvr.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3cctjpmgb.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3iunenmle.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3uabbvxqo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3qlmekqvs.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3xladwobg.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3jnkzxqcd.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3mjudiylv.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3jmbeifwg.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3twtmpkfm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3kaafjmbe.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3wgpbvdft.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3pqpfvnqu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3lrofagls.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbdczvey.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3wijyxspq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3apawsffp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vdsbzjrt.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3eyosmtfz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3afzxippx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3zbzimovu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3xwawvlhe.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3nzjjcapl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3tcazwvyb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3loblnfuu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3yiygcipw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3iyvdtloa.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3ilegvsmy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3yvhigkqk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3etlmmnsm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3vkhwpeez.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3iuejvtzs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3iqztxahi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3gzxrstqy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3srcqlydo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3luslxmzo.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3dprpkoaq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3sapqizca.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3jqweavzu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3owvmzqoc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aybvvmrb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3uhqdpnlf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3pmsimxjv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3inptthvo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cnvrikwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cltlwrng.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3uoetundn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwjjaxli.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rfgocriw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3fahsulhj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3kowepufm.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3epzwicdh.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3nfzgdxto.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3tpuqbkwd.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zndbpvfv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ifdyhhqc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3afheastu.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3jwcjjklv.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3akpbhgbp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3ffnxqled.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmxbqge.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3utakwxol.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qrvxxcds.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3odlpgurq.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mtkdvpdq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qjngwsbq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3tffxsemt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3hlrgapqq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3iyagpawn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sncnsbzf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3thukgvfe.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3xzizopmb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3qmpydalp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3kbsutwfd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ajcftteg.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3iaaujwkp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wiragadg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3niclbddc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ntyjtwdi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jzrtfywa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3keohkcxo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3bixmkqhp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3efpacuct.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ihnqmiri.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3lfipdxqs.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3xmbtncwm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3brlqzgiq.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lluwoinq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fiedmpch.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3gbvqonna.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3oousmyhj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ofpggqaj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ahlpzdzd.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3lwdtobxp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3eljhjqld.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3hsxzwljt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3hzkufbfq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zqzwukij.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3hpwvhoib.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wudzerqq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fgijvfgd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mozakjiv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3fpvaccqp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vljibmrf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3fzloefbq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3npxocudz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bwgbxent.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aevhkuvl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3pokdkufp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3fmgdyzzx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fplevhnx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3smmsldqf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3stdfhoos.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3clzgmdik.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3wkwovomm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3avucynza.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ngvjkvti.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3embxhsmc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3wqocsdba.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ayvyxmdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jllxsyov.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ntnmxugx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iliqgbko.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3hebeexgy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ktcwwagm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3lkeoeofz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bipbneyi.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jplzxfgw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3zqkxtgfd.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3zbqdpkjl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3eueavssv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3rkdjxpqh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kobgbuvg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3iexosije.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3tmhcznqn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ohynulot.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ihwpfaep.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3cttmtvqu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3khawkdws.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3uplljqrv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3udcmwmpz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3zypmhuzw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3giitjonj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zubdcfpe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3mdaoasej.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uwyxgxwy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3tnexedvu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3oaiencis.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3kvhyvvri.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3jsntmvpo.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3msszshmf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3uoopoqln.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ybccijlo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3yflvlexl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3pjmnwwsz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3heuxfhzc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3gjznmycs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3fxovtzxc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3sfduuohy.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3vbypkhrl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3jmovblol.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3vsiffnnr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lqudzasr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yldsxyxp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3guanrele.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3yndyzuyl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3eheuyhjc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pkqmnmdg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3vwlrvigq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ihqxjpky.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3xyewbdfb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hdtqzufw.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qsyxygqd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hfuzqxdj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3zbqkpjgp.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3fiikeeuf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3xdicigro.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3htilhgfa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zlhevskk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3tvsydmbq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ggrhiniu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tggfxfgz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3mbyqxdzl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3dkxogems.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3odkzszen.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3zwuueyld.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ncpyzjrq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3rbsewhxp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3fzemgcgt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3plwddrdh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3scqyztez.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3gzyzanet.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3qlkxspaz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3lskvpjwy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ozhunxqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tarxlgpu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3xsvtzjng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvbymnix.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iwiuaaon.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3utkgwesj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hvgnzhza.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3olgtlvyu.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3flrlqfpb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cudzjxva.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3gndqyujy.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3rypfarmr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wxzbxkxx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jdscehit.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rngvbddh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hjiymkdl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wtcwncyd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ebrzzayd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3iixopzbb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xfutffor.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3tqmzgxhd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qvgwfyoi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3afdujrtg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gxrqsjtc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3mfmysoke.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3pyiuvqnb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3lydyfzny.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3thzfqkgf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ekvkxhnj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3dcbtjslw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qlhjjebp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3oafcnqxi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3smdfwnlq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3lnsghlua.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zvywremn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hdvyfceo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3udzvlwwj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mtztkjkq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ixydcnhv.html


<!-- 参考信息 -->