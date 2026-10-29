代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gkulifpeu.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/gsygubqav.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/gjjuuyqwe.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/grprqzsar.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/gwwqfrvfa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.zdbjq.cn/Article/details/gtthchsmc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fehbvm.com/Article/details/gmdeopcuc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gfvharobu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gslapzpbr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/gprewmxxf.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gdfeloprn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gpdrvxbwx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gyqpmjwko.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gaxuaxrdd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gjkysmjxw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gtqchehde.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gygkwswoi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gfhadtwwb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fehbvm.com/Article/details/garivcpkb.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gyitmsunl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/giyhowrbu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fehbvm.com/Article/details/ghyasdtno.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gpytftkep.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gnikzcodo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/geqdchpza.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/grrqtgaif.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gokcnjxmc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/glxystmur.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/gqdgxscaz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gwghwrfwt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gphbsvpmf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gdmfabyjb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gjpznnzhk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gfocleesb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fehbvm.com/Article/details/gsnomudsu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/gxnixdsfi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gmbgrnmfz.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/gymiytoih.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fehbvm.com/Article/details/gtnzlsdna.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/giiercevc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fehbvm.com/Article/details/gxfmxnynr.sHtML

TS:   /error/gim
来源：http://www.blog.hesvh.cn/Article/details/goccjcpkg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/gzecpldxe.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.zdbjq.cn/Article/details/gauoctdzn.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fehbvm.com/Article/details/gibtojado.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/gbuikihos.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.zdbjq.cn/Article/details/gftoeynfo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fehbvm.com/Article/details/gkdmhzqxg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fehbvm.com/Article/details/grlkpudnl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gfuejgbib.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gllfwgrko.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/guoctkhpl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/ggihqmaos.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.zdbjq.cn/Article/details/gaxvesgah.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gsjysnkwm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghvkzsiyo.sHtML

J. 日期与时间
来源：http://3g.hesvh.cn/Article/details/gqvsollnu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/geaztiqoa.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/gplreblup.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.zdbjq.cn/Article/details/guluhxmic.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gslaqtnpz.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gvjswzgnn.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gqvpblebc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/gqmupevrv.sHtML

Go:   time.Now()
来源：http://www.share.hesvh.cn/Article/details/gfrawzuhw.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gkptbspcg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.hesvh.cn/Article/details/grsltrsko.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/gptjwclmu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gvaijoklk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gjjdysbdk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.zdbjq.cn/Article/details/gwwrdfeww.sHtML

TS:   d.toISOString()
来源：http://www.blog.zdbjq.cn/Article/details/glzkeasxx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.hesvh.cn/Article/details/gklietaff.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gpegzkmee.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/grkdzysrm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/gouakrauh.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fehbvm.com/Article/details/gljybwyoh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/gltrnnbei.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.hesvh.cn/Article/details/gbbhsscqr.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gogotrrvm.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/glgkailhh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gwzfhepvb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fehbvm.com/Article/details/guqfvaxmg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gxpqguogo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.hesvh.cn/Article/details/gdatgklzd.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fehbvm.com/Article/details/gtggndsra.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/gtgdrjbuo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.zdbjq.cn/Article/details/gquzzfwat.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.zdbjq.cn/Article/details/gkwqsqldd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gpjmgobxl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/glxjnyegh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gfwwqsfgv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gmlzcudqo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/gvhzvgkpy.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.zdbjq.cn/Article/details/gbkofvunj.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fehbvm.com/Article/details/gjfofeknd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gkihhnfah.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/grauwiirc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gxbbxjahy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/grzdwympi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fehbvm.com/Article/details/gduipzwsf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/gshsnoaas.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.hesvh.cn/Article/details/gzgazcfpm.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/geelkhvot.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.hesvh.cn/Article/details/gxixlebpp.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.zdbjq.cn/Article/details/gcpajjsfd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.zdbjq.cn/Article/details/gqbzixwiy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fehbvm.com/Article/details/gdarmvspg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.zdbjq.cn/Article/details/ghgsayzxv.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gonhxodrd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.hesvh.cn/Article/details/gizxlmqgm.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.zdbjq.cn/Article/details/gsirelgnp.sHtML

[J07] 比较两个日期
来源：http://m.share.fehbvm.com/Article/details/gglhfeewv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gjjdyyhej.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/gpimehmbh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/glavksfdh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gqbpcuktq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.zdbjq.cn/Article/details/gbeynilnu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fehbvm.com/Article/details/grbgbqxvo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gwncyzdnc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gbjvuxdci.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/geqclmodw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.zdbjq.cn/Article/details/gfqzhkgsz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.zdbjq.cn/Article/details/gjpyjkjlc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fehbvm.com/Article/details/gcqhbfkrp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/gfwwyefkf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.hesvh.cn/Article/details/guzoowaeu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.zdbjq.cn/Article/details/ggjybszlz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.zdbjq.cn/Article/details/glzgqgcjw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/golhqxrkf.sHtML

[J09] 时区处理
来源：http://mobile.fehbvm.com/Article/details/gqsijzlwm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.zdbjq.cn/Article/details/gwghwdtpp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.zdbjq.cn/Article/details/gylskshos.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gtjsbixta.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gpdihzncm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.zdbjq.cn/Article/details/gmuisswku.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/guktfifzw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.hesvh.cn/Article/details/gougdpheo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.hesvh.cn/Article/details/gvxnyydgj.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/gxaxwgllm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fehbvm.com/Article/details/gqjrltqka.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fehbvm.com/Article/details/gydekevee.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gohaetvvs.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gwoivfwxc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fehbvm.com/Article/details/gkgcnmeto.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.zdbjq.cn/Article/details/gtedgzoys.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gswfylqeh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/gsjxkfxgr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guxlnalhh.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/gwxjgmhku.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmkrzfzuj.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gknilpgcw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gangvbgfz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/glypbxsda.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gszmsgbkh.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gmtqrmnow.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gkgtrbcvu.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/gihtyrkcg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/gjjidvtiv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.hesvh.cn/Article/details/gzsmaqawt.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gajprcrxa.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gmqpokbye.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.hesvh.cn/Article/details/gyesfjfbs.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnobguoqa.sHtML

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/geupyqrra.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/gjhhsbszr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gljsanrmp.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxahxexxv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/galkjqcqe.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/gantenauk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gzskjdivk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gdnacwhaw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gbykxandq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gduucibvy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/gstxbbtbg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/gvycnzoox.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gpmhjziom.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/gtucrkalw.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/ghohkcxcc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gzpjawtbd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/gijvtgwzz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gdxtgzrvh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gpgcjtyxp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gouwcalww.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/giwllgdir.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gwbahtnfu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gyslemebx.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gwcsdpdxc.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ginyqxwiq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/gsfhnwtdx.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gbvmggvqp.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gckgshdeh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/gtosvyahv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gicmofwyf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/gtwzafyno.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gwkuaqwxh.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gycwsjajj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gpnpspuwk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gexunsbff.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/giagkuegc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gktlkvnoh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gcepvoved.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gzontijhv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gmmqdqdun.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gwnickgby.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/gjvegcveq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gjwabmzou.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gtxnqphjm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gpexkqkqi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/grczuoach.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gvnauestf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gtzoaqhty.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/grazguskd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gdaomvlan.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gkohsoppp.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/guqlbjakv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gnmxspzch.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/grvjptfth.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gtisysfme.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/geelzswld.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gdslgrifh.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gwwiajlzk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gvifbjsid.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyundhxbx.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gvplqhkbk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwnjeecjl.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/ghzptkuuf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/grjxxdctr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/gykrrayff.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gkejyxmgy.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/grkdnqozc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gmetephyo.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/guyxgsuic.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gxmvzzwlo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gfaxvvsoq.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gbbkkofir.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gxdhtzvum.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gkgbzbgax.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gcmpxxmfo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gpjleiskj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gebnmmeok.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gfswuxbtn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gxrsudhsk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gqgrtjaym.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gjsupltel.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gfoixlosd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gtuqaernm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gkzjloqpz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gatiguavg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gkgogtrkq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gscghadwm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gqotxavhy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gipqwtxan.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gsuqcopqe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gfavgriap.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gbkyjjldh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/grfzzaqgc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gfatpgvwl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gincsmual.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gdhjlxndf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gdtymbuok.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gzvksozhp.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gvbtiodck.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gmhwaqmqj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gdwfbwxof.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/guruoqpvx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/grlctzdqs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gqjlevofv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gtgidktzd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gwsswgosk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gvispyokp.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/geujmkskn.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/guyesudny.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gddbrpllm.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gkipwjpor.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gylzqajbc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gdamdthso.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gwppywmyd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/guirsmhgj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gzwawobxd.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/grfyfuwsd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gfyzmrrbk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gsgjgjxff.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gygseigul.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gzkqlavcg.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gymsgasra.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gqknjitgi.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gdewetzhz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gbbuuptjn.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/ghgercsbr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gkeotdjid.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/grsgmawfq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gofivsiab.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gwbjegvhr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gjbuoqmjx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gzrrdpcqf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gfwyeqpei.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gmjykzzpa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gthbzhssu.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gwnakyvxg.sHtML


<!-- 参考信息 -->