代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenzaomai.com/gtxmskqrmf.html

Go:   defer f.Close()
来源：http://hz.zhongyouzk.top/gtahgrqrtl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.chenzaomai.com/gttppptqak.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ivvv.top/gtzyqndbic.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtfepvxnmh.html

I. 正则表达式
来源：http://hz.9152youxi.cn/gtvxqkxobg.html

================================================================================
来源：http://hz.ivvv.top/gtcxvxjksl.html

[I01] 判断是否匹配
来源：http://hz.zhongyouzk.top/gtyvzyxwua.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.kuanghao11.cn/gtinqjqdlc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.mhx1999.top/gtwoxsrdgj.html

JS:   /\d+/.test(s)
来源：http://hz.yuxming.cn/gtyawrkzmk.html

TS:   /\d+/.test(s)
来源：http://hz.tanke756.top/gtdedtzcou.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.smart0.xyz/gtrbpubnjr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xziqi.cn/gtydcqpjro.html

Ruby: s.match?(/\d+/)
来源：http://hz.jqgfzy.top/gtdbspyvsv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ppjwa.cn/gtpkjhtnum.html

[I02] 提取所有匹配
来源：http://hz.andypj.xyz/gtilezayof.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinqigufen.top/gtzoektjkg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.birdmap.top/gtwqabbbeb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuetiantiany.cn/gtszkwdgxm.html

TS:   s.match(/\d+/g)
来源：http://hz.316326.xyz/gtopmcehib.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xylfe.cn/gtvhkhvujb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinghuilouyu.cn/gtfrxhhkpm.html

Ruby: s.scan(/\d+/)
来源：http://hz.ywan-chungtsiang.top/gtbtimrbon.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.fengsongda.top/gttpmioipg.html

[I03] 提取捕获分组
来源：http://hz.zdqjudy.top/gteabaqhjr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gotoacloud.top/gtmwrfllyo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.havefunace.top/gtoevepznd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xuanzx.com/gtbjddyeqf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cheryme.top/gtnhphnmpl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ppjwa.cn/gtxymcgafj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tian-w.cn/gtilxxowon.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cheryme.top/gtotujjxrw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhongyouzk.top/gttffflyre.html

[I04] 正则替换
来源：http://hz.mhx1999.top/gtzjhxrzrn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xingfuxueyuan.xyz/gtsidkvdwy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.svipenyu.cn/gtrxsqwlgk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.dianchejie.cn/gtjpesfpiq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jlsjyb.cn/gtjssrarwf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sysykeji.top/gtwgbktakj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.meibo888.top/gtfpofvvks.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ehwqpu.com/gtcxqcoith.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yvedp.cn/gtagsqfrdf.html

[I05] 按正则拆分
来源：http://hz.hywenlv.cn/gtdkcsxmge.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xylfe.cn/gtrbyhmkzs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hongshengwenyu.top/gtuocifikl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtqvbobwzk.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtrzoqaxsx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.guowangkeji.top/gtfozeqzem.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhijiandao.cn/gtlmmisilj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtlzciwuqb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.mhx1999.top/gthuwmjwax.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxuanxn.top/gtfhjqkomh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgfzy.top/gtagxomiud.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yanxiufei.cn/gtzjkktpyy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gtevdvfuzu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtfsviysco.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenzaomai.com/gtmizoxmrh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shuidangran.top/gtcehwbuqk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhongyouzk.top/gtvjiwqkte.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.snrcjt.cn/gtoxdefeuh.html

[I07] 忽略大小写与多行模式
来源：http://hz.nanxinkj.top/gtehrxvaox.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.daxiang520.top/gtfiskmnys.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gzhubu.top/gtdcubuwmx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.dianchejie.cn/gtrdxkwfkc.html

TS:   /error/gim
来源：http://hz.mhx1999.top/gtttndhsag.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.birdmap.top/gtvtzgfkba.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.aizwys.cn/gtaagksafo.html

Ruby: s.scan(/error/i)
来源：http://hz.shanyushiyangtech.top/gtwsygfvzk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yangfankeji.com/gtturiquli.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cucudq.cn/gtalyzlpyl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xingfuxueyuan.xyz/gthemyhzqs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.quarkkingdee.top/gtlpkozmnw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hammf.cn/gttjiysxhq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cheryme.top/gtgxdpmjgt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yueranfly.top/gttaepiyay.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.aibaodan.cn/gtauldztrj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sweek.top/gtewbanztn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gaohongyu789.top/gtkuxexxyk.html

================================================================================
来源：http://hz.cqqwz.cn/gtdtnbeevm.html

J. 日期与时间
来源：http://hz.zhengqikj.top/gtpwnvzels.html

================================================================================
来源：http://hz.quarkkingdee.top/gtuatbppdc.html

[J01] 获取当前时间
来源：http://hz.yongpay.top/gtpjxjvarz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sysykeji.top/gtncyzvkun.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.0kj1m.cn/gtivhpfjbe.html

JS:   new Date();  Date.now()
来源：http://hz.zhoulong.xyz/gtuzwqklhg.html

TS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtstzaknac.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jyoumei.cn/gtctuuhzvj.html

Go:   time.Now()
来源：http://hz.guowangkeji.top/gtqpuudiqb.html

Ruby: Time.now
来源：http://hz.pengpengdd.cyou/gtqcknwyuh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jyoumei.cn/gtarwneddt.html

[J02] 格式化输出
来源：http://hz.gotoacloud.top/gtavsuwozr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.bjfxy.top/gtlkzqqior.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenlongwang.top/gtfvdbaeym.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yangfankeji.com/gtlmtzmnql.html

TS:   d.toISOString()
来源：http://hz.guowangkeji.top/gtjzroinkk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yueranfly.top/gtbonoiujj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sweek.top/gtxjhkfyom.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuanzhike.top/gtopgzpmpl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.52xcode.cn/gtpebcpnsx.html

[J03] 字符串解析为日期
来源：http://hz.gotoacloud.top/gthaxsaieh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.pycfn.com/gtphgyvryl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xinyue.icu/gtombwpcwk.html

JS:   new Date("2024-01-02")
来源：http://hz.sysykeji.top/gtwpilrqpt.html

TS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtixcuqrmc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yongpay.top/gtbjsbgbmb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sufxvd.cn/gtsxvkcdvt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daxiang520.top/gtmjscgsvp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xuanzx.com/gtmtjnviyo.html

[J04] 时间戳与日期互转
来源：http://hz.yj20258.top/gtndppodpx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hammf.cn/gtefuxafag.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jianghu66.top/gtimvsyiuc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.vqdsnc.cn/gtplqcctgr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shzxlz.cn/gtwmbpewgy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yvedp.cn/gtpyljxdwy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nwbrower.top/gtforygxbd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yuxming.cn/gtamwovauz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sweek.top/gtjvqfgvgb.html

[J05] 时间加减（加 7 天）
来源：http://hz.havefunace.top/gtwkfvvkdr.html

Py:   now + timedelta(days=7)
来源：http://hz.jlsjyb.cn/gtoufpnaxe.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhoulong.xyz/gtoeghwpuv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.birdmap.top/gtfelwdqey.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.haohaochexian.top/gtivaahfac.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhongyouzk.top/gtgwlwbpzb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.pengpengdd.cyou/gtaggulobu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xinyue.icu/gtpbtjvgzw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shanyushiyangtech.top/gtetycjeir.html

[J06] 计算两时间之差
来源：http://hz.sxryk.cn/gtovgkkgbo.html

Py:   (end - start).total_seconds()
来源：http://hz.jinghuilouyu.cn/gtkgjcoscm.html

PHP:  $end->diff($start)->days;
来源：http://hz.jqgfzy.top/gtdwukqdhl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.andypj.xyz/gtikhnoyxp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xylfe.cn/gtckrlbqfa.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ybcxt.top/gtystiyiiv.html

Go:   end.Sub(start).Hours()
来源：http://hz.dianchejie.cn/gtxvffnuif.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenjidiqi.icu/gtzxcezdju.html

C#:   (end - start).TotalSeconds
来源：http://hz.sufxvd.cn/gtlpmjwlnr.html

[J07] 比较两个日期
来源：http://hz.ehwqpu.com/gtbudngurv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtiqlrtiek.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.pengpengdd.cyou/gttxmhqnwa.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigfzy.top/gtppwsuzwe.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangkeji.top/gtkjraoxnc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.pengpengdd.cyou/gtyyxktolp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nanxinkj.top/gtxiacmhxh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gtvbvntikt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtvzpldlqp.html

[J08] 提取年月日与星期
来源：http://hz.meibo888.top/gtqwunabtn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hnqzz.top/gtrruaoxtg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.svipenyu.cn/gtmddhoqek.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinghuilouyu.cn/gtvfdjsyxa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hammf.cn/gterjngbei.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.c1oappe.top/gtpwrnxwax.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zycfv.cn/gtqlhbellg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hammf.cn/gtlycxdrxz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zdqjudy.top/gtofgvgngq.html

[J09] 时区处理
来源：http://hz.ybcxt.top/gtuwlkxlaa.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nanxinkj.top/gtsagadifn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sysykeji.top/gtiktkyhqt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtzevljlqk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.andypj.xyz/gtyrddzbrg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhongyouzk.top/gtjpdcgddn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sysykeji.top/gtzsdgndla.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj20258.top/gtyodnazlf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.vqdsnc.cn/gtcmsiczns.html

[J10] 取今天 / 本月第一天
来源：http://hz.316326.xyz/gtnxigxsvg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhijiandao.cn/gtmvbiecxs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.aizwys.cn/gtutcibjwv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cdnleiting.top/gtnqshaddr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.haohaochexian.top/gtggwkjpgg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.quarkkingdee.top/gtuvxlqjil.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.feifeiyinyue.top/gtyhzuzkza.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.daria6918.cn/gttrychpij.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cashguo.top/gtdvkgdlri.html

================================================================================
来源：http://hz.ppjwa.cn/gtdhpvuaya.html

K. JSON 与序列化
来源：http://hz.daxiang520.top/gtdnvqsjoy.html

================================================================================
来源：http://hz.jinqigfzy.top/gtgabwitcb.html

[K01] 对象转 JSON 字符串
来源：http://hz.wangdashe.top/gtdfjcxbmn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jiagoushi.top/gtqeeivmxx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtgdagzbtr.html

JS:   JSON.stringify(obj)
来源：http://hz.shuidangran.top/gtcdwwaxcj.html

TS:   JSON.stringify(obj)
来源：http://hz.chenlongwang.top/gtjbtdxhcy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.nwbrower.top/gtwejnejqh.html

Go:   json.Marshal(obj)
来源：http://hz.pengpengdd.cyou/gttduipnpa.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.feifeiyinyue.top/gtxuqhsahv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shzxlz.cn/gtdppabiae.html

[K02] JSON 字符串转对象
来源：http://hz.nwbrower.top/gtnsostdcu.html

Py:   json.loads(s)
来源：http://hz.cqqwz.cn/gtlrtfgqtz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhixingplan.top/gtlkyenmuf.html

JS:   JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtojuqmldj.html

TS:   JSON.parse(s)
来源：http://hz.ydjk.org.cn/gtkfaobewe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jqgfzy.top/gtwidazrjz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinyuanbaomall.cn/gtmtcckxmr.html

Ruby: JSON.parse(s)
来源：http://hz.gaohongyu789.top/gthdnjsrxd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.daxiang520.top/gtfisrghuw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydjk.org.cn/gtnagxiazq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.aizwys.cn/gtoijbwhjd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.snrcjt.cn/gtopsiiuxj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenzaomai.com/gtrkrscfmx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtsolejpls.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tian-w.cn/gtncfcmhmr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhixingplan.top/gtusujwxaj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.0kj1m.cn/gtjyasikic.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgfzy.top/gtxprrwogw.html

[K04] 读取 JSON 文件
来源：http://hz.cqqwz.cn/gtwggnrunf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.havefunace.top/gtscdgrsmq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.guowangkeji.top/gtiimzgwjk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangshuangyany.cn/gtirtuyxep.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.havefunace.top/gtzqardzob.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.smart0.xyz/gtdrvyrkkk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hammf.cn/gtymdgmbrt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shuidangran.top/gtkpekitsz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.snrcjt.cn/gtppvpywni.html

[K05] 深拷贝对象
来源：http://hz.shangyingyoupin.top/gtqrycsrno.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhixingplan.top/gthfbsvydb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shangyingyoupin.top/gtzhlncdca.html

JS:   structuredClone(obj)
来源：http://hz.shangyingyoupin.top/gtglpfxyub.html

TS:   structuredClone(obj)
来源：http://hz.haohaochexian.top/gtxxfeunak.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.andypj.xyz/gtlosptplb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhaomingkeji.xyz/gtrubddjjh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sxryk.cn/gtfcmykxab.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.guannengcc.top/gtgopazwzl.html

[K06] 解析 URL 查询串
来源：http://hz.cdnleiting.top/gtzgorqvnk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.fengsongda.top/gthdzqbisq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yonumen.top/gtmhrgmdkm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yueranfly.top/gtyadyzchn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhoulong.xyz/gtoxeynypw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhoulong.xyz/gtgzmcmgwk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.quarkkingdee.top/gtjerozfzp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shuidangran.top/gteegirgny.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yongpay.top/gtpwijmnen.html

[K07] 进制转换
来源：http://hz.pycfn.com/gtxfpbjmxv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj20258888.top/gtmygqyzif.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinghuilouyu.cn/gtknijhrtm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtkjbleten.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj202588.top/gtsmypqkcc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtfaprjjtg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.wangdashe.top/gtrbozesrr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cheryme.top/gtxtjytett.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cucudq.cn/gtayciaucq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.316326.xyz/gtziupslbg.html

Py:   pickle.dumps(obj)
来源：http://hz.dianchejie.cn/gtumgvrjip.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.0kj1m.cn/gtrxvjjniz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gtmlsvahhy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jlsjyb.cn/gtuqhlfybd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.redwolf501.top/gtjgwppqwz.html

Go:   encoding/gob
来源：http://hz.316326.xyz/gtlhecfopq.html

Ruby: Marshal.dump(obj)
来源：http://hz.jyoumei.cn/gtbjqbhahz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hywenlv.cn/gtudefyfrh.html

================================================================================
来源：http://hz.xuanzx.com/gtpniuljqi.html

L. 网络请求
来源：http://hz.sysykeji.top/gtoxwnnwtk.html

================================================================================
来源：http://hz.nwbrower.top/gtklwyerqa.html

[L01] 发送 GET 请求
来源：http://hz.hywenlv.cn/gtakhpxafr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sweek.top/gtzywgieuy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daxiang520.top/gtrtzevzdr.html

JS:   await fetch(url)
来源：http://hz.xinyue.icu/gtylzohvio.html

TS:   await fetch(url)
来源：http://hz.chenjidiqi.icu/gtuhymbasa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.iojbl.cn/gtamtxdekk.html

Go:   resp, err := http.Get(url)
来源：http://hz.shanyushiyangkeji.top/gttulelvbk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nwbrower.top/gtiqibjnnj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.meibo888.top/gtuqzqapea.html

[L02] 发送 POST JSON
来源：http://hz.birdmap.top/gtbvfacdsi.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xuetiantiany.cn/gtrgtuytxc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tianlin.xyz/gtnaqumebp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuanzhike.top/gtgxvjaghj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinyuanbaomall.cn/gtjisyuavs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gaohongyu789.top/gtdhuzbcag.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hammf.cn/gtjsmmsode.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jyoumei.cn/gtexoqlvjl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sufxvd.cn/gtyilsbvkc.html

[L03] 设置自定义请求头
来源：http://hz.snrcjt.cn/gtgmgjfbvf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.aibaodan.cn/gtewjlsqyi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sufxvd.cn/gttdcqjavo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gtwzvmixpb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gtsdypngih.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yuxming.cn/gtcqnugbjs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ywan-chungtsiang.top/gtkitoozwt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.pengpengdd.cyou/gtrbttbjyu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yueranfly.top/gtrevpomev.html

[L04] 设置超时
来源：http://hz.feifeiyinyue.top/gtrqvspagx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.dianchejie.cn/gtiskwnkwa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.daria6918.cn/gtvkbsrezx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtmmyeonpx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.c1oappe.top/gtpguyqadj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ppjwa.cn/gtjssekxsf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hywenlv.cn/gtitihatvp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jyoumei.cn/gteyiduqru.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.iojbl.cn/gtfeicpzmn.html

[L05] 上传文件（multipart）
来源：http://hz.dashuyun.cn/gttbunsleh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.chenlongwang.top/gtutgdopvc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.wangshuangyany.cn/gtwfazrrsx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.kuanghao11.cn/gtjhbbdevh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuxming.cn/gtjoomffdr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sysykeji.top/gtsqbpfzdx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xziqi.cn/gtkqgihlep.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jiagoushi.top/gtbhjikfqh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yanxiufei.cn/gttrugllwo.html

[L06] 解析响应为 JSON
来源：http://hz.jianghu66.top/gtmqwhfchb.html

Py:   resp.json()
来源：http://hz.tianlin.xyz/gtslxolfdp.html

PHP:  json_decode($body, true);
来源：http://hz.c1oappe.top/gtjbjguaot.html

JS:   await resp.json()
来源：http://hz.zhiwuduotai.top/gterqtcywt.html

TS:   await resp.json()
来源：http://hz.feifeiyinyue.top/gtnxcmpjrl.html


<!-- 参考信息 -->