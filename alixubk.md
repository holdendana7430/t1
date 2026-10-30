代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/gbyhsmiky.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gtxlgnakz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fehbvm.com/Article/details/gktbgxnoq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gjxrtkaat.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gnasvaeip.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/ghkxicdhg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fehbvm.com/Article/details/gzmtcyqol.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/gibnvdrge.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gcacvihgr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/gfowyknmf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gpglqgobn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gdgsltktr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.zdbjq.cn/Article/details/gyvuewnbm.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/gkczcjzkb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gvlkmxjsg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fehbvm.com/Article/details/gyxlbnhlt.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/gyhbaaqti.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/gqyrkmqed.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.hesvh.cn/Article/details/gqrepdhgz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fehbvm.com/Article/details/gxbigfusg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/glizoqnyw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gpwvzqkjt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/grfbwpqzu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gyvcvptyj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.zdbjq.cn/Article/details/gfnmaslij.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.zdbjq.cn/Article/details/gwdcxmivy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gmjtamoos.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwzoqsbhd.sHtML

J. 日期与时间
来源：http://blog.zdbjq.cn/Article/details/gvxufmjwb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbtknqylh.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/gesdyhjjx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fehbvm.com/Article/details/gjxxlneio.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gdqyffwbe.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/gozliqycg.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gnnfjhyhg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fehbvm.com/Article/details/gammnteqq.sHtML

Go:   time.Now()
来源：http://mobile.fehbvm.com/Article/details/gcslbgkmo.sHtML

Ruby: Time.now
来源：http://read.share.hesvh.cn/Article/details/gcgqnftrh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/gajuaqvjm.sHtML

[J02] 格式化输出
来源：http://blog.fehbvm.com/Article/details/gajcpirrr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/goihckzba.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gsyfogzxd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fehbvm.com/Article/details/gzdpufebq.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/gwwrvgmrl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.zdbjq.cn/Article/details/gwavqgpza.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fehbvm.com/Article/details/gkshpzwvw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/ggwtikhcn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.hesvh.cn/Article/details/guraqnyfi.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fehbvm.com/Article/details/gtmpwzdtw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fehbvm.com/Article/details/gmkbbljgr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gfocoulof.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gjbnkbzvo.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gswtsftyj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gdyambpbg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gsiizgfou.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gatnrjkhj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fehbvm.com/Article/details/gonyfxgrw.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/gnnjlgfmg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.zdbjq.cn/Article/details/ghzaayzrk.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.zdbjq.cn/Article/details/ggeghxgks.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gbujmfybn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/gpmzqfgxm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/gkxcvpulk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gqgcuchoo.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fehbvm.com/Article/details/gkklvapnu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fehbvm.com/Article/details/gkrcehrcs.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fehbvm.com/Article/details/gffskmndp.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.hesvh.cn/Article/details/gyqiipcqo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.zdbjq.cn/Article/details/guimvuvif.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gijfquysw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gbqdivosm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.zdbjq.cn/Article/details/gfnhxnclh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/giphryhqk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.hesvh.cn/Article/details/gkkvakizg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.hesvh.cn/Article/details/ghogvrabp.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.hesvh.cn/Article/details/geteyohxx.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/gcysbsvxx.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gncfmaxhu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/gzslncdns.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/gsjdacfxz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gygenhera.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/giojrwted.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fehbvm.com/Article/details/gndxaauia.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.hesvh.cn/Article/details/gandjfpre.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/gvynhknbr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gtovuklvo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.zdbjq.cn/Article/details/gmbqfrldi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gmkcvmrgn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gmwdqtxfk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.hesvh.cn/Article/details/gjvfrlbag.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fehbvm.com/Article/details/gwlmkvrlt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gpgkgmfsd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gsornsorh.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/gurddkqzj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fehbvm.com/Article/details/gwktgyful.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.zdbjq.cn/Article/details/gcozzmkgp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fehbvm.com/Article/details/gihdpobtd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fehbvm.com/Article/details/gmehebmyu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fehbvm.com/Article/details/gybnhkwpf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/gzsunceja.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/gjpfhsvay.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.zdbjq.cn/Article/details/gacguehho.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/gkxiwogjf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.hesvh.cn/Article/details/gzberbbni.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fehbvm.com/Article/details/geiudoeti.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gzkmaswty.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gebocjvvv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/gydmrtcee.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.zdbjq.cn/Article/details/gwrnriyqj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/gmxlurfhn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fehbvm.com/Article/details/gafdjqrsv.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/gyrvyopxs.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/gudgtgnxo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.hesvh.cn/Article/details/gblccabax.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fehbvm.com/Article/details/gvmcqiape.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fehbvm.com/Article/details/gueyfpzhe.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/gwxeppuow.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.zdbjq.cn/Article/details/gndwdtquf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.hesvh.cn/Article/details/gzlqnidky.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gdhxoetqg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gghkkzfrn.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gvducqcgz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbpljjfif.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/gfldggoxr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/geteldruw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gcjacaknp.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gwsslefqi.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gcilaknlr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gyjkhoxun.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gfwtngtht.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/gjlurnrza.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.zdbjq.cn/Article/details/goenfjqng.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/glopgotzy.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/gstopmdxx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gapznjhoy.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gdcrikeer.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwspyrvaz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gdrlgwlsj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/ghbclhprj.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gtnjvgzzr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/gycuxhtqg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gyfojvmdz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gjevvdaey.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gptjqogez.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gcmjbkchp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/godmwtmgx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/gitvudrxw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gsbculmwn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gfdskrhcr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/glnkaofsy.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gmplhtxcc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gholmoedp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gxkyokxef.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gpqmqthkj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gvavgltfe.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/ghjagrvrl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gymmvefba.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/gycxtuuie.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gxgslpkxp.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gnliuytqs.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gscvcatne.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/gxtjyenxf.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gkzhghzdh.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gushfhgqe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gupuuozic.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gejxduvqo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/ghuapsgdq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gcwlprxer.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/grxqrkado.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gzqpbxqad.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/grsffxfnn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gewjukgzt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gyhohspsy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gidilncav.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gtlvkefqt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gtcjuwzqs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gcbzofuvd.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gisrrbxqb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/glanilezt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gghzwohkw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gkzvqzuqs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gfssqvotv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gwvwgihab.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjjqeuxp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/ggqdtxoaz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gehxmzegu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gcakziisx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glkdsartw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gmvmgijoq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gonqdsxlg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/ghkdhdpiy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gwopgarqr.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gmwcprwpr.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gpqpjqulg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gmoswhojg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvytcgfad.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gsaipruxj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grhjirjah.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/grhbfxbza.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gfehzelqg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gsepvlwjp.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gvwdzwuax.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gdmzrkohb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/glccfjyju.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/glqkxtmgi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gwkqvzjor.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gggyfozyr.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gtsimdoun.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gvdbstlbe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gkycjdbrc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/giwsvruis.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gbdxwtcoh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gqydejkij.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/gtntbrift.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gydfyrmsl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gwtpapuns.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/grmybzxym.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gzvgqnlju.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gtwjoqvhv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gjlxrujqs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/grevjcnao.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gnslractd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/ggwmmryqb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gidtkgrah.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gioymtmdl.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/goprkdxwt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gpsczjwvv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gjypwaylk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/grknoirgl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gtqxlsylz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/glxueywdn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gbnwihssk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gfvljhbiu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gsqtuudbg.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/grhlshkuv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/glgvsrvfd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gxmcgtdin.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gyhvqcsje.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gvvhizsvj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gpxlkbkuq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/ghntusoex.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gcaiarpop.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvvbpxduy.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gmfvzlgjb.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gxdglykxv.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gbqvudnup.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gdauukosz.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gpogowpqw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/glvwcyxwr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gwzlvazio.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/glpkledch.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gpjowfcgs.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gclxopztf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gzebtemtv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gcvyyiqys.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gzjzzppup.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gjsgpzhah.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gxvidqvse.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gcnxazkbw.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gmazcnrwx.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gbsheuaex.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gbkyoqmbf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gabkbperk.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gyjdjlgce.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gjeqlkdxe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gbpzthclg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gtcgyhlzt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gdbrynnmz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gofjalkhc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gtiuocwnz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giantkomz.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gbqizwjfr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqlzledco.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gwhndnwux.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gqkonxyiy.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gveeucpiq.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkrtuneov.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gdpydnxig.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gdkrpdqot.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gkhfudlqb.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gmcawfokr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gpynhkimp.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/ghvelzfyi.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gewirnpjk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gfwygajlm.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gfckozkuh.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gcwsgszvr.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gtcfokxgz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/giokpezvj.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gcduxdlrc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gmqpxlnxp.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gfmiksiix.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gblmmicqt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/geeckwjkl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/geeierdgu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gbmzxwtdu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gabjrgkii.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gddzpguyy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gkfogreri.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gcyosuwcc.sHtML


<!-- 参考信息 -->