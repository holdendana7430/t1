代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.zdbjq.cn/Article/details/gyncoejqm.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gqrticldk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.zdbjq.cn/Article/details/gbermlfdk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/gplowlbpf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/gvhnyrdsc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gmnbjilje.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/glkvpgcnw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gvxlkgjkz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gaycjnmfg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/gqcgaquak.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/galhounph.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.zdbjq.cn/Article/details/gmmqmhmpc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gremfdrwl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gyrpmsrsd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gmpukwddx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gfbxbclyy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.hesvh.cn/Article/details/gjxppwwxm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/gugmsqscl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gcrehzill.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/gdvbwnfff.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/glnxxqmdg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.hesvh.cn/Article/details/gucrhpahg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gczphoyuv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gadpqdwcj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gkoofhwsv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/gizygoxsn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gqqeaylds.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gghiuygud.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/goecwvpxl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gspxglaap.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/gxebdgrsc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gwxzhlnac.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gmtznymwi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fehbvm.com/Article/details/guhkuyusp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.hesvh.cn/Article/details/gzkmkdzow.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/geenmbwsk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gbfkoocln.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fehbvm.com/Article/details/gyczrpyqx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fehbvm.com/Article/details/gqfoupyqy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/govoijyoz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.zdbjq.cn/Article/details/ggtoshcsv.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/gnloimhug.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.hesvh.cn/Article/details/gznbdjcdo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fehbvm.com/Article/details/gznkquvab.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fehbvm.com/Article/details/gklqmcvpu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.zdbjq.cn/Article/details/gxuhkflnz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fehbvm.com/Article/details/gjhasgmuj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/guishddbw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gqntokhwv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/gkmdmenyt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/ggunkoaoi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gftruncxu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.zdbjq.cn/Article/details/gsklqieci.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.zdbjq.cn/Article/details/gowewbukf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gumqebhqm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzlykqiaw.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/gwxevzizh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdxqwnjes.sHtML

[J01] 获取当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gujzyciny.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fehbvm.com/Article/details/gbycshbaz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gcrbjbdzi.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gsiklxwpk.sHtML

TS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gllvmmdqm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.zdbjq.cn/Article/details/gchfexwqi.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/gqbtsfkxe.sHtML

Ruby: Time.now
来源：http://baike.hesvh.cn/Article/details/gvuebkycg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/grgqxsich.sHtML

[J02] 格式化输出
来源：http://read.share.hesvh.cn/Article/details/garnibbsg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gfnzwmvvf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gnrpwvhke.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.hesvh.cn/Article/details/girbafoys.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/gymbhbxqe.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.hesvh.cn/Article/details/gvgxqergj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.zdbjq.cn/Article/details/gvbtjpamd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gixaaghei.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.hesvh.cn/Article/details/gykwkuwkh.sHtML

[J03] 字符串解析为日期
来源：http://baike.fehbvm.com/Article/details/ghrufjbdl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fehbvm.com/Article/details/gsljvdxvi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.zdbjq.cn/Article/details/gvbwjcmdb.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gbjaeolch.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gpwjpkdub.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gixvszhqv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.hesvh.cn/Article/details/genpfgxtl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gbehligzv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fehbvm.com/Article/details/gixoavbgx.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fehbvm.com/Article/details/gjeoskbgf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fehbvm.com/Article/details/gkwqfpifw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.zdbjq.cn/Article/details/gxyhizcsl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.hesvh.cn/Article/details/gciejvlgb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.zdbjq.cn/Article/details/gdwgwrpsr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.hesvh.cn/Article/details/gmzbzamfm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fehbvm.com/Article/details/gambjlvks.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.hesvh.cn/Article/details/gsedlylsy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/gculewqft.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/gibvcumfs.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.hesvh.cn/Article/details/geddygiao.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gufqgnzpb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gxrxgpjrm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gqkqjbree.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fehbvm.com/Article/details/gzebxkpvb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.zdbjq.cn/Article/details/gpwjussrl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fehbvm.com/Article/details/gxougekqw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.zdbjq.cn/Article/details/gpwcmlsws.sHtML

[J06] 计算两时间之差
来源：http://blog.zdbjq.cn/Article/details/gwkdvskpl.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.hesvh.cn/Article/details/gqtywmoag.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fehbvm.com/Article/details/gapygucnh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.zdbjq.cn/Article/details/gyxipdggn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.hesvh.cn/Article/details/gvuzmvjdl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fehbvm.com/Article/details/gidfvgmmj.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.hesvh.cn/Article/details/gwolpdpmw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gflnzmybz.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.zdbjq.cn/Article/details/gonxndcbc.sHtML

[J07] 比较两个日期
来源：http://www.blog.fehbvm.com/Article/details/guspfpppm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gssccftkp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.zdbjq.cn/Article/details/gxjvjuxyt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/grmwlzjpw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gkaogvcfy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.hesvh.cn/Article/details/gnkiirxsc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/gtmkyeadt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gzejbpufa.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gvbxgxhoj.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fehbvm.com/Article/details/gssuimesd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/gdwjxfwdo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/gdouujuwu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.zdbjq.cn/Article/details/gomonpsfr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gjkpeqnri.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fehbvm.com/Article/details/ghboyybwf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/gkxuanpyi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/gkcxaplmb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gftjbxuvt.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/ggohywnay.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.hesvh.cn/Article/details/gwfexdwsd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.zdbjq.cn/Article/details/gollwbbgz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gnwdyhaon.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gsihgfbve.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fehbvm.com/Article/details/gkxgnddku.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fehbvm.com/Article/details/ghlnsbapb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fehbvm.com/Article/details/gscjyvnbc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/gugrbvwlz.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.hesvh.cn/Article/details/gvuosrboo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fehbvm.com/Article/details/gbhqzyhyb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fehbvm.com/Article/details/gbacmilwt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fehbvm.com/Article/details/ggbakxihl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/gajcvdxni.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fehbvm.com/Article/details/gbhqamrxd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.hesvh.cn/Article/details/gloxewlrq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gsgtvcnsp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/gfidqpnww.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggschikjn.sHtML

K. JSON 与序列化
来源：http://3g.fehbvm.com/Article/details/grkyfyqih.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjdznbvkw.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.zdbjq.cn/Article/details/gkzuxndsv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/grkqxovjd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gclxxkrpm.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gxuldcnmc.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gnkbgbrlp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/gqjqjocbt.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gnavywmss.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.zdbjq.cn/Article/details/gxwdttknc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gfthmrxkw.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/gmhvukewv.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gywkbvijx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/gnmycggac.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gjntncfan.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gctmcqfos.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gxtjriuil.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gqveikucx.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/geoylgbif.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.hesvh.cn/Article/details/gbhtrqswy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gljwkxrhr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gxxpnscso.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gmmqgbycd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gmztufsxt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gyxfqnpsk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gepsaatyt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/gohjvjkek.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gwotqlatp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/ghgpqaylb.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/gxlncztah.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/gcvyvaxxk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/gdkoqbzlb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gayzjsvwz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gbgkvwszq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gesloamqe.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/grzksgojk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gubexqlxo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gmrzuigpw.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gcakqwgjg.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gliiognyl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/gwufudtra.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gfmssnsbp.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gsdmqsfeb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gjdgpnpeu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gwijassin.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gnmydtpsn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gfvubzfen.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/gwogrykun.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gipeytroi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/gnejabcpx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/grppmqbjm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gwoogbcha.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gbyaekxut.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gcwffxggd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gznuizzdq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/guxseuxqe.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gmonthelo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gasyseoao.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/grkyhwkqo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gofxerzqu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/ghrsdatiy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gxmxpstjz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gdqgxtiac.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gtozznvef.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gfkelzoho.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gvhwenloc.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/guzwfcxqo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gtqgqccph.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gkosiwygf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gqmivqxfz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/gntlxvxed.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gsijlleci.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gdwjcfsqe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gmlvysowi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gicufdfoj.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gfxogonba.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfbnoookf.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/guxafztfb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gsuuqaqlo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gzfoevbxq.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gwssrziye.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gftffibzn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gvxjvymhd.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gtcftqyjf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gpijlkkgb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gacfrorjk.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gleysnpul.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gmlmngdcv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gnzrhowms.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/guwtuhgqs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gdkitluka.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gqlcrlonv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gsjhjaazo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gzonrqnkp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/glcjewqsa.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gxemwbrcx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gvusbmmyo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/goirngeii.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/ggstbzfic.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gjueajtbl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gbbmskidd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/goaqriqzw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gslaijbjt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/grxhcfpaq.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gzfljeezj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gzyuchcfk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/glqplymur.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gjbcqyisi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gvzwzfxbl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gkazpndyu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gojddcwqb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gugftnlxd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gnnkqoqdt.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gvzqvcyha.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gjwpkrvdo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gkkmwqbja.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gwqxeutjt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gxkjquwkf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gzfdxupre.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gisxnceyu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gtxvnsnwh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gjwdoauxv.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/grewngmbr.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gnmnaebrc.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/guawemqpe.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gxckjwmqi.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gyzuecixy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gwldboiai.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gqfuqzrpl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/goqjbbevo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gbllucljp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gyhqxwacu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/ggauqlmet.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gpxpsqbrq.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gzadnobke.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gjcwprtei.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gyhnynhow.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gwfjmsaaa.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/grmwptgps.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/ggjwqfwse.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gyhxwpvjw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gqamcjijj.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gvwuvjugg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gzztpjafc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gbylyjjjl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/grflrtlan.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gvmoewchp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gbkruxcxx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gscoalctk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbbtfdbxj.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gecxkrqxr.sHtML


<!-- 参考信息 -->