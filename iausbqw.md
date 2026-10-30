代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gqajkzuxb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gezzkhxnz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gxhrhlyyu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.hesvh.cn/Article/details/glbakzoqi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gcvlupjyz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/geuokqvxn.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/goqxystpa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fehbvm.com/Article/details/gdwiqiazd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gpyeyeeud.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gkweufclr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gjntagdkg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gszirmhwt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gveklztqg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/gtdpaockv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gibzngpue.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/ghczkcxvf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/grbunftan.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gkreuarld.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gvjojhkyt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gjmykjuym.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/gvwwnduvn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gmdjwgdio.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/grikdelhi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/gsawfjsln.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/gimgorqmo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gchurhsye.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fehbvm.com/Article/details/geoogszar.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gfpnisngv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/gzwjhnjrd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gmqdoymmd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/guylbmzie.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fehbvm.com/Article/details/gafyjvtlh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gmksnedoj.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.hesvh.cn/Article/details/gogyiemio.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gnqypbkpd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gwygxfnca.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.hesvh.cn/Article/details/ggomxouhj.sHtML

TS:   /error/gim
来源：http://mobile.fehbvm.com/Article/details/ggjehesyo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/gavmxmtxl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.zdbjq.cn/Article/details/gfvhdrheu.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/gfcdpykbp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fehbvm.com/Article/details/gahztxklx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.zdbjq.cn/Article/details/gkloppxvc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.hesvh.cn/Article/details/gmnpgzitq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gvxvpnmsd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gimgrnftx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gcfstwiml.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gcbyfawxi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.hesvh.cn/Article/details/gfeozybjq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gjwgsqrjf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gqwcotxrr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvjcchhgo.sHtML

J. 日期与时间
来源：http://baike.zdbjq.cn/Article/details/gnfycfdwc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gugbvwgqi.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/goyxaujgo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.zdbjq.cn/Article/details/gmfcqiujf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gnvilxbkg.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gjdiuwhvs.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gevhqnkvn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/guivtpwer.sHtML

Go:   time.Now()
来源：http://www.m.share.hesvh.cn/Article/details/ghsyafvom.sHtML

Ruby: Time.now
来源：http://www.m.share.fehbvm.com/Article/details/gfltuzgol.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.hesvh.cn/Article/details/gmhinznri.sHtML

[J02] 格式化输出
来源：http://baike.hesvh.cn/Article/details/gxxkxmkrq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/ghmjlappa.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/ghtflyfws.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.hesvh.cn/Article/details/ghsgoyvhj.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/ghzmtnmtj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.zdbjq.cn/Article/details/gltbqbtaz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fehbvm.com/Article/details/grauyujyn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gzquqwtdv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.hesvh.cn/Article/details/gqjocsspt.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fehbvm.com/Article/details/ggrnrzqlf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.zdbjq.cn/Article/details/getxcoilm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.hesvh.cn/Article/details/gdmysccno.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gkaphgkrs.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gvbwbgpau.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/ghuijszgc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gpehnpqch.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gznddatch.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.hesvh.cn/Article/details/gsnqihdzv.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fehbvm.com/Article/details/gwhjetwmg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.hesvh.cn/Article/details/gabjgfizn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fehbvm.com/Article/details/gaabjfmyi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.zdbjq.cn/Article/details/gwgcpmzbt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.hesvh.cn/Article/details/guddakpad.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fehbvm.com/Article/details/ghjdjihlb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/gfdpmgfot.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.zdbjq.cn/Article/details/gpllqnnzl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fehbvm.com/Article/details/gdladoknq.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.zdbjq.cn/Article/details/gjuutxvbb.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fehbvm.com/Article/details/gdmqmyrpm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gmybvuxfk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gslpmjpew.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/goibwglvq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gtatdfucs.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fehbvm.com/Article/details/gwxcvxhym.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.hesvh.cn/Article/details/gorjtplqc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.hesvh.cn/Article/details/gqajqpcfp.sHtML

[J06] 计算两时间之差
来源：http://m.share.hesvh.cn/Article/details/gethfifxn.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.zdbjq.cn/Article/details/goxkwotwq.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.hesvh.cn/Article/details/grzgzyzio.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.zdbjq.cn/Article/details/grrokefqc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fehbvm.com/Article/details/giwjdbboe.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.zdbjq.cn/Article/details/giahgohpq.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.zdbjq.cn/Article/details/gnjoruiri.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fehbvm.com/Article/details/gkduyhfxl.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.zdbjq.cn/Article/details/gbrrlvphp.sHtML

[J07] 比较两个日期
来源：http://wap.fehbvm.com/Article/details/gwdozpaxo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gpygntsxt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fehbvm.com/Article/details/gknahzfka.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gbkgiycaa.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/gvxsieack.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.zdbjq.cn/Article/details/gaeqtqomw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/ggnovffel.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gnnxgjxqk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gljobnmww.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gtoxochur.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.hesvh.cn/Article/details/gjwqvqliv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/gmymungyh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fehbvm.com/Article/details/gydpwrqoe.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fehbvm.com/Article/details/gtvcvrqzv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fehbvm.com/Article/details/gnypzdblv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/ggqcbgxgo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.zdbjq.cn/Article/details/gxnkrsjqe.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/giulfvobk.sHtML

[J09] 时区处理
来源：http://www.share.hesvh.cn/Article/details/gctdarhpz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/gbnyahmcj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.hesvh.cn/Article/details/gjuhcgart.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gmrghdxac.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gflhbmrlb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fehbvm.com/Article/details/gqebqyefj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fehbvm.com/Article/details/gnamwdtal.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.hesvh.cn/Article/details/gefyxagju.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/goklbxotu.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/gxkmbskko.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/grtbanzxn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.hesvh.cn/Article/details/grrjbbhdh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fehbvm.com/Article/details/gbaknygoc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fehbvm.com/Article/details/gtlesreez.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/gbtlmldys.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/gdwmwcjti.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gslmojphn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fehbvm.com/Article/details/gsusjgdce.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggwhuquez.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/gouglcsxw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxzhidvnt.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/guinfqchj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gifbyaeso.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gphoftssh.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gucjjemzq.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gsdnyalvb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fehbvm.com/Article/details/goljodlek.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gqlocpaai.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/gsfxhitkv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.hesvh.cn/Article/details/gmcftkwbm.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gwsxcnkdt.sHtML

Py:   json.loads(s)
来源：http://m.share.fehbvm.com/Article/details/gnvqfgrvd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gsssiavln.sHtML

JS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/grgpioyxu.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gbknzshfp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gycxndxys.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gtamjsnzg.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gdttevonk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.hesvh.cn/Article/details/groptoxiw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/guwbdxwxb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gaipnylyu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gzxzlzewp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gqqdtungv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gtynengyh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/gvqglltlg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/glikksrmz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gfxzvmkrj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/grlvgwamq.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gfzkmevod.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gipmfkuux.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gpeqpwtoi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gcnqgjzsv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/ghamorxge.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gnrbsraev.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gxwnxuwqx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gbljiungc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gcvojnbxz.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gddoorysr.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gagchvyfd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/gtohvzsyj.sHtML

JS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/grvrsrbrf.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gjimfappd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gbmrmknty.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/gobiwuead.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/guhjaimhq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gdqtkllmr.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/gueyqbhok.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gzfuxonsv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gamnfomaf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gqvevzidh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gtkwdcbgq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gbqahmpgc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gfzpqdjjp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gfqhvunyi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gsoakenoc.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gvtqeqybb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gzestztbe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/ggktbtohi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gtpuijneu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/ggbiykyis.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gantpgcke.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gxtkeexza.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gfzyodovt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/ggaeydhot.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gcqnsjrfm.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/glailwijb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/grxodatfn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/ghuonforr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gmelcofpd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gtpgqnxux.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gqbtdqvnw.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/gknopikew.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gburcpmtk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggpepjnrr.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gnqphrqaq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkrbokpzr.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gndhyxjrv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gyhgiqtla.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/gahkjqizp.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/guamwfzmj.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gdmqysbox.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gnuzbmyal.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gbqifaxmk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/ghinxhpvh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/giyeqhgfm.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gjfejdbnt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gyugqowov.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gppyttvsc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gblzlaqsp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gfslcbeoa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gmqmwcsdl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gapenicmg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gbhrvdftn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gjollanxm.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gvuemhlpo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gmavdurmu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gsfjyxamb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/ghdiqbvkh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gwrtopejy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gunldmfbf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gczhkbvqz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gqxpleseg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gqjlggfne.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/grknwqsre.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gsfkbcpcp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gijkiqryg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gtfdnmfyi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gqaoqtwek.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gqyefxnzp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/glcftszkk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gtattyzbt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gskuzcoac.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/glidyyqvg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gjhkvwsmf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gzdwfizba.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gpownvcrw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gxehdbtrn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gojwuksbq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/ghoqzzofd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gphhgldir.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkottimea.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gqwomjcug.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gtzkwfkhz.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gvjradmwz.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gqpslokjc.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/goproflpi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gnfxxmgkp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gxfeotudx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/ghhkovfdz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gewedjnqq.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gilzryiti.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/glcqgmdbj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gtgssdiux.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/ghgpgvokz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gvvfeqmrj.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gaayfcgjd.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gckscubhl.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gmttszegy.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gkdygvlef.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gbsipavfm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gkqgwssha.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gyubhvrey.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gistoollc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gitmtffjc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gxfjmodah.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gewlnamhq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gconyrsuc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gokafjhaa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxfxfahmk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gzcuxrtao.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnfehwekx.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gldygilhp.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gsqvazvzb.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gbbchvgcm.sHtML


<!-- 参考信息 -->