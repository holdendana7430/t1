代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://hz.vqdsnc.cn/gtvjalcefj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.feifeiyinyue.top/gtrqagmsrr.html

[H09] 带错误码的异常
来源：http://hz.cdnleiting.top/gtkzidbhqn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.aizwys.cn/gtlbgpirgh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.haohaochexian.top/gtacyxsdxh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.quarkkingdee.top/gtbdvkbeka.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhixingplan.top/gtajuthwdd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigfzy.top/gtasqbqajn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cheryme.top/gtnlsarooc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.svipenyu.cn/gtlycmsngs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.c1oappe.top/gtaxfqsmji.html

[H10] 资源自动释放
来源：http://hz.shanyushiyangkeji.top/gtgukmtyrx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guowangkeji.top/gtcoqekyvs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hnxiangtu.top/gtiqvoaczx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.316326.xyz/gtwdohyzsg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuxming.cn/gtzkhdgeqq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.haohaochexian.top/gtgciwriur.html

Go:   defer f.Close()
来源：http://hz.jlsjyb.cn/gtttpokrmo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hongshengwenyu.top/gtgypaluyo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.fengsongda.top/gtwhuohghm.html

================================================================================
来源：http://hz.daria6918.cn/gtnbvfplte.html

I. 正则表达式
来源：http://hz.pycfn.com/gthhtxaeje.html

================================================================================
来源：http://hz.xuanzx.com/gtzmnaregc.html

[I01] 判断是否匹配
来源：http://hz.zycfv.cn/gtynurktjg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yuxming.cn/gtalarmoad.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sufxvd.cn/gtmysyfzrn.html

JS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gtyqjvayaj.html

TS:   /\d+/.test(s)
来源：http://hz.shanyushiyangkeji.top/gtjqrozeai.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cashguo.top/gtaakxdidu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.9152youxi.cn/gtlgqgyrfm.html

Ruby: s.match?(/\d+/)
来源：http://hz.xuanzx.com/gtktvrywaz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yanxiufei.cn/gthbooqyse.html

[I02] 提取所有匹配
来源：http://hz.tianlin.xyz/gtvgyvlttf.html

Py:   re.findall(r"\d+", s)
来源：http://hz.daxiang520.top/gtamjbacaz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhoulong.xyz/gtrmplkbcu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhongyouzk.top/gtbroeeohg.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigufen.top/gtmawloiiv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258.top/gthiuxgwio.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sxryk.cn/gtapcnmmwx.html

Ruby: s.scan(/\d+/)
来源：http://hz.ehwqpu.com/gtrqkfftle.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.guannengcc.top/gtahwmgnfk.html

[I03] 提取捕获分组
来源：http://hz.hysaishi.cn/gteywwjzai.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj202588.top/gtjfuxojrw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.meibo888.top/gtpackwhyl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jianghu66.top/gtuzuigoqr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jqgufenzy.top/gtywbyittc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.aizwys.cn/gtnwxhaodf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.daxiang520.top/gtdieucyto.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.dashuyun.cn/gtbvnleexr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.birdmap.top/gtllqvhkqw.html

[I04] 正则替换
来源：http://hz.ybcxt.top/gtocozlwlp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shzxlz.cn/gtchzixwqi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yueranfly.top/gtnafunqgd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtbjiromxu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.52xcode.cn/gtvwiulqjm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hammf.cn/gtgatbkzak.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhongyouzk.top/gttirmjgzq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yuanzhike.top/gtbqbiyqlt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.meibo888.top/gtnqylsjqn.html

[I05] 按正则拆分
来源：http://hz.aibaodan.cn/gtxrsrowlq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.pengpengdd.cyou/gtjhjxrgqq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.pycfn.com/gtlrhhlwjn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtkgetsdse.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gtewbhbgdw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zycfv.cn/gtknmetdbq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.meibo888.top/gtbusklepq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gtgdiltnvg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.bjfxy.top/gtnlhcwsjp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.wangshuangyany.cn/gtacgwctvt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xylfe.cn/gtakxsymgs.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.chenzaomai.com/gtlauofbys.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxinkj.top/gtvvpbucka.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xuanzx.com/gtghrutcgz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sxryk.cn/gtjkytnsau.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.daria6918.cn/gtimigoept.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.316326.xyz/gthlrjsvkg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.haohaochexian.top/gtnyahekca.html

[I07] 忽略大小写与多行模式
来源：http://hz.haohaochexian.top/gtmawjfphf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nwbrower.top/gtcusbjtum.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.redwolf501.top/gtfzugrfkj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xuanzx.com/gtuikztipx.html

TS:   /error/gim
来源：http://hz.jiagoushi.top/gtnkopvdyy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sufxvd.cn/gtmystyzym.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydzc1.top/gtehkxhvoc.html

Ruby: s.scan(/error/i)
来源：http://hz.shanyushiyangtech.top/gtykicjlai.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yonumen.top/gtipcdbxid.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhaomingkeji.xyz/gtydqzwvnr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj202588.top/gtdgzjmcku.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cqqwz.cn/gtyhasttjs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxuanxn.top/gtaltagevc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daria6918.cn/gtfpjhlmwd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nwbrower.top/gtrnndawti.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sufxvd.cn/gtkbwbuqxv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.c1oappe.top/gtzdaftgyg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gaohongyu789.top/gtzcijmftv.html

================================================================================
来源：http://hz.shuidangran.top/gtmebfrgcr.html

J. 日期与时间
来源：http://hz.aibaodan.cn/gthpsahxdf.html

================================================================================
来源：http://hz.jlsjyb.cn/gtycccxqrv.html

[J01] 获取当前时间
来源：http://hz.zhengqikj.top/gtqczldprc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj20258888.top/gtodoohqbf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtbomtbnhc.html

JS:   new Date();  Date.now()
来源：http://hz.nwbrower.top/gtnawfdwey.html

TS:   new Date();  Date.now()
来源：http://hz.shanyushiyangtech.top/gtqicxtsmi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.daria6918.cn/gtumuaiohe.html

Go:   time.Now()
来源：http://hz.c1oappe.top/gthharblzp.html

Ruby: Time.now
来源：http://hz.fzhhl.top/gtxvuqpoyd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hnqzz.top/gtvmmslyux.html

[J02] 格式化输出
来源：http://hz.cheryme.top/gtzillclnu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.quarkkingdee.top/gtvzrinccj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinqigufen.top/gtrnbbvxij.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.pengpengdd.cyou/gtvvabtpie.html

TS:   d.toISOString()
来源：http://hz.gotoacloud.top/gtyqwfdbvb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.wangdashe.top/gthriovdjy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.wangshuangyany.cn/gtpbeziptv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hfpthk.cn/gthdqeoqga.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.52xcode.cn/gtycrwdqft.html

[J03] 字符串解析为日期
来源：http://hz.jiagoushi.top/gtqsadcmbx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhaomingkeji.xyz/gtpeuldsfy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.wangdashe.top/gtzczbezkc.html

JS:   new Date("2024-01-02")
来源：http://hz.gaohongyu789.top/gtlfgadlce.html

TS:   new Date("2024-01-02")
来源：http://hz.zhengqikj.top/gtjsnzuvcj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gthvyavbow.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.pengpengdd.cyou/gtvvmalsvx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cucudq.cn/gtlebstqqu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhijiandao.cn/gtyablnzhx.html

[J04] 时间戳与日期互转
来源：http://hz.wangdashe.top/gtbwmgilkb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hywenlv.cn/gtkglkzpbd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yvedp.cn/gtulsyfjqq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nanxuanxn.top/gtiziatpyb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hnqzz.top/gthfycfdxi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yanxiufei.cn/gtnsaeedbv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jianghu66.top/gtymphlajv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj20258888.top/gtebeydvli.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yuxming.cn/gtilpdyjgb.html

[J05] 时间加减（加 7 天）
来源：http://hz.feifeiyinyue.top/gtlrpeltaj.html

Py:   now + timedelta(days=7)
来源：http://hz.cucudq.cn/gtclaidklx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.pycfn.com/gtobrzjrxr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj202588.top/gtyzstofjz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhaomingkeji.xyz/gtsqfrdigo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shangyingyoupin.top/gtszxaxfje.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yj202588.top/gtcshqcvyq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xingfuxueyuan.xyz/gtjucuslzd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.kuanghao11.cn/gtcfpnpzqx.html

[J06] 计算两时间之差
来源：http://hz.sufxvd.cn/gtkfkplykp.html

Py:   (end - start).total_seconds()
来源：http://hz.feifeiyinyue.top/gtsusdssxf.html

PHP:  $end->diff($start)->days;
来源：http://hz.jianghu66.top/gtjhntiyzd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xziqi.cn/gtnzdettfl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.haohaochexian.top/gtlagikqwn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.svipenyu.cn/gttndjuvjf.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinqigfzy.top/gtdzsvbyjm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hysaishi.cn/gtzektimab.html

C#:   (end - start).TotalSeconds
来源：http://hz.tian-w.cn/gtdamndcex.html

[J07] 比较两个日期
来源：http://hz.smart0.xyz/gtejcwyslh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtycdongms.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shzxlz.cn/gtggkdprss.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhaomingkeji.xyz/gttuzejxzn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.wangshuangyany.cn/gtdurotmnz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hnqzz.top/gtwttebilk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinqigufen.top/gtdnqouilo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtnzpgjrso.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtqqhetwmj.html

[J08] 提取年月日与星期
来源：http://hz.jyoumei.cn/gtiveikqny.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shanyushiyangtech.top/gteuwalgbd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.chenzaomai.com/gtrfhxbylp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sufxvd.cn/gtfpozxtwc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yuxming.cn/gtzewfnuyt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gogol.net.cn/gtziztwdia.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jianghu66.top/gteasidzvl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.dashuyun.cn/gtmadvugoz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guannengcc.top/gtsoqzwjzr.html

[J09] 时区处理
来源：http://hz.yonumen.top/gtvptsavra.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nanxuanxn.top/gtyamqhtez.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jlsjyb.cn/gtxotqbpla.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtpociwcnt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtkyxjwzlz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yanxiufei.cn/gtrdepibuu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zdqjudy.top/gtugoiuirc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sufxvd.cn/gtdwrlewam.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.chenzaomai.com/gtlwzvsqpi.html

[J10] 取今天 / 本月第一天
来源：http://hz.wangshuangyany.cn/gtpkfbmtka.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shanyushiyangtech.top/gtscmjiazz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gogol.net.cn/gthuzzrpwn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj202588.top/gtnuhzkhts.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.havefunace.top/gttdfraesr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yueranfly.top/gtpiilxxii.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.svipenyu.cn/gtmlyoziky.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.fzhhl.top/gtdvcuopkw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ydjk.org.cn/gtmyumnram.html

================================================================================
来源：http://hz.chenlongwang.top/gtafdvwnad.html

K. JSON 与序列化
来源：http://hz.aizwys.cn/gtdedlzhpc.html

================================================================================
来源：http://hz.zhijiandao.cn/gtqcosrzix.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenlongwang.top/gtmvcvgsqr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhixingplan.top/gtxfyiutdd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgufenzy.top/gtpeoeznzl.html

JS:   JSON.stringify(obj)
来源：http://hz.ivvv.top/gtdovzauyc.html

TS:   JSON.stringify(obj)
来源：http://hz.shzxlz.cn/gtczwsdsjz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.wangshuangyany.cn/gtrjqazwck.html

Go:   json.Marshal(obj)
来源：http://hz.jqgufenzy.top/gtkymyntwn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.daria6918.cn/gtvogxulae.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nwbrower.top/gtwcqxcqdw.html

[K02] JSON 字符串转对象
来源：http://hz.chenjidiqi.icu/gtkintfcyr.html

Py:   json.loads(s)
来源：http://hz.shangyingyoupin.top/gtpjcjplup.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhongyouzk.top/gtbkrtqxzl.html

JS:   JSON.parse(s)
来源：http://hz.ppjwa.cn/gtunwlcxet.html

TS:   JSON.parse(s)
来源：http://hz.yongpay.top/gtrwcthejj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zycfv.cn/gtfufqhmnu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gogol.net.cn/gtbmskjhga.html

Ruby: JSON.parse(s)
来源：http://hz.sxryk.cn/gtcqndyfal.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zdqjudy.top/gtipsxwjun.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sweek.top/gtsbcsliog.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cashguo.top/gtbtqyfekz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cqqwz.cn/gtwewcrgos.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ppjwa.cn/gtmfvrrvnz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gtuiarkvpp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.fzhhl.top/gtwnastjbz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.andypj.xyz/gthxjyrgiu.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gaohongyu789.top/gtstkudfxr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yonumen.top/gtkdetggib.html

[K04] 读取 JSON 文件
来源：http://hz.yueranfly.top/gtfehnkprz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.guowangkeji.top/gtbnjkrzwu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.fzhhl.top/gtydrojeap.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtvygtoayu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ivvv.top/gtawzycuzb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhixingplan.top/gtflyqeamf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xingfuxueyuan.xyz/gtuhocrowa.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yonumen.top/gtmuedpsbi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhongyouzk.top/gtrypzfbqj.html

[K05] 深拷贝对象
来源：http://hz.ydjk.org.cn/gtrwgsxhvv.html

Py:   copy.deepcopy(obj)
来源：http://hz.zycfv.cn/gtfvykghfv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.nwbrower.top/gtaccutqqb.html

JS:   structuredClone(obj)
来源：http://hz.dashuyun.cn/gthkhcmjbb.html

TS:   structuredClone(obj)
来源：http://hz.yvedp.cn/gtvvevwvsc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cheryme.top/gtlgbmzefn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nanxinkj.top/gtahpltlso.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhaomingkeji.xyz/gtvueseqrm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.haohaochexian.top/gtyfmeqhtm.html

[K06] 解析 URL 查询串
来源：http://hz.quarkkingdee.top/gtegjyeleg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hysaishi.cn/gtafnfclsw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.daria6918.cn/gtqjkzadfp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jyoumei.cn/gtcnsrjmbm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydzc1.top/gtlprhrpob.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nwbrower.top/gtuwkxxkzl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.bjfxy.top/gtsfghccso.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtflxwwvkr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.svipenyu.cn/gtnegngvlj.html

[K07] 进制转换
来源：http://hz.cashguo.top/gtajerslwd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj202588.top/gtsqhjxdwb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xinyue.icu/gtkkjqmdqy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtsjghkpsm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ivvv.top/gthualajve.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tanke756.top/gtwryrhsis.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.kuanghao11.cn/gtevyqdlhn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.andypj.xyz/gtopyjiffe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cqqwz.cn/gtxzpputpi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj202588.top/gtzcrfhshr.html

Py:   pickle.dumps(obj)
来源：http://hz.jinqigufen.top/gtjpeumdwh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.nanxuanxn.top/gtiittyrwj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.meibo888.top/gtzwcqcqpz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.aibaodan.cn/gtdbyydpyr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.guannengcc.top/gtffiojqhb.html

Go:   encoding/gob
来源：http://hz.jlsjyb.cn/gthiyuzbgx.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinqigfzy.top/gtkwqymeqk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.wangdashe.top/gtuxefgadq.html

================================================================================
来源：http://hz.snrcjt.cn/gtvkhbjnik.html

L. 网络请求
来源：http://hz.ppjwa.cn/gtnfmwfxae.html

================================================================================
来源：http://hz.cdnleiting.top/gtyclqulnb.html

[L01] 发送 GET 请求
来源：http://hz.xuetiantiany.cn/gtbyndrixq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.wangshuangyany.cn/gtwssgajnx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.tanke756.top/gtffadhjkq.html

JS:   await fetch(url)
来源：http://hz.zhoulong.xyz/gtzhcxmotl.html

TS:   await fetch(url)
来源：http://hz.xinyue.icu/gtbbjpitzu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.316326.xyz/gtcbqboksy.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhengqikj.top/gteykvgeno.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.aizwys.cn/gtyanjpggc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.0kj1m.cn/gtfuiqhdch.html

[L02] 发送 POST JSON
来源：http://hz.jyoumei.cn/gtextguimy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgufenzy.top/gthhpqtnxq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhaomingkeji.xyz/gtvdgtrlhl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhongyouzk.top/gtldugkhif.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gtrokgxgzk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gotoacloud.top/gtzoelnjns.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhengqikj.top/gtbsguwfey.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cqqwz.cn/gtsplecltt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gogol.net.cn/gtoglhnrnz.html

[L03] 设置自定义请求头
来源：http://hz.jyoumei.cn/gtekgwtbut.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ehwqpu.com/gtypwgktqb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yongpay.top/gtohikwoar.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.9152youxi.cn/gtksdkyqny.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinghuilouyu.cn/gtlgqsthgk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shanyushiyangtech.top/gtvnkomssn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zdqjudy.top/gtbvtciwjw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yueranfly.top/gtiyarllso.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.quarkkingdee.top/gttdbntxvu.html

[L04] 设置超时
来源：http://hz.gotoacloud.top/gtnhwlnzmg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zdqjudy.top/gtonoeckwl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.haohaochexian.top/gttxqobdfl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gtbbcxklgg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtapmuemqt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.shuidangran.top/gtbbrwizdn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zdqjudy.top/gthuxtakye.html


<!-- 参考信息 -->