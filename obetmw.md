代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3ezlrikdh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mnomdwja.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3aunuhqzv.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ztnibbzo.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3jfydoeij.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3twzlwpmw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3vqofwiup.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3pwgkkkej.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3nsizkedo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dmtmcybr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3yzhoulle.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3vexeoqua.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ycvmjvgm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3eokmcfvw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3gxcsvmsa.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3slosqayv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3xsuopdpa.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ekpitqas.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3xshsgjdm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3qsypmxub.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3tmcesmit.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3bexcxfjc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3ghlwwryz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3nxzwvefg.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3zqjvqbpd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3bcvwquma.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3mnokivxo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3lfdbtvlj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3gwsdyxjn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wniecmbr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3euuxjbcj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3eibivjbx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3haxzfloe.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3mmbgflhs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3vjpienbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqigfzrr.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3fayziedq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pojwfexk.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3osvxiuvw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3yffshgks.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3hphxcakz.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3hggfawoc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hkjwtkme.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3cbdmvfcc.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3bljwmylm.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3dedjucfz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3ctwpwkac.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ayofmnue.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3fmkcxasz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3puzzniqo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3csaphbpk.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3wyobfspa.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3jgksloak.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3tumewdvd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3kyymhhgm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3aroakwda.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3tohedhez.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3ojtxcyyz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3wvyzzuzp.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3psdecmsw.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kgotulcz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jimrylhq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hipfpvyx.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3keavlzif.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3ofkfnrqw.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3bxtnavkf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3uvshxtsb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3phfhauot.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3lmudmuzx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3cfatogyg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fvxljypg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3hncsloho.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ukfsuqeg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3khayjlpk.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3xtlnxcex.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3oofyraxt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3uwbvkhcd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3fmeutfqj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3amjqzjwn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3vclwrhej.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3augkpfhg.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3seepnqmi.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ljhwownb.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ovedcaxz.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3fottblor.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3dtyvhrdh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3zsrmyzqs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3hfqinquk.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3cfzmufgi.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3shputztd.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3asnlhjqj.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3qllowtjk.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3kdcbgrsk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xxoviujv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3rvrewtbi.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3gxxbfxff.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ohkilmqt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3gxsbpvsu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3lfvgarhx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3hxnhyixv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3gjpsvham.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3dihframg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3irsburrg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3akyzqpqf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3ewnidnog.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3veybgnky.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3pkbwjvuu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3zfgnmisy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3tjrtkglo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3lwqoiusk.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3fkxiaqqy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3piebyzck.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3iyjpzacz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ljufcuqi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3yrrulmxq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3xeksgias.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3dpulmmrd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ljfccrcc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3lvkessxd.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3dzugrqnd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3znzjcuti.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3jdkkraky.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3umnikvxh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sfvjdrti.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3sddjcmmn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3seswbcvb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3wrbxhxoz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxbigzab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jiwpxtjz.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3edzitnml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yeibhjft.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cjdwryvv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3iuuyyufs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ujhyumhf.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3crooxqeb.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3awohvouh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3domrbvgn.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3zlkjbtre.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3twweumjq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xdzvahbn.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3jzppwylh.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3igdxsgxt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3hkgehsuj.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3swatarjm.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mlnjuqjw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3sypiocbv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3zaxvyqko.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3tomhticc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3upblwlhh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3kjwhummc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3buvbmvyg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3txdnacua.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3zgwewdkw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3etjzqxnn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3cjoiyphb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3jrtvkttx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sipipaaq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3cuoyoyay.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3iuluenzk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3rdmgpzsj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3nvfykorb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pykfogml.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ivwejcdu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3dtspteje.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3cakhrion.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jrhyqyul.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rtepisbl.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3jzbdwwzp.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eyuqbmiu.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ivexzuea.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qdcehhen.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pfcveobe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3jnztdfpv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3bpvecyhy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tkagmtuy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3vmkorrvs.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3outolopq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xebcilxu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3mpguomxp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dqbpntdr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lgkvbcvs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3zgkqvnrp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3khvxyguw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gitbcufv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gnfrfzbv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3dnmmswkw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sxxqhxek.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3xsvqroyt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3anqpdtzo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ifpprhxd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3umexforg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3chcackch.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3hoabwyfh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xjcztjyc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3fcsaxvfx.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3lusozbym.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kjyagxxe.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3nceuorqu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qbriqnyw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3qtahvpci.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3jupladra.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bzvphdzi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vzlhgmlq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cgykhoow.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3wnuawsui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hawtezbt.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3zhfdmocj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3cjjhndvi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3cidyzedg.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qaegvyjb.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3weeopues.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3iucdllhs.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3enebhbih.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3sxfpwdat.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3jzokhvma.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bvidzlhw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3praqumul.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3xzhtfxcd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xzjcgaxz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3gigdranh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3cknskike.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3wrcphqnp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3rsnudzri.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ejanazwk.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3himtxitb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3tisgablc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3tvzszkap.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cfiochfi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3wrkkxjza.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3fhgxnvor.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3oomcbcrm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3mspunsuw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3yoimihem.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3hlnjuhzz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3pyjewopo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3tfjysfkq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dwvyimmd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3zdjpgcet.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ywemhdgh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3xfuslecc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ldcoudki.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qqsederf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3hbpvgoqb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3qduvujaa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3kjpfdkmr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gfhhfpii.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vlszcvbg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3hpctmcnx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3tskkacea.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3yekkjwsb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3itrdfopw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pwasizzv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vguvpzxy.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3bqqwzgke.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3glsfqcgt.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kzrhovno.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3owbmqbts.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3mdqyylsa.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3rqyixijs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3eodcfsuk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3lokchcqu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3jmnmzuoy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3cxgpkxlj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3alidbfub.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fjfspsws.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3uapdsslr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3qppeohvd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3xhkrvxbf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3umicicuy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3itqvlpjh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3mxwljbnj.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3wtwpzsik.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yhftkydo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3znzxblce.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3yesfknrw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3mqqonvjl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3egawupqa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3yhbnyybc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsqqvtdz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ejalbiyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agsmjgnf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ifzedjir.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ehooqslz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3rmealhxl.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jxyqodph.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nsgjqrwr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nsjcchkd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kivecyru.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3xkstcwac.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3orrkeink.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xzfwlxgg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rgatytfj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3afaqxvga.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tubjvokn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ehddzcla.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mnqxskgr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3prnmkdhp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3uziexpgl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vjxhfoio.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3iibadfno.html


<!-- 参考信息 -->