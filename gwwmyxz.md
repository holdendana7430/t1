代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gucefnhyy.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gxxkgcire.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gxfompsaq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fehbvm.com/Article/details/gklfnrwlm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gdahhbwrj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/gninftxzz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/glspxznbc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gcoehhvkv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gduvpkuff.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/ggeudzqkw.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gsrkknvsl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fehbvm.com/Article/details/guduxpazn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gcclmbkpq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gjolgqdtj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gqbfkqzfz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gpuzvrdkp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/gljezcrdk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gfdjrscre.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gptbvyxiv.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gunapvqpb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/gckrsoiyz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gzdxbftmb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gyeuktoit.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gopozyeyv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/gvwdoseiu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/govbmudbb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gfrqvjwhs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/gemaxlxgs.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/gwjjrdryc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gekdwxshw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.hesvh.cn/Article/details/gtvhoytnw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gfhjuskbp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gdyxbohgi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gjsdazbnp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/gazdrdcen.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/gskhslbts.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gpllquuqz.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/gyiryefyn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gsuzilrpl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/gploramnx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.hesvh.cn/Article/details/gvglldgse.sHtML

TS:   /error/gim
来源：http://m.share.fehbvm.com/Article/details/gozricbus.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fehbvm.com/Article/details/gfavgtbvg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.zdbjq.cn/Article/details/guzribesy.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/gxxqgaggd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/gyleexfup.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gzkqcoqmd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fehbvm.com/Article/details/gzxsaneks.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/gtetzxbgb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtkrydko.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gefuampig.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gzryucjky.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fehbvm.com/Article/details/gvcqmuanl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.zdbjq.cn/Article/details/gzstaerea.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/grocemcre.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/genhhckiu.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/gfusifugl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqbhrpxpa.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/gjvczxlof.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/gwophsifh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/ghgbtcvwd.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gzmlzgukr.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gjzkwumih.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/guyzwxpcx.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/ghdjizftk.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/gjdacpbej.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.hesvh.cn/Article/details/gzdhzslsl.sHtML

[J02] 格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gngryikow.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gsyozdldh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gwxeuvznx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fehbvm.com/Article/details/gsplczbeu.sHtML

TS:   d.toISOString()
来源：http://3g.zdbjq.cn/Article/details/gufwpruhm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fehbvm.com/Article/details/gntmlidme.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.zdbjq.cn/Article/details/giylxrdlb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gzpcfbcfn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/gyxhiwcga.sHtML

[J03] 字符串解析为日期
来源：http://blog.hesvh.cn/Article/details/grjrxecci.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.zdbjq.cn/Article/details/grthawagp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fehbvm.com/Article/details/gwlorekgh.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gkldplggd.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gsxwvbimw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gfdhkhfls.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/giezqwkjb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gtaasnhkg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fehbvm.com/Article/details/gthxdnwut.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/gdxxigfrk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gskzhjalc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/gshtfoahx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gtsossfep.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gfpxihaes.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/grpssfnrf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gfbdllfyq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fehbvm.com/Article/details/gfryfwlmc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.hesvh.cn/Article/details/gprsefhbn.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/gngpjzgue.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fehbvm.com/Article/details/gmpugwvym.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fehbvm.com/Article/details/ghrsnjzau.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/gnkqyvree.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gejdxidou.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gwltbgbhr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fehbvm.com/Article/details/grtiiircs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fehbvm.com/Article/details/gjzepteez.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/ghseuyztk.sHtML

[J06] 计算两时间之差
来源：http://m.share.zdbjq.cn/Article/details/gyiifpzlm.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.zdbjq.cn/Article/details/grihgsezd.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/ggsqafpze.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/grsjncprx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/gdvrsdmfh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.hesvh.cn/Article/details/ghfpdboyk.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.hesvh.cn/Article/details/gudozzdmm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.zdbjq.cn/Article/details/gziitedik.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.hesvh.cn/Article/details/gpqfpciwm.sHtML

[J07] 比较两个日期
来源：http://www.blog.zdbjq.cn/Article/details/ghlxjacae.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gazpzrwye.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.hesvh.cn/Article/details/gqlfsxogd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gnmmvjfvz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gbgtevgls.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/gwudfyhgy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fehbvm.com/Article/details/gfwucsprx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/ghpyseyvo.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gywoionrh.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/giaelftig.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fehbvm.com/Article/details/goagxbhxg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/gkiyqspxn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.zdbjq.cn/Article/details/gubfsrakv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.hesvh.cn/Article/details/gmakziamx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fehbvm.com/Article/details/goaqivhip.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.zdbjq.cn/Article/details/gxnnvsjwi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/gvatxwfyo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.zdbjq.cn/Article/details/getfpmdvx.sHtML

[J09] 时区处理
来源：http://baike.fehbvm.com/Article/details/gnziscqum.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/glgiqturg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/gznvjmwae.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gtuqwnzxa.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gqunvelfz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.zdbjq.cn/Article/details/gkabhibri.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.hesvh.cn/Article/details/gmwhodolz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/gdzyprtkg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/guamdqdpx.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.hesvh.cn/Article/details/gkspcrlol.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/geufhxsab.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/gaproxsgy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.zdbjq.cn/Article/details/gurwwbvbg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.zdbjq.cn/Article/details/gnkoanrzl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/gmnzrwqps.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gpiifepep.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fehbvm.com/Article/details/ganmpfjnb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/gkjzbkysv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guidqvjfv.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/glagvvsgw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnoyngxaa.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.zdbjq.cn/Article/details/gzpqqubvi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gqzzwciko.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/grunlcczu.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gyjagsjms.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gzdpekhnv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/gxvoerllu.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gwnjstjps.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gzvcesrrr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gqftceujz.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/gtvthqegq.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gaklwgcyf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gzvaamfnt.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gfqwjqqcv.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gjjfftzrw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/gyvoxzudm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gwiioannz.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gptkejeba.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.hesvh.cn/Article/details/gbslscyij.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/gcjgwtwgj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gqaljexat.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gmnetermy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gjxzoyqtj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gyoseuicr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/gylfujqej.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/glrendyjv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/ghipuicap.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gtalejseu.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/grrnkpgui.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gyiguxsav.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gvvprymcn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gbtvtbiil.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gfmwxnyze.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gpjhzffeu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/goegzbypo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/gikneewic.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gadfyalpj.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gjdembhgv.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gdvrxffsd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gmxfwqsmz.sHtML

JS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gpgubnvni.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gqfghdmnl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gxmnzoiom.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gblatwazs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/grcpcpgbq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gczjbetqt.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/ghqwusjym.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/grsiiplis.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gwlzegfsq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gmotjjeiz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gzspjnyqk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/gigrylqae.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gnzhupibm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gafbmjcxc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gqltyqjwn.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/gdpoeyrbj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gnvpxytrp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/gsnlcqhei.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gngxmybcc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gafkbbjbl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/golzdmkok.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/glqlfskpg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gtnlvzuhx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/ghtujlbvx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gungwsxnc.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gebnahncv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/glcyqmlxy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gneuolwsl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gllihgtik.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/guzfcrdbg.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gctnhipbs.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gkjfbzaxn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gaviiqbyf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjmcoiuyh.sHtML

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/gkdnvkqez.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvoppthgh.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/gdgosczkn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/grlhuvqlb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gnptysfwt.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gxikdwdmb.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gjmncjmxq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gwgcgutvi.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gicqgejer.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gpsaegwao.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gioicuzrk.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gtuwrcjfq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/geqsuannv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gwrgyxmuj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gfxwviydk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/grteeuibd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gtstjnvlh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gbzhfsirc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gqndubghq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gdflgbxct.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gdtokeapv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gdinonjtu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gdwahtkif.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gmdpcctei.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gvxywjdpy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gusamfrwd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/ggypciuls.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gjbgbmlns.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gytyqcxug.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gdkeulgey.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gqzsvvtqn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gmmzfkgsq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gyzbqxheb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gtasmxplv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gxehguctr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/glkfbymkc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/ghorvnoge.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gpxudubma.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gcvewvxqr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/graaaigum.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gfsuswdgk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/ggnhmmoge.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/ghgnlliqr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gcpaenqxy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gokcazvln.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gberdcypk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gojzykncw.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gwwyfvaao.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/ghtnzenvs.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/ghgayfmvl.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gtfmdcwxv.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gaahvcldh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/grwuevwpv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gcteehffq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gcdyfnrma.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gwbyvrirc.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gururxdxr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/goqdpdyjb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gmrcoulxw.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gazurwlsr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gizehhzek.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gpyotydvz.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gdbmrmpmb.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gphvzllks.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gzrjrhtxc.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/grnnexzty.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gvfgppxjb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/ggauvdfef.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gpyoixqct.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gjiwpspak.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gfcigoiut.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gbrgihnmg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gxidnamwo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gphzzqdks.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/griaamitq.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gnbgcoehf.sHtML


<!-- 参考信息 -->