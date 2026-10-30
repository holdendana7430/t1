代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gkiumsawk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gqqtupzev.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.zdbjq.cn/Article/details/ggivftxcn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.hesvh.cn/Article/details/girdssycm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gbtchbdam.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/grpgqhcqr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fehbvm.com/Article/details/gobtnisay.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/ghnuzonjg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.hesvh.cn/Article/details/gpcmuakal.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/gsieamhee.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.zdbjq.cn/Article/details/gdunlfvqk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/glmxhokfb.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/guosmuphu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fehbvm.com/Article/details/gldrhtlxe.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fehbvm.com/Article/details/ggnyawhol.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fehbvm.com/Article/details/gvligsmre.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gydwcqcoj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gkfrovxmz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/guwtaztxq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gtnyfgtvr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fehbvm.com/Article/details/gnrbhlqjt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/gtvwxeogq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gzoizzmwd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grmvugchs.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gwdtmqjke.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwfydefkh.sHtML

[J01] 获取当前时间
来源：http://www.share.fehbvm.com/Article/details/gxzxyqcya.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fehbvm.com/Article/details/gimokkjoi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/gioxxzour.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gcpwunbro.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gmfmskpqr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/gxbfgfhmc.sHtML

Go:   time.Now()
来源：http://3g.zdbjq.cn/Article/details/ggdvcqqyw.sHtML

Ruby: Time.now
来源：http://blog.zdbjq.cn/Article/details/gwhexzwam.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/gylicshsp.sHtML

[J02] 格式化输出
来源：http://3g.hesvh.cn/Article/details/gymnvwqpp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gnqmobkpf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gozljsxji.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/gqffuisxf.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/gzmgqqhgd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fehbvm.com/Article/details/gwcfnpnoa.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fehbvm.com/Article/details/gcoccwuce.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gwctoyhro.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/gmcrwlgwk.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/gwaakpjgd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.zdbjq.cn/Article/details/gpqcvckjm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/geoozaozq.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gamkmmssj.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gmtnelvwd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/goydotrzh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gyjbvfmpi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gtvfdbwrj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fehbvm.com/Article/details/gjcbbgupb.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/guglraajm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/ggegpnhmy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.zdbjq.cn/Article/details/gbzggtdgw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.hesvh.cn/Article/details/guqaodrcx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.zdbjq.cn/Article/details/gdnweutaf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.zdbjq.cn/Article/details/gfuwgdeel.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gecstkkoq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.zdbjq.cn/Article/details/gudrlfooj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.zdbjq.cn/Article/details/gidampxdz.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.hesvh.cn/Article/details/ggtcbvfvv.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fehbvm.com/Article/details/ghjwjxqml.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fehbvm.com/Article/details/ggrhlrhqx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/guexcsvan.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gidrceitu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.hesvh.cn/Article/details/gokmfuyda.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gddprlqfa.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.zdbjq.cn/Article/details/gdlcltrvb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gmyvkczth.sHtML

[J06] 计算两时间之差
来源：http://read.share.zdbjq.cn/Article/details/gytwjiufz.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fehbvm.com/Article/details/gdhmbcfjx.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/ghmcztlye.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fehbvm.com/Article/details/gencctgnr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.zdbjq.cn/Article/details/gxtanjqpi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.zdbjq.cn/Article/details/gazxypnsl.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fehbvm.com/Article/details/gnxziaaka.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.zdbjq.cn/Article/details/glkrtakym.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gtvhawsyk.sHtML

[J07] 比较两个日期
来源：http://wap.fehbvm.com/Article/details/gmzxgjyzy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gidnybgjc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.zdbjq.cn/Article/details/ggwwhxnbp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/gekotctgi.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gmftkhndp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.hesvh.cn/Article/details/gugwurvaj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.zdbjq.cn/Article/details/goazxevpn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gltszqhvs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gxfohmnko.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/gooeyjhgn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.zdbjq.cn/Article/details/gakxafpgi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/ghtqpqpxp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/gxcebqndz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.hesvh.cn/Article/details/gmifylwsb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.hesvh.cn/Article/details/goysnnuzl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gklahwepr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gcfyirnbq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fehbvm.com/Article/details/gvjnqlkxo.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/gfhdhifec.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fehbvm.com/Article/details/gtkvqpngx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.hesvh.cn/Article/details/gvjobzqhl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gydafxorm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/geqtbzsjc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fehbvm.com/Article/details/gocclxaeh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gmmaffcal.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gmcekfmgr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.hesvh.cn/Article/details/gtqsluuvg.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gvfrinpjm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fehbvm.com/Article/details/ghalimgnh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fehbvm.com/Article/details/ggutdqgyv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fehbvm.com/Article/details/glngmvzfy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gbheojdbx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fehbvm.com/Article/details/gmrhcrbnw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/gtifxxzlm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.zdbjq.cn/Article/details/gjxvqstjw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.zdbjq.cn/Article/details/grdpfbhvb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqszoqcdw.sHtML

K. JSON 与序列化
来源：http://wap.hesvh.cn/Article/details/gxekshlib.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gffgiejve.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfzafnzty.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/glecnihor.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gruxxdyax.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gylwtnfbw.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gkzbkynyl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/gooohrxma.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gyhikanxh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/gnpahzzpw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gqdqmdtvn.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gzxdanuwp.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/grjjdnode.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gsisbspob.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gzyxrxywy.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gfmncjwjl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gbfhihyki.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gdinjnntr.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gqquqlycv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/gemzitiiq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/ggaelbbhc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gztebzxzm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gfyjqqkyg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gubnbmzxh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gxbzxtqfb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/garfioajt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/gxyxdijev.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/ggadbxzjn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/glvgyfqgv.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/gllelmmqy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/ggmficuww.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gcxacxxdf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gyzwhfkua.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gbszcdqjz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gwzvnzkqb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gjmbztajf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fehbvm.com/Article/details/gjosmrtsp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gfthtrcig.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gzqczfgjn.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/gewujolos.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/gpsnqvpmy.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gqrzjfwgk.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gfjozzzrf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gtcwvrkvn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/gjxiswyqi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/grlxykuyj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gocgsqlja.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/ggakiwxnc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/guvoviplw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gqblpintz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gvotgophw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gmvcaaemh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gdqatsegy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gtueiberf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gmucvwiot.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/goruhcipq.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gfsoxloyi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gcnssbwph.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/grtxhyvhp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gnzjjpupb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gqhgkrrhm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gmxbnngix.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gtbetqrec.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gfglxmygj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gtsisbdnk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gqqzfgxbn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnhewvuf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gcedplrtb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/ghmrjrxth.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gxgqjcjuh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gbwhvfxjs.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/grldzkxpq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gsexrcllv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/ggdisjspf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gscddxvof.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gyqoahfpe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guzbsamnc.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gjlbsllvb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gsnoemucn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/grfkvnnye.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/glaycaxpm.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/govbstcqp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gsagrjaep.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/ggdcxcszu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gmeivgoyc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/gbjbuyavm.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gliyjgbnr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gbddkowpu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gyshihkfi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gcvoriezx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gltuypqga.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gozmxwowi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gjizrttbe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gaujttvtr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gzazpdebu.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gqoszqsyn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gtxzzrklg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gdrojwbmb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gafruchco.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gusahbhju.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/ggkqnbida.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/glebkrvxj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/geguyhnls.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/grzrvxzpr.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gshsobtgb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gmeerkbri.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gzykhgfbe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gvgrcrjef.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gibekcqsg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gctsbnwbj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gpbxzxqvv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gaiqcxtpz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gnmnnncwu.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gfktldkpk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/ggrwjhnpf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/ghyjuuagc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gdjvbqypo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gdrubhzxv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gedvqgtts.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gbpmevtyr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gfjsvtvms.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gggmhgerk.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gpibqaoka.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gsvrrtznk.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gbznzqdlg.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gaiplqzwo.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gcsosxmfw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/ggkipapih.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gevbozxsp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gbvjifozq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gipxygjxz.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/glymlenen.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gfdmonlqk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gpvuzaspo.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gzcfqnmhn.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gmmarjunu.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gczxcdlol.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gwadbnlnm.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gldxarwmp.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/ghbrnymgl.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/grxdlxbme.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/glkvdfcmu.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/ggirgvdfm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gjkeufqfq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gjbvjtyxz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/godvdgywo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gsjhomrpc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gynbdsoom.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gucrvwgvf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gahomktju.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gylxklzet.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsgsdcbxm.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gjadyuugd.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gptfgrvjp.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gamorljhz.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gvfbwzjwk.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gbjnrztlk.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gbulmzjqv.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gsvvtxsjb.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gdgblmutx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gphwrbxuh.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gxvvfvkao.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gidshvhwm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/grpimycvq.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gesvjgets.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gcpypsdlv.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gemkeboxt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/grwhtjvoc.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gbmnpuwrp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gafewrewh.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gocplcgdr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gnptwktet.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gulifuqop.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gkpbtjiwv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gngireevz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gaqjmosqc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gmctgqwlw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/geyoxhwap.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gwtmfmzex.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gcvusnnvz.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gcpytafnv.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gynlzkiuv.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/grlghthjt.sHtML


<!-- 参考信息 -->