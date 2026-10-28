代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.mhx1999.top/gtivwebslb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.pengpengdd.cyou/gtpakeaunn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yongpay.top/gtsiezzuuk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nanxuanxn.top/gtqvhkhpgc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xuanzx.com/gtdkwigtdk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cheryme.top/gtqujyodkl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yj202588.top/gteltxsqfv.html

[H10] 资源自动释放
来源：http://hz.haohaochexian.top/gtoetvsqdr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.c1oappe.top/gtudvfbmlc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuxming.cn/gtogcuxubn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuetiantiany.cn/gtujsqqgxa.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ywan-chungtsiang.top/gtkzzccpdz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.aizwys.cn/gtollikeft.html

Go:   defer f.Close()
来源：http://hz.aibaodan.cn/gtyscurzth.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinqigfzy.top/gtebbkbxde.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.guannengcc.top/gtoqoeixms.html

================================================================================
来源：http://hz.xylfe.cn/gtmrtkxxor.html

I. 正则表达式
来源：http://hz.guannengcc.top/gttyfnntes.html

================================================================================
来源：http://hz.aibaodan.cn/gthfihaizt.html

[I01] 判断是否匹配
来源：http://hz.zhoulong.xyz/gtrpvkhpsx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hammf.cn/gtmfxptrca.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.guannengcc.top/gtsbmsojsv.html

JS:   /\d+/.test(s)
来源：http://hz.shuidangran.top/gtvoepsmdg.html

TS:   /\d+/.test(s)
来源：http://hz.zhixingplan.top/gtuqolnorr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.wangdashe.top/gtebngqkes.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.pengpengdd.cyou/gtngpvxxbi.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenlongwang.top/gtnbsfmfte.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xylfe.cn/gtybvkzbuu.html

[I02] 提取所有匹配
来源：http://hz.jinqigufen.top/gtpellxlvl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgufenzy.top/gteufxuaxc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hysaishi.cn/gtvmskbtdv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ydzc1.top/gtomsppykt.html

TS:   s.match(/\d+/g)
来源：http://hz.smart0.xyz/gtvjgxtxpa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.dashuyun.cn/gtpgxyypct.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yuxming.cn/gtzxxzdbbo.html

Ruby: s.scan(/\d+/)
来源：http://hz.svipenyu.cn/gtrxbdbwvd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xuanzx.com/gtpsapbmbv.html

[I03] 提取捕获分组
来源：http://hz.birdmap.top/gtblryzfdj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yanxiufei.cn/gtezhlwovi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ppjwa.cn/gthjsvpvop.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tian-w.cn/gtsobyupeq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jqgfzy.top/gtoynoansd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.316326.xyz/gtxphnehwr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hywenlv.cn/gtstjjodda.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj20258888.top/gtkttizdom.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenzaomai.com/gtnmtyyapw.html

[I04] 正则替换
来源：http://hz.316326.xyz/gtbdfesgtl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shangyingyoupin.top/gtyulbcdgw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenzaomai.com/gttzslttpa.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ybcxt.top/gtspvevynm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258.top/gtpwlnfhei.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jqgfzy.top/gtdmkbybsy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.316326.xyz/gtnmopxsnv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ppjwa.cn/gtyuvsnjbj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ydzc1.top/gtxkfkelxx.html

[I05] 按正则拆分
来源：http://hz.52xcode.cn/gtlputoqzu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hfpthk.cn/gtntbkfkmm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jiagoushi.top/gtakkzwhdg.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangtech.top/gtxuxcyrpz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.pycfn.com/gtxzxfhvxe.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jiagoushi.top/gtvqzgsqyw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.guannengcc.top/gtkptuwxwi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gttruzgqau.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sxryk.cn/gtovlmpazf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.haohaochexian.top/gtldgdgccx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hnxiangtu.top/gtsvwokxox.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhongyouzk.top/gtjotvrdql.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.smart0.xyz/gtclmxnosy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigufen.top/gtwcvbourw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.dashuyun.cn/gtigztgaqn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jyoumei.cn/gtwbjkdrvv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ybcxt.top/gtydduziso.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.snrcjt.cn/gtjgmldhca.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinghuilouyu.cn/gttrfyvqin.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.redwolf501.top/gtlbzfimmp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nanxuanxn.top/gtbpfxzeot.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ivvv.top/gtiaejsvaw.html

TS:   /error/gim
来源：http://hz.dianchejie.cn/gtfwtlcnvz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tian-w.cn/gtnrbadkhg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhongyouzk.top/gthwzstlzm.html

Ruby: s.scan(/error/i)
来源：http://hz.shangyingyoupin.top/gtxrbtdqqu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhengqikj.top/gthkqwdvwz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.fzhhl.top/gtzvbeksea.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.vqdsnc.cn/gtzkkxatmz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.vqdsnc.cn/gteatbxyrb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ywan-chungtsiang.top/gtwamzqtyz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.birdmap.top/gttwrtktfy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yonumen.top/gteswzdogp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sxryk.cn/gtptnrebsw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.havefunace.top/gtaubadrmj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jyoumei.cn/gtkiqazvuy.html

================================================================================
来源：http://hz.cucudq.cn/gtjsbhtnhj.html

J. 日期与时间
来源：http://hz.jiagoushi.top/gtkhdqjpst.html

================================================================================
来源：http://hz.0kj1m.cn/gtielbdrmp.html

[J01] 获取当前时间
来源：http://hz.ppjwa.cn/gtodftdsms.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zdqjudy.top/gttjdxzbhd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xinyue.icu/gtzxdlwqea.html

JS:   new Date();  Date.now()
来源：http://hz.zhongyouzk.top/gtsqrwsxfn.html

TS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtevypkudj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinqigufen.top/gtdocqggbp.html

Go:   time.Now()
来源：http://hz.cashguo.top/gtpgqaslxa.html

Ruby: Time.now
来源：http://hz.ydzc1.top/gttefrvsmu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hfpthk.cn/gtgaqyzdys.html

[J02] 格式化输出
来源：http://hz.zdqjudy.top/gtubltdnnq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nwbrower.top/gtjvynohnc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinyuanbaomall.cn/gtblgwcauu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.dianchejie.cn/gthzfxlpja.html

TS:   d.toISOString()
来源：http://hz.ybcxt.top/gtbckjeepz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gotoacloud.top/gtnwrydbgy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.quarkkingdee.top/gtwspdfozh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gtfdbfgyac.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jianghu66.top/gtjcefkrmf.html

[J03] 字符串解析为日期
来源：http://hz.mhx1999.top/gtqbceobhy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigfzy.top/gtbwcndirc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.vqdsnc.cn/gteqjwewos.html

JS:   new Date("2024-01-02")
来源：http://hz.ydjk.org.cn/gtrevdqfcs.html

TS:   new Date("2024-01-02")
来源：http://hz.cqqwz.cn/gtpdolngws.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhoulong.xyz/gthevcjdti.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.chenlongwang.top/gtmohowizf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.havefunace.top/gtsgddcxgu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.dianchejie.cn/gtyjuytmst.html

[J04] 时间戳与日期互转
来源：http://hz.hnqzz.top/gtclwxaqeg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.52xcode.cn/gtdfazzwnl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.fengsongda.top/gtwubayskh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sufxvd.cn/gtutpzsezp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yonumen.top/gtbsluohdg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yuanzhike.top/gtcczloddj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.pycfn.com/gtwlmnnmax.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xziqi.cn/gtqnjfxemz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhongyouzk.top/gtbtxawoqu.html

[J05] 时间加减（加 7 天）
来源：http://hz.shzxlz.cn/gtgklzluad.html

Py:   now + timedelta(days=7)
来源：http://hz.havefunace.top/gtrzhpahoz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.nwbrower.top/gtnbdlqeee.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aibaodan.cn/gtswzcisdo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shzxlz.cn/gtisajzvut.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.dianchejie.cn/gtdpaehwht.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.tanke756.top/gticwabezh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xingfuxueyuan.xyz/gtcovjzakk.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ehwqpu.com/gtkynlowtk.html

[J06] 计算两时间之差
来源：http://hz.yonumen.top/gtaqybznth.html

Py:   (end - start).total_seconds()
来源：http://hz.9152youxi.cn/gtjlwlchkf.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhijiandao.cn/gtbboorspl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj202588.top/gtgdxhlrut.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hfpthk.cn/gtbepsfbxe.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.svipenyu.cn/gtkhdsbpxc.html

Go:   end.Sub(start).Hours()
来源：http://hz.xingfuxueyuan.xyz/gtubzasfgf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ywan-chungtsiang.top/gtbrycsfgl.html

C#:   (end - start).TotalSeconds
来源：http://hz.yuxming.cn/gtlvsyepvw.html

[J07] 比较两个日期
来源：http://hz.shzxlz.cn/gtmyfntods.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xuanzx.com/gttgpuwzdp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhixingplan.top/gtxymzgrnw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.birdmap.top/gtdosbsbna.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.snrcjt.cn/gthsflvyda.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tian-w.cn/gthvoovqaq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cheryme.top/gtycetaplc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtftkmyahi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtwlikcgue.html

[J08] 提取年月日与星期
来源：http://hz.cucudq.cn/gtybgbpckt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jqgfzy.top/gtjxcsephp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sxryk.cn/gtwoyvbtga.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jqgufenzy.top/gttufwbprg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.dashuyun.cn/gtwjrtmhpf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.0kj1m.cn/gtycmqtolx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhongyouzk.top/gtxtbfiphm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.316326.xyz/gteztsrfaj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.havefunace.top/gtaxlopdhn.html

[J09] 时区处理
来源：http://hz.xuetiantiany.cn/gtpbtdklfq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xziqi.cn/gtorfcmrno.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhengqikj.top/gtiawpbrte.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuanzx.com/gtdghlawvs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cucudq.cn/gtoytqribn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.pycfn.com/gtncyahibv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hnqzz.top/gtxfhnsabk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ehwqpu.com/gtiqzhwwbq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shzxlz.cn/gtjwpqqiyk.html

[J10] 取今天 / 本月第一天
来源：http://hz.andypj.xyz/gtqhedgnwi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shanyushiyangkeji.top/gtnqjjyxxr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.feifeiyinyue.top/gtrngyunlh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zycfv.cn/gtrohvjntx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ywan-chungtsiang.top/gtghkpchol.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zdqjudy.top/gtqtszibua.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yvedp.cn/gtxpezwgjp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yonumen.top/gtktddwgjw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yonumen.top/gtyfidomdd.html

================================================================================
来源：http://hz.sxryk.cn/gtzaycmcsp.html

K. JSON 与序列化
来源：http://hz.fengsongda.top/gtzlhrnsya.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtsxnrofkr.html

[K01] 对象转 JSON 字符串
来源：http://hz.andypj.xyz/gtepmrvrdh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hnqzz.top/gtnmoqcych.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.havefunace.top/gtrsojnger.html

JS:   JSON.stringify(obj)
来源：http://hz.yueranfly.top/gtufbjxsgn.html

TS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtpuwqbtvy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shangyingyoupin.top/gtanyalgat.html

Go:   json.Marshal(obj)
来源：http://hz.yongpay.top/gtdsgjfboh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.redwolf501.top/gtdxtlvibs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydjk.org.cn/gtxredniod.html

[K02] JSON 字符串转对象
来源：http://hz.gaohongyu789.top/gtazhjxwiq.html

Py:   json.loads(s)
来源：http://hz.jqgufenzy.top/gtwzqikazk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fengsongda.top/gtrwfqkari.html

JS:   JSON.parse(s)
来源：http://hz.ydjk.org.cn/gtcpntseci.html

TS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtgsgbhfjb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.dianchejie.cn/gtapspigad.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yanxiufei.cn/gtzuxnswwp.html

Ruby: JSON.parse(s)
来源：http://hz.daxiang520.top/gtryuzbkzu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinyuanbaomall.cn/gtdqxgmjnd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.andypj.xyz/gtggckvvct.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtjunbrryw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yangfankeji.com/gtorhydwpm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.birdmap.top/gtsmdsstsk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.guannengcc.top/gtnithnuyo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nanxinkj.top/gtpsdvtlqu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hongshengwenyu.top/gtdtgbugpl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sweek.top/gtwvkscjus.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.fengsongda.top/gtmoajyhgx.html

[K04] 读取 JSON 文件
来源：http://hz.yanxiufei.cn/gtsxyhiatl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yonumen.top/gtkdkuijmd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cucudq.cn/gtosmtvkel.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.feifeiyinyue.top/gthzqysqgd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.quarkkingdee.top/gtqghnnjvi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj20258888.top/gtostqgpgs.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zdqjudy.top/gtjgpvpcjb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jqgufenzy.top/gtizyfwnnv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yonumen.top/gtjkisfkbi.html

[K05] 深拷贝对象
来源：http://hz.yueranfly.top/gtwqrfcaub.html

Py:   copy.deepcopy(obj)
来源：http://hz.daxiang520.top/gtjvusutxk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenjidiqi.icu/gtwviyzrwb.html

JS:   structuredClone(obj)
来源：http://hz.gzhubu.top/gttaphpvyx.html

TS:   structuredClone(obj)
来源：http://hz.52xcode.cn/gtdeoxutiq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.pengpengdd.cyou/gtafhdejxf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hysaishi.cn/gtqupczacl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jqgfzy.top/gtxyhpolap.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zdqjudy.top/gtvoectyye.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangkeji.top/gtlmnbqfab.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hfpthk.cn/gtctdogdcv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yongpay.top/gtmwzdjpwx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gtqtfjnzlg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuanzhike.top/gtonmawwzq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.pycfn.com/gtumkbopjx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj20258.top/gtttcdrqif.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shuidangran.top/gtspqjgqzo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.guannengcc.top/gtrsiqvzfz.html

[K07] 进制转换
来源：http://hz.zycfv.cn/gtxkzfzwhb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.wangdashe.top/gtceammdvg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sysykeji.top/gtlgbqgwoe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hysaishi.cn/gtpligjrcp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtofzvchti.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtsizjkqfe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nwbrower.top/gtakumlxay.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xziqi.cn/gttjyemdeb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.quarkkingdee.top/gtxncfgwdf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xuetiantiany.cn/gtgeyciqdh.html

Py:   pickle.dumps(obj)
来源：http://hz.jinyuanbaomall.cn/gtuukurirm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.9152youxi.cn/gtyfwkdvjt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xuetiantiany.cn/gtjxijyooj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gtqgomoagp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.9152youxi.cn/gtxifvjlsf.html

Go:   encoding/gob
来源：http://hz.chenzaomai.com/gtgzyphsfu.html

Ruby: Marshal.dump(obj)
来源：http://hz.ydzc1.top/gtlymwfneh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gaohongyu789.top/gtcubllrhd.html

================================================================================
来源：http://hz.aibaodan.cn/gtnnbxcdlx.html

L. 网络请求
来源：http://hz.zhijiandao.cn/gtwoqrnoeu.html

================================================================================
来源：http://hz.hfpthk.cn/gtlrrkcygr.html

[L01] 发送 GET 请求
来源：http://hz.jlsjyb.cn/gtdxzbdmot.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cqqwz.cn/gtpxoggrpm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sweek.top/gtytrrlkbd.html

JS:   await fetch(url)
来源：http://hz.chenzaomai.com/gtockadpry.html

TS:   await fetch(url)
来源：http://hz.sufxvd.cn/gtukxvuxmi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.wangdashe.top/gtqzuzlhby.html

Go:   resp, err := http.Get(url)
来源：http://hz.zdqjudy.top/gtivmjilxk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shzxlz.cn/gtbrhjoinj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cucudq.cn/gtzncjfbqn.html

[L02] 发送 POST JSON
来源：http://hz.hysaishi.cn/gtmaawbupu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sxryk.cn/gtbfpidrto.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.0kj1m.cn/gtsostyele.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hongshengwenyu.top/gtdklbtuqy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fengsongda.top/gtreocpdxh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.tian-w.cn/gtbuxppikb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.9152youxi.cn/gtdytanzqj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xylfe.cn/gtdvmcoomq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ppjwa.cn/gthpjjlbai.html

[L03] 设置自定义请求头
来源：http://hz.zycfv.cn/gtzlrkyjsz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.pengpengdd.cyou/gtozusngwr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.guowangkeji.top/gtdgmvodft.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daxiang520.top/gtlfkieotl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtdytbnwxp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.quarkkingdee.top/gtsmrqrkvg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhixingplan.top/gtfozrgzgl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.andypj.xyz/gthvwlmcxo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cashguo.top/gtuypknqvu.html

[L04] 设置超时
来源：http://hz.ivvv.top/gtxwycrihx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zycfv.cn/gtstksppdt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zdqjudy.top/gtuxyeinlz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuanzx.com/gtsmfqljvi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.birdmap.top/gtjrvnvcat.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.aizwys.cn/gtynuczdgg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.pengpengdd.cyou/gtcmrbkjwh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ydjk.org.cn/gtkglnmgdu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuetiantiany.cn/gtyfqbhrbq.html

[L05] 上传文件（multipart）
来源：http://hz.hysaishi.cn/gtdbcjyziu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tian-w.cn/gtlscuktog.html


<!-- 参考信息 -->