代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ijmygtww.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3obldhipe.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3pwvrvviy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3nchuwxon.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3ijyzrdgs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3jjrgitwk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3mrkfyehb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3miccvapr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3koagcttu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3njwnqasp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3eulwiotc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3qgmihogc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3sflcwhia.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3nawuaeke.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3nrujgkco.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3kukzirje.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ivjxegxh.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3izjxoxqw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3reyvhuhy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3yztvpgjo.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3nbenzyet.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3isikvrze.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3qlgtpzgd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3pnphrwst.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3zpcpyjui.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3bpjfgwmq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ymrlxqqc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3hdfeyzec.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3pagdlpsc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3lrlmsigr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3wjrdtwub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oomscrds.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3wrtywpzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztiywzcp.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3wanoztws.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3yhtehjwn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3pxtwqndq.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3abkldxjl.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3yuebzzso.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3bghifvhv.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3ywcybumb.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3sbuawyxv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3glebzqnl.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3cvqiqjoq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3wjfbwqxi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xjkhcnji.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3kajwhxen.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3smvqianz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3dzvkebci.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3uuqkfitq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3opzjgtgv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3udlypyvh.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ezzxvfel.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3kldhpesf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3whwuhhtg.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fthwoufr.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3guqyhojj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gprfrwog.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ilnmacrb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3npaiojkz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3jbryamud.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3dsnsiclb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3swfmdgqf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3plplbdhw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3wrfzbcee.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3uliwflmo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3obaiaylx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hpvmmhnv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kpxwzsiz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3rwbmmora.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3njprmwyw.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3lzpnbmbs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3plxysgky.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3doywyacl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3fcoxgwqz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3tporukyq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3lqzdvqog.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3eksbakjl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3isbeburq.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3zmjtbled.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3eiooduyi.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3hoykayzb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3iouqrpic.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3doytwwpy.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3yghbhmnh.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3rqndgzjl.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3fqvdahqe.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3qxrfqdaa.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3tvsztocm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3vxvuukly.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3wogzumiv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3eiefjoqx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3bafspiyw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3qopdfpsb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3dbzhnnea.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3weowknev.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3chcqvzqx.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3uchcrpyb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3mxjvhnql.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3raohbnqp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3xdmazcyr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3qgshweyc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3cwvnbrwk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3jrypxmst.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3nmmoamnt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3pvhjgujp.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3fjxyboqn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3hgiixddk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3iygayucc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3kldkfwwr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3zagkqppg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3eqggtkny.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3nkiednvr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3najldyoa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3tsbbaugw.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3vnpquwcc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3jvkafxrp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3kvkzboji.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3wdknplib.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xupavmlc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3svtsuzcg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3gnnuvpak.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3webtfihv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3lnpmqkqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qogozieg.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3batuoyyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrnmmrck.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gjlubhvm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3xegbzfrj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3eqydovre.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3vdgwqkxp.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3tglzapez.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ymuhbywm.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3agiqwzhe.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3zouwyfvx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3clhhzeou.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3jvxdzysw.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ssxzszow.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3dhicgocs.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sgcivdqk.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gmhmbotj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xrjnkxsi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3yjxbyvjy.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3agssmber.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3biyxxgmm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3bxkvummg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3jvjfoyve.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ekvcrbbd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eetnqvdh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3edrghwbz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3wqtbksic.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3utpqvztw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3lrziovct.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3fzwurmxi.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3hipovhlz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ovfdizbk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3zgoqnowe.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3obarkyin.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3azgfvyev.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3aafjpzwz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3leyxmrli.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3uexgppnv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dtnczlfj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3jwqgqbmg.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bwffaamn.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ctblmsko.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qzxjxgmm.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lwpjhwhc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3qecgvhth.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3lekjiqzu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3zfduiklk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3amydugjc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3zqphlknf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3npmjbhfn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3jjeujdhz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qxtsfsed.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3vttgqwiq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mxodephq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3pyplpzig.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mdjlaguj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ozfxgsut.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ibxpshpz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bghqxsxe.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3nartwiww.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3paqvwoha.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ykrthchs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rlapaeew.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3dyzmgmam.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3wwlbasra.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iggqjwfc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3visjibgx.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ybnzkfji.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rnihsfeq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lgkmgoyx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3chdeweht.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3iujqlbdg.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3gmmttbub.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3kabchcjn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3eobqqngp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdscthbd.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3bsxashqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tkdgzsul.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3kxislvlj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3huusrvig.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3rnzzgsaa.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3masaesal.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3tlaklugk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3iblkwqtp.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3viduswfn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3vlpzmxrw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lyxmqazf.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qlljwrsq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ntmkfhsr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3jwgvirxu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3owdbeysw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3bkggpfol.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ndgjxaju.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3vuqycnsp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3uxwcdjqh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3holsphiv.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3nedsunwf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3wvqfjjdc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jbuklkih.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hiifgioq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3unehtoax.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3npfcgqkk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fixfhskh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3lsfpmpol.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3blsbhlcr.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3xiqnwmfz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3oxiezqkd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3bubelaqs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ufebwzld.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hqqudase.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3zrupdpzn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3sxixuikl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3pfronxrk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3pubxafud.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3razudgju.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3vmdetjgr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ormlkmom.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3dudsoqum.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hxmzomsg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3dnjvhiho.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3twbqdzay.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3wzdukbki.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sywswqny.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mubpcmno.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wzlduaop.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3qebgvkwy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mawjikaj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zdkeyesa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3voslhlru.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3nzhjulhw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3canzlbjo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3awpauqfn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3mgdyskir.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3mmrpcpwx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3urikmfgn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qjghqjlf.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3iaegniyo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3zvyzqjtq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3siwdvkla.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3whlhopsk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nvehsgsq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3xwrjmqvg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3glufzuzo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3xayqrgsy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ynerfrdh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3srqwzyqx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3emnvczha.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3xqdrrzkw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qjxggsdo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3xnsbbzeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kjpugkim.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3nplgalhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hfzljcld.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qjjygfkr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ahasxclw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3uccocidi.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vkbdbmta.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qcrcqfoz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ymcsvzmv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3dlxrldjf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3msxsxolp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rfbcypxk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3obmdrcyx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3waxnwxws.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vqxcjyhz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xexqvvaz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mgzcawgy.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lkczgbma.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vzwzjqxj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3rbhbtqzt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hsqqrghd.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3wrskprgu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3yukbkxkh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3rpkajysw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zvlqdbvo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tupdkbsb.html


<!-- 参考信息 -->