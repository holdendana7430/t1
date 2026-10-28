代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://hz.jianghu66.top/gtjzmphlrb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenjidiqi.icu/gtuzupywqr.html

[H09] 带错误码的异常
来源：http://hz.dashuyun.cn/gtzctibzyw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenlongwang.top/gtcuauitcw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ivvv.top/gteessstyk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tanke756.top/gthatoxqrj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yvedp.cn/gtnzlkjios.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cqqwz.cn/gtzmnjshpp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jqgfzy.top/gtkyqkobal.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.feifeiyinyue.top/gticksyqub.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xylfe.cn/gtcknfxdka.html

[H10] 资源自动释放
来源：http://hz.hysaishi.cn/gtsgpdfpcv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yueranfly.top/gtvotmdlfq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydzc1.top/gtodcqvayi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sysykeji.top/gtvamskhvt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ivvv.top/gtkwjibdpb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hysaishi.cn/gtfbwhxrew.html

Go:   defer f.Close()
来源：http://hz.cashguo.top/gtxqhiozwv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xingfuxueyuan.xyz/gtjvgeigxp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnqzz.top/gtdehcjauf.html

================================================================================
来源：http://hz.ybcxt.top/gtxwdmykki.html

I. 正则表达式
来源：http://hz.nanxinkj.top/gtzqqntpym.html

================================================================================
来源：http://hz.daxiang520.top/gtbyrbuucx.html

[I01] 判断是否匹配
来源：http://hz.pengpengdd.cyou/gtezzbqcpj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.9152youxi.cn/gtvnyqhszh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jqgufenzy.top/gtiteqboyx.html

JS:   /\d+/.test(s)
来源：http://hz.cucudq.cn/gtsttkviog.html

TS:   /\d+/.test(s)
来源：http://hz.ydjk.org.cn/gtyofyfqyw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydjk.org.cn/gtaldztpih.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xuanzx.com/gthyrhdqvd.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhijiandao.cn/gtjshliice.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xinyue.icu/gtpcqgolha.html

[I02] 提取所有匹配
来源：http://hz.pycfn.com/gtwbcdahhb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nanxinkj.top/gtmghwrfvp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258888.top/gthnatmdst.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.c1oappe.top/gtibxapgld.html

TS:   s.match(/\d+/g)
来源：http://hz.wangdashe.top/gtvjqtydfb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jlsjyb.cn/gtiqtnxpwc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sufxvd.cn/gtpoguxnyc.html

Ruby: s.scan(/\d+/)
来源：http://hz.pengpengdd.cyou/gtxyhsppho.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yvedp.cn/gttvzbdmga.html

[I03] 提取捕获分组
来源：http://hz.aizwys.cn/gtecsyqzuj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cashguo.top/gtxobdckku.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.iojbl.cn/gttdaymoiw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yueranfly.top/gthfvvbhye.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.smart0.xyz/gttofpswgz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yuxming.cn/gtcrtnvabg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.mhx1999.top/gteivalcga.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yonumen.top/gtwkbiwhsm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yueranfly.top/gtiyayqchu.html

[I04] 正则替换
来源：http://hz.birdmap.top/gtwyuytvzc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hywenlv.cn/gtwtfimlev.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.guowangkeji.top/gthsykbjoy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtgmhozicz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtojpupemx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jlsjyb.cn/gthvxuvptj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhixingplan.top/gttcbgmicx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhoulong.xyz/gtcygptraw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.chenzaomai.com/gtecbyiddx.html

[I05] 按正则拆分
来源：http://hz.sweek.top/gtkqjalilh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.chenjidiqi.icu/gttclsmfkz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yj20258888.top/gtkacgeckq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangtech.top/gtfqjnbujg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtnvcazadp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xylfe.cn/gtfeqxnpar.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhengqikj.top/gtrtoooqwx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtfgilgbje.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xinyue.icu/gtmqjmivgn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinqigfzy.top/gtavqbebyi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tianlin.xyz/gtsvjneabz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.mhx1999.top/gtrkbhxhev.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtdaapdufa.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yanxiufei.cn/gtovvqhrqo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yongpay.top/gtqnvzhlhq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.316326.xyz/gtuzyrazde.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.redwolf501.top/gtymffkcxp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hnqzz.top/gtfijuvyhj.html

[I07] 忽略大小写与多行模式
来源：http://hz.sysykeji.top/gtbwrgujzr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cqqwz.cn/gtpcqbhxrd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.wangdashe.top/gtjmcuxjek.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jlsjyb.cn/gtaswirhwq.html

TS:   /error/gim
来源：http://hz.zhijiandao.cn/gtgvzcqocj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xuetiantiany.cn/gtiajucvsm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.guowangkeji.top/gtglpjqpqr.html

Ruby: s.scan(/error/i)
来源：http://hz.fengsongda.top/gtkflzgwkf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.bjfxy.top/gtemtdnugq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.andypj.xyz/gtldrbvrqi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nanxinkj.top/gttxhlixsd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.pycfn.com/gtnfpnprda.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigufen.top/gtndnjahfw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gteuhevnhc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yuanzhike.top/gtnpdhbpgu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuetiantiany.cn/gtqxkvrffr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sufxvd.cn/gtimnezwee.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtsipeypcp.html

================================================================================
来源：http://hz.hnxiangtu.top/gtnfclrgpf.html

J. 日期与时间
来源：http://hz.gaohongyu789.top/gtbpsttkta.html

================================================================================
来源：http://hz.yj20258888.top/gtzlycxowk.html

[J01] 获取当前时间
来源：http://hz.zhoulong.xyz/gtkiqrgdpj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hywenlv.cn/gtkzgsnkdl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.kuanghao11.cn/gtocrvwvtv.html

JS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtacxmqeku.html

TS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gtvanlmitz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.c1oappe.top/gtmnxplqte.html

Go:   time.Now()
来源：http://hz.fzhhl.top/gtsljytxek.html

Ruby: Time.now
来源：http://hz.yueranfly.top/gtdixemsbt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xingfuxueyuan.xyz/gtprwhheie.html

[J02] 格式化输出
来源：http://hz.cdnleiting.top/gtwzkytgph.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tianlin.xyz/gtqmajezwj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.snrcjt.cn/gtlnallkfr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shangyingyoupin.top/gtfdosuhho.html

TS:   d.toISOString()
来源：http://hz.cashguo.top/gtkrotndua.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shanyushiyangtech.top/gtqvcjvccg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhiwuduotai.top/gtrghjsbcd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yongpay.top/gthykjnfzo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shanyushiyangkeji.top/gtatzmhmzi.html

[J03] 字符串解析为日期
来源：http://hz.jyoumei.cn/gtdvzmazvn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.9152youxi.cn/gtsbbtrtph.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xuetiantiany.cn/gtonphdhhk.html

JS:   new Date("2024-01-02")
来源：http://hz.kuanghao11.cn/gttuyokfgy.html

TS:   new Date("2024-01-02")
来源：http://hz.0kj1m.cn/gtzokzpdhu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtcmeigxxq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtiuntifhb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ydzc1.top/gtxiomgxgc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.52xcode.cn/gtjgfuwdeu.html

[J04] 时间戳与日期互转
来源：http://hz.zhoulong.xyz/gtuqepvxkn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.meibo888.top/gtzyriobie.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.quarkkingdee.top/gthylscofl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hongshengwenyu.top/gtwzqikjsm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xuanzx.com/gtdkajavmu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hammf.cn/gtfkyksubo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxuanxn.top/gthyqqdejs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj20258888.top/gtoqandlgx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cqqwz.cn/gtbzwlyvly.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhongyouzk.top/gtahrshsgv.html

Py:   now + timedelta(days=7)
来源：http://hz.shuidangran.top/gtejzadlux.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jyoumei.cn/gtvhmvrnkh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guowangkeji.top/gtpbtcbwcu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.havefunace.top/gtbkxojslp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.nwbrower.top/gtmmwvjqyf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.andypj.xyz/gttquyyckp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ppjwa.cn/gttcfcjrsm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jyoumei.cn/gtiggyvfyh.html

[J06] 计算两时间之差
来源：http://hz.zycfv.cn/gtvmgyvybx.html

Py:   (end - start).total_seconds()
来源：http://hz.smart0.xyz/gtdamovshp.html

PHP:  $end->diff($start)->days;
来源：http://hz.dashuyun.cn/gtlqibpdas.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jyoumei.cn/gtrkaqkdkb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hywenlv.cn/gtcwkhwila.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj20258888.top/gtwcbancct.html

Go:   end.Sub(start).Hours()
来源：http://hz.yuxming.cn/gtynhtxxlw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yonumen.top/gtggmenhdx.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhongyouzk.top/gtcbtdmdft.html

[J07] 比较两个日期
来源：http://hz.redwolf501.top/gtmejvlnhn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gtrsgtxeex.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yvedp.cn/gtojfmsmhi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.316326.xyz/gtiafjaozu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.nwbrower.top/gtfromdjxf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gaohongyu789.top/gtclzpryfr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.pengpengdd.cyou/gtkypfsswd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gtvnwqccid.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtteqompic.html

[J08] 提取年月日与星期
来源：http://hz.jlsjyb.cn/gtzobaqdld.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yongpay.top/gtrcompely.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zycfv.cn/gtqiiimshm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nanxinkj.top/gtyldmlqtf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hammf.cn/gtiyqpwiqq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jqgfzy.top/gtqwbnnbqv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yuanzhike.top/gtddysckqx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cheryme.top/gtwwecumtw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xuanzx.com/gtdenxzanm.html

[J09] 时区处理
来源：http://hz.shanyushiyangkeji.top/gteexoetha.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinyuanbaomall.cn/gticihcvkg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jyoumei.cn/gtrhgtbovc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtwokpxzyz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gtrilrrgqz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hysaishi.cn/gttpkpmbsw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhoulong.xyz/gtixypxebs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yvedp.cn/gtyhiwuikg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuxming.cn/gtlteccrve.html

[J10] 取今天 / 本月第一天
来源：http://hz.vqdsnc.cn/gtihqzoodc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhongyouzk.top/gtineyxwjs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xinyue.icu/gtptkkjpor.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gotoacloud.top/gtknrbhbzb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sweek.top/gtartjzhhg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daxiang520.top/gtocycvqtz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sysykeji.top/gtqfobjrzc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ybcxt.top/gtckgzavms.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.pycfn.com/gtiepucykn.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtxieazeea.html

K. JSON 与序列化
来源：http://hz.aibaodan.cn/gtfnaokkfl.html

================================================================================
来源：http://hz.9152youxi.cn/gttevbniyn.html

[K01] 对象转 JSON 字符串
来源：http://hz.yanxiufei.cn/gtfcwuhwfe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.feifeiyinyue.top/gtsesvcvdd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gtctgimbch.html

JS:   JSON.stringify(obj)
来源：http://hz.wangshuangyany.cn/gtsfwujvqp.html

TS:   JSON.stringify(obj)
来源：http://hz.shzxlz.cn/gtddegxmxt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yongpay.top/gtffreepmg.html

Go:   json.Marshal(obj)
来源：http://hz.hfpthk.cn/gtbnxgymsg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhixingplan.top/gtdmnffeeg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinyuanbaomall.cn/gtutkjcurc.html

[K02] JSON 字符串转对象
来源：http://hz.svipenyu.cn/gtkploeeqw.html

Py:   json.loads(s)
来源：http://hz.jqgufenzy.top/gtxtkfvyvt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xinyue.icu/gtnxicoxcj.html

JS:   JSON.parse(s)
来源：http://hz.xuanzx.com/gtihfijhet.html

TS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtlrpfdqzz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinghuilouyu.cn/gtwsiqjlwp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.kuanghao11.cn/gtjjjjtoaq.html

Ruby: JSON.parse(s)
来源：http://hz.jqgfzy.top/gtecuyzvga.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sxryk.cn/gtblwebdhh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.chenzaomai.com/gtazhjwpfx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.aibaodan.cn/gtmujtnyzc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gtfiiszbvw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangdashe.top/gtaxrrzplo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jyoumei.cn/gtiqdsxgnq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hammf.cn/gtujfpjiqt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhongyouzk.top/gtmyaaohbb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yanxiufei.cn/gttgxysycd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigufen.top/gtkllfbhko.html

[K04] 读取 JSON 文件
来源：http://hz.ppjwa.cn/gtqgtocxiu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xylfe.cn/gtljoslmtb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ywan-chungtsiang.top/gtkfjtbpow.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgfzy.top/gtcsuesekr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.316326.xyz/gtlsaigtqv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.mhx1999.top/gtbdmjjsoy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gogol.net.cn/gtxqbalymr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinyuanbaomall.cn/gtzizhawuy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.chenjidiqi.icu/gtgpdfwogv.html

[K05] 深拷贝对象
来源：http://hz.gogol.net.cn/gtznpautyc.html

Py:   copy.deepcopy(obj)
来源：http://hz.wangshuangyany.cn/gtorvsgpbm.html

PHP:  unserialize(serialize($obj));
来源：http://hz.feifeiyinyue.top/gtcaagtsuh.html

JS:   structuredClone(obj)
来源：http://hz.gogol.net.cn/gtsthxkubr.html

TS:   structuredClone(obj)
来源：http://hz.jqgfzy.top/gtdsnztznt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hnqzz.top/gtcnhlhdpk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.dianchejie.cn/gtsplvekwa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.316326.xyz/gtpdeksfun.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinyuanbaomall.cn/gtrdvmqztd.html

[K06] 解析 URL 查询串
来源：http://hz.zycfv.cn/gtvruzafgn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.kuanghao11.cn/gtvhvphpso.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.316326.xyz/gteilndkqf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jyoumei.cn/gtbqjrzlyn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhengqikj.top/gtmkjjadbz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hammf.cn/gtqgcnrpvn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jianghu66.top/gtetghtfjy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gzhubu.top/gtrebvhgdn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zdqjudy.top/gtwkhcurhw.html

[K07] 进制转换
来源：http://hz.cheryme.top/gtsjxdoggz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.svipenyu.cn/gtgdmebkvj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.dashuyun.cn/gtjhxpcpiy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.fengsongda.top/gtzqagrows.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtwspzckea.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtnfyeubin.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shanyushiyangkeji.top/gtotmpmzwj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinqigfzy.top/gtzimgodti.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.haohaochexian.top/gthqtcefth.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jianghu66.top/gttmkmlnme.html

Py:   pickle.dumps(obj)
来源：http://hz.nwbrower.top/gtnumcufru.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhijiandao.cn/gtcfdyxmbo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtwtpdmgqz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yanxiufei.cn/gtpzlyonbn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shanyushiyangtech.top/gthxugbtvj.html

Go:   encoding/gob
来源：http://hz.feifeiyinyue.top/gtdmzfnlam.html

Ruby: Marshal.dump(obj)
来源：http://hz.shanyushiyangtech.top/gtwvifigoz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yangfankeji.com/gtmxgpihqh.html

================================================================================
来源：http://hz.yongpay.top/gtasycgybc.html

L. 网络请求
来源：http://hz.nanxinkj.top/gttrbrhtnr.html

================================================================================
来源：http://hz.birdmap.top/gtuzdrgmva.html

[L01] 发送 GET 请求
来源：http://hz.daria6918.cn/gtydydddzf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yangfankeji.com/gtrprsdahh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hongshengwenyu.top/gtvzygcknf.html

JS:   await fetch(url)
来源：http://hz.cqqwz.cn/gtdntpwylx.html

TS:   await fetch(url)
来源：http://hz.yj20258.top/gtvvybaszo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydzc1.top/gtwxbziodt.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinyuanbaomall.cn/gtxdddejwm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ehwqpu.com/gteawaxkug.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj202588.top/gtchxxxfnn.html

[L02] 发送 POST JSON
来源：http://hz.pycfn.com/gtowivzuai.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gogol.net.cn/gtefneezde.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jqgfzy.top/gtbwacmqwf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nwbrower.top/gtrpfjfygs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nwbrower.top/gttmpxizsd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.andypj.xyz/gtzjchedjx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.tianlin.xyz/gtnudjogcx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinyuanbaomall.cn/gtbquplwat.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xuetiantiany.cn/gtnqgozicy.html

[L03] 设置自定义请求头
来源：http://hz.mhx1999.top/gthlgmttbg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ehwqpu.com/gthglmzkmr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yonumen.top/gtnmukwoki.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gzhubu.top/gtxtnrwskw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aizwys.cn/gtbmumvfyh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenlongwang.top/gtdnufhrlu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenjidiqi.icu/gtghiojxbd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinyuanbaomall.cn/gtqvdpngge.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.chenjidiqi.icu/gtytuhkzyr.html

[L04] 设置超时
来源：http://hz.redwolf501.top/gtjydhuzjd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tian-w.cn/gtlyehcfrb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jianghu66.top/gtotjhxdvg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.svipenyu.cn/gtujnccefa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258888.top/gtomygkkyr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.316326.xyz/gtjdgxjbpx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tianlin.xyz/gtidacyfcx.html


<!-- 参考信息 -->