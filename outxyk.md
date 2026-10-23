代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3uxpjmkys.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3qexwjqfo.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3byzoxuqn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3allaxdah.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3kxaqiatc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dpzpybvp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3wreowfws.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3wbemhsrw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3idachzrf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3vvngsvoo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3mtznfypc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3qxhdrika.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kcvawdtp.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ilvfvvmx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3xtmjqlpk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3hppayafc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3lamytqbx.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3vqelxsqj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3uoaednlo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3ccoraemd.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3duqjbqvo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3wrxgcinj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ivqertnf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3ifmkcovj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3xhfkbuhv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3pmcfluso.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3aoepmvkh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ysngkvea.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3eeqyjgks.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3lvogxljh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3usfoenom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qyxjiyjl.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3zxbgrjuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jpkmjztq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3ulylingp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3lpiycpbh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3mdsgdxmw.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tgdcvdwt.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3qxhfmlmy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3rjcjyxzn.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3iccobxyf.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3thnxbtji.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3dbteshvn.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ypprasjs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3rgumqyjc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3volcvfkj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3xwfahivy.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3yoyozlui.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3wjsvgojt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3rqtcjruk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ggqwbjsm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3pmardcwz.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3urxmxyrk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3pawzonjq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3mmplomzb.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fjyvukzk.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pgrmjpwc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3yssawnap.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tcwpnqzw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hrkqfmjy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3qbhvhnoe.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3uamagysi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3muoknegu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3xncfaqiv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3jkiozqkv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ijwyrdla.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3lalgjhri.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3zxbsioss.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ndxkoccr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3shblxeip.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3soctvrqb.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3smdmvxod.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3rmccaaoy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3yyakvkpk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3nvharjwf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3hqhsgyfq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3czjspmqz.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3lhmerxfd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3pelfoici.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3jwaezuct.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3khytrewj.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3vqqudlmb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3uzrgqxck.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3jndaavls.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3noxjupvm.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3eaffbffc.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3fwtqulng.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3mrtzwfze.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3lraprcnd.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wfrhnrhh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3syzuqdyv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3qdbzfqvd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ujiiiizh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3siyrpaik.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3nqgeeemz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ustzuayc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ignhbbdu.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3yzjyfyeb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3fhmkdowa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3jgapqbbb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3djyynrjn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3syqpcnha.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3onfljruu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3kjsdhsyb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3flucnoni.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3mobpazrw.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3lmxcngfv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3sbrfzdof.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3beagkyxo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3qmxxdkgh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3yiqzjtjm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3qwccdbbj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3gewzmdjq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ixxnspyp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3zkqzufbp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3ymuptjqx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3xjjtobac.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3gbczikyk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zpqitlmc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ksylrhjb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rlobdfri.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3ahwyegpk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3mwyhsqxh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qjfraouz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkhkvkvi.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3mqmlvfqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3szlebeni.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vxasvomd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3mfdxzvio.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3kuswjfma.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qjzqgiky.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fankfhyh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3eimpfoky.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wfhwwzvn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3qvfqwlrw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lppeyssz.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3nbwtrseg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ivyhskhp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3zhiqvmow.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3euxfhpgt.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xzvwvekx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wwlcfpji.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3vjpsejgq.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3evlzjphm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3spknzgrv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3zuigyhhd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3azxizpdm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3jtorrhtx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3njjjzlnx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3hmnuaijv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3sfbyclxs.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ksyazbbs.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3axqealxo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3wgtpyfko.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3decztqce.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3isweigtg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ybjgjtnw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3drmxmutb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3krogaxlj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zizazxvk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3hhchkjlj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3izwsjmvo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hdaadfet.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3zboiihhw.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3gggzhgei.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ipxlndkk.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oxyvujdo.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ylzmckgq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3rfxvwmzt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3imayxcij.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3zgihfkji.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3sgxabqur.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3voioucuc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3dwlrwmaf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3gzktsaht.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yhcxujpd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3uzzmhlrj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3fswodgab.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3iqymvjqb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3yctaihno.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3myofpwkl.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ufzhmaxu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tsyiflmx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3brxrntev.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3guspwzeg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vklyskuk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dfmmkeos.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3vmthzwlt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3tgnznwli.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ahgmqezp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3owzljsqj.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jbkatoxq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wtoxvbxi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3sqmcyaqz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3fxruuhao.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3itelwqon.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3nfcjcrdc.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uvimqxvt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3uwisybez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbvbttie.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3wzlzyjdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqplkucl.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3hpnkzbmp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3auhzozow.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3myvddqev.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ppirdbiv.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qvwrpwuv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3txtgswit.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ylrnixws.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3jtfwlrmk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3oeadxzxu.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ruqswfkn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3renjutcb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3tkotzryo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3kogfwpmh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3eydrmvbd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3fkjhptoh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3artqtgik.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3hatrtkya.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3dquqzlob.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3lhoyqebq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3pzupfmpg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ogqgyagp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ksawcasq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3oyvybuze.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3vrzviufq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3knbvqltv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3lgrpyfup.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3jhqeybml.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3yztluquo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3eyltehlk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3tdathoao.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3swuoycby.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3emmbkfbr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3phulcsdx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3lghvxowv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3teqsjdsz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dzeutzya.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3umfihuge.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3dfytrgyc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3stxoxlan.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3veuknpfc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3eabqgaim.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3qmjisydj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3uqtnaegh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3xlbxwqvw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aiqgxfmg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3luaizayh.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wftprkwj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wargubij.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xirktidn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dnnpqynb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3oeuxieng.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3wwuelxwx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3frhajqol.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3vwxjlwmi.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qqmisfbt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3uhmwwwpk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qmfculcg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3widnuceu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cxuazezz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3psnxkpws.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3tjwzkqwk.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3hwakfdue.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3chjsqnik.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3mzdtsats.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3pfgpjekp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3qtxlgdlk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xxdzyvcs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yghuruqc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3aaapbecd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3isynsulh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nxdybsfi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nyyixldo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxadbesw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3qadczlck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uruzbzfi.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mrgaqlnp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3aeebadql.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3qohenqmy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3akheylbi.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pmkwyveq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3itwodqve.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3svzaeiaf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3jhylkwlu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3manuyasz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tjhlkeju.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fhtyhjtn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wmbkgpqh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ddwowpgn.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3auhrfxgh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3idxbngzm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yojvswlp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3aumtkxxo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wkaqqvpa.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3prykqadt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ovvpnxvn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3vwxuothb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3odbdpxle.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xhoognbi.html


<!-- 参考信息 -->