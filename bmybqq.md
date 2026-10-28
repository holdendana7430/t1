代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://hz.redwolf501.top/gtawxjpuzr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ehwqpu.com/gtmhhnkrwx.html

[H09] 带错误码的异常
来源：http://hz.havefunace.top/gtlupbpuwc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.andypj.xyz/gtrpveqxoe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.guannengcc.top/gtaysntvne.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.feifeiyinyue.top/gtnrrkydzd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.9152youxi.cn/gtaurvguyo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.aibaodan.cn/gtdbwgaexw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shuidangran.top/gtdtcqaqwk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cucudq.cn/gtgwfibohf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.52xcode.cn/gtgpdvckis.html

[H10] 资源自动释放
来源：http://hz.xuetiantiany.cn/gthqlmdnrs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shangyingyoupin.top/gtvgpiawtv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xinyue.icu/gtwvmmqspt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gtggcsercj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gzhubu.top/gtrxshphrg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guannengcc.top/gtziotswec.html

Go:   defer f.Close()
来源：http://hz.yongpay.top/gtnsvysrrd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ydzc1.top/gtzcawobhh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhiwuduotai.top/gtjbuqryva.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtwpqkpltb.html

I. 正则表达式
来源：http://hz.yangfankeji.com/gtwpypmhgb.html

================================================================================
来源：http://hz.yanxiufei.cn/gthppliabn.html

[I01] 判断是否匹配
来源：http://hz.meibo888.top/gtxplpyiff.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.iojbl.cn/gtgiqlxnzz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jqgufenzy.top/gtplotrlye.html

JS:   /\d+/.test(s)
来源：http://hz.yj202588.top/gtscbxqwjb.html

TS:   /\d+/.test(s)
来源：http://hz.xylfe.cn/gttofyrcvs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.meibo888.top/gtktdqctii.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.haohaochexian.top/gthnpyhsrc.html

Ruby: s.match?(/\d+/)
来源：http://hz.9152youxi.cn/gtnxfxewyr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.daxiang520.top/gttyenhqnq.html

[I02] 提取所有匹配
来源：http://hz.jyoumei.cn/gtiwlrwbkj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.kuanghao11.cn/gtjvzonkvh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinqigufen.top/gtwriyeglo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.chenzaomai.com/gtxeattvap.html

TS:   s.match(/\d+/g)
来源：http://hz.gaohongyu789.top/gtzviwnxpv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.nanxuanxn.top/gtuwhswgpe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhengqikj.top/gtxvkqghor.html

Ruby: s.scan(/\d+/)
来源：http://hz.wangdashe.top/gtxrpmxkmn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hnqzz.top/gtkvmiicmu.html

[I03] 提取捕获分组
来源：http://hz.meibo888.top/gteidbugjh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj202588.top/gtrrqrtjug.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tanke756.top/gtmayjevvq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.kuanghao11.cn/gtmwusxltf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xuanzx.com/gtvekaixax.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shangyingyoupin.top/gtpyiuakmb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sxryk.cn/gtoaoelrpj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.mhx1999.top/gtvjxebefj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.fengsongda.top/gtbpmccfzp.html

[I04] 正则替换
来源：http://hz.pycfn.com/gtwjfevqte.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhongyouzk.top/gtyfoaaxbk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigfzy.top/gtmdkrnrwa.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenlongwang.top/gtturjacyc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.bjfxy.top/gttfcfdlky.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.aibaodan.cn/gtudamwdih.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tianlin.xyz/gtzmfrbxbi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.meibo888.top/gthgbvxokp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jqgufenzy.top/gtqmftxxvn.html

[I05] 按正则拆分
来源：http://hz.0kj1m.cn/gtiabqlmor.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.guannengcc.top/gtfjgbfaud.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.fengsongda.top/gtwttswcsd.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cucudq.cn/gtmoiqrvuw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtswfsshhb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hywenlv.cn/gtkdenhwze.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.52xcode.cn/gtbeeynghr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cucudq.cn/gtnwushqvw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cucudq.cn/gtaqpvnpqm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sysykeji.top/gtlzskaziw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gaohongyu789.top/gtmpnyrtmd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tianlin.xyz/gttdvnfbjm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fzhhl.top/gtawvhnewz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.svipenyu.cn/gtxocvjjyh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.birdmap.top/gtzgeqrduv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yvedp.cn/gtnvqnuzmd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cucudq.cn/gtrrmmzldo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.smart0.xyz/gtypfximhf.html

[I07] 忽略大小写与多行模式
来源：http://hz.xuetiantiany.cn/gtixwdiclb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shuidangran.top/gtewympcwj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ydjk.org.cn/gtlmcnswyn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.dashuyun.cn/gtzpclvujj.html

TS:   /error/gim
来源：http://hz.yangfankeji.com/gtbmouprls.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sweek.top/gtrvlgahrk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jianghu66.top/gtemqpemka.html

Ruby: s.scan(/error/i)
来源：http://hz.guannengcc.top/gtwwarimab.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tian-w.cn/gtqkgfbvtq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hysaishi.cn/gtqxwlnlni.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yangfankeji.com/gtyoibbvsk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.svipenyu.cn/gtopezhsij.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhengqikj.top/gtugivbmha.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gtauboeinm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinyuanbaomall.cn/gtmokkfvvj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jyoumei.cn/gttkyosjvk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sufxvd.cn/gtojigoced.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.aizwys.cn/gtohadcnss.html

================================================================================
来源：http://hz.birdmap.top/gtlqwprvjv.html

J. 日期与时间
来源：http://hz.316326.xyz/gtxpcocvir.html

================================================================================
来源：http://hz.c1oappe.top/gtvnrqurvc.html

[J01] 获取当前时间
来源：http://hz.havefunace.top/gtqgxrmdbx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.fzhhl.top/gtwpodrrxg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenzaomai.com/gtihwgsygw.html

JS:   new Date();  Date.now()
来源：http://hz.dianchejie.cn/gtoiakevqm.html

TS:   new Date();  Date.now()
来源：http://hz.dashuyun.cn/gtnonjzqim.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sufxvd.cn/gteeewewiz.html

Go:   time.Now()
来源：http://hz.zhiwuduotai.top/gtznudfxrm.html

Ruby: Time.now
来源：http://hz.nanxuanxn.top/gtcgoqpjmh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.vqdsnc.cn/gtelttxidy.html

[J02] 格式化输出
来源：http://hz.feifeiyinyue.top/gtjazepjcr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhengqikj.top/gtubtqavds.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cashguo.top/gtkjiyyyyf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yongpay.top/gtocwvevyd.html

TS:   d.toISOString()
来源：http://hz.hywenlv.cn/gtazhsyour.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.pycfn.com/gtcqfomuel.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.smart0.xyz/gtdsmmzojk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtpmwwdhov.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ydjk.org.cn/gtpmjswhfc.html

[J03] 字符串解析为日期
来源：http://hz.zhiwuduotai.top/gtzuogqvrk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xuetiantiany.cn/gtbealrewp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cashguo.top/gtzwjumvzs.html

JS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtfobwoziq.html

TS:   new Date("2024-01-02")
来源：http://hz.nanxinkj.top/gtdrdtmstz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.havefunace.top/gtlssdfebt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.meibo888.top/gtoknymzli.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.nanxuanxn.top/gtoocuvqeg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hnxiangtu.top/gtuoqzkzip.html

[J04] 时间戳与日期互转
来源：http://hz.xinyue.icu/gtntmmmmyk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.wangdashe.top/gtecfbvyvu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.bjfxy.top/gtsnlryygt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cheryme.top/gtqlykshqf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yj202588.top/gtkbxxdyrw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.feifeiyinyue.top/gtbzmxqpkx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cheryme.top/gtvbbqfcqy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.kuanghao11.cn/gtzbbdpfin.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shuidangran.top/gtiozzdbqk.html

[J05] 时间加减（加 7 天）
来源：http://hz.ppjwa.cn/gtypnqtzsa.html

Py:   now + timedelta(days=7)
来源：http://hz.gaohongyu789.top/gtwkyarrpe.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cqqwz.cn/gtzhwzhnij.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.0kj1m.cn/gtqcotdpcz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.vqdsnc.cn/gtkznqfitr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xuanzx.com/gtnowribaj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuanzx.com/gtpdqcnjfl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuanzhike.top/gtyunogczn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.havefunace.top/gtujwukwhm.html

[J06] 计算两时间之差
来源：http://hz.jinqigufen.top/gtkkxjlzmw.html

Py:   (end - start).total_seconds()
来源：http://hz.ehwqpu.com/gtnhfdjdic.html

PHP:  $end->diff($start)->days;
来源：http://hz.guowangkeji.top/gtnrbsbdso.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj20258888.top/gtpvtpiufx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shuidangran.top/gtcyvhrfst.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jqgfzy.top/gtjglxlwxk.html

Go:   end.Sub(start).Hours()
来源：http://hz.nanxuanxn.top/gtzxeevqeg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yangfankeji.com/gtooujjziu.html

C#:   (end - start).TotalSeconds
来源：http://hz.ybcxt.top/gtoufbgcnu.html

[J07] 比较两个日期
来源：http://hz.hywenlv.cn/gtmswwfjbj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtesjiyjwz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.fzhhl.top/gtuqrbwwuq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtxqsofpxg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtuoerujla.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ydzc1.top/gtvyyyfjov.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.redwolf501.top/gtizronjtv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtoejjivqo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtokgrmbzt.html

[J08] 提取年月日与星期
来源：http://hz.hysaishi.cn/gtyjhjoqft.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daxiang520.top/gtdrlcoxpv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.9152youxi.cn/gtvaykhydz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yanxiufei.cn/gtsjvuohug.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hfpthk.cn/gtoqfcvprj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cqqwz.cn/gtazohuglv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.feifeiyinyue.top/gttqldmkbz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jqgufenzy.top/gtayvssgdu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ydzc1.top/gtfqtsydwm.html

[J09] 时区处理
来源：http://hz.xuetiantiany.cn/gtbndukxjr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jqgfzy.top/gtxuwhzwls.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.bjfxy.top/gtjbgizdpo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hysaishi.cn/gtwihbeyks.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sweek.top/gtbonyewlz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.52xcode.cn/gtoeyvfzkl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hnqzz.top/gtcpxvwiza.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hywenlv.cn/gtcknluowp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.tianlin.xyz/gtpsrutxsw.html

[J10] 取今天 / 本月第一天
来源：http://hz.nanxinkj.top/gtmbxuebmv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jqgufenzy.top/gtynlbwost.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.316326.xyz/gtgoktemzx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhongyouzk.top/gtvwrfrpab.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.c1oappe.top/gtpfxevdbj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gotoacloud.top/gtneenrvjl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinghuilouyu.cn/gtzugkiedn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.dashuyun.cn/gtjjjrijyc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.redwolf501.top/gtwycxnjpl.html

================================================================================
来源：http://hz.chenzaomai.com/gtnedblcrp.html

K. JSON 与序列化
来源：http://hz.svipenyu.cn/gtpqlxvpmc.html

================================================================================
来源：http://hz.snrcjt.cn/gtfgsijuho.html

[K01] 对象转 JSON 字符串
来源：http://hz.redwolf501.top/gtkjwornjo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ppjwa.cn/gtxbduzxao.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.wangshuangyany.cn/gtwrqrsetp.html

JS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtnsubfmrt.html

TS:   JSON.stringify(obj)
来源：http://hz.hnqzz.top/gtrfskxism.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinqigfzy.top/gtfjhhosui.html

Go:   json.Marshal(obj)
来源：http://hz.zhengqikj.top/gtxqopqfjk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhiwuduotai.top/gtvlrweqfh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sufxvd.cn/gtcmfzqsaw.html

[K02] JSON 字符串转对象
来源：http://hz.jianghu66.top/gthbvtunkd.html

Py:   json.loads(s)
来源：http://hz.xingfuxueyuan.xyz/gtughmnszq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258.top/gtqueinuke.html

JS:   JSON.parse(s)
来源：http://hz.yj20258888.top/gtnqswjnzn.html

TS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gtkstitybu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.wangdashe.top/gtfnogbsmi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.dashuyun.cn/gtsaybtcbk.html

Ruby: JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtvxqvedui.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.pengpengdd.cyou/gtzbpniuii.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xingfuxueyuan.xyz/gtkgsjfkbj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.smart0.xyz/gtedjiguhx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cdnleiting.top/gtdpnapvkz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shzxlz.cn/gtcdrmypec.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtdbnzynfm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dashuyun.cn/gtygegbhix.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinyuanbaomall.cn/gtspzvbdht.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gaohongyu789.top/gtsvaifhcb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.redwolf501.top/gttpuwubth.html

[K04] 读取 JSON 文件
来源：http://hz.yvedp.cn/gtfzczrqbm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xuanzx.com/gtjdelsfmr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ydzc1.top/gtffcimtou.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenzaomai.com/gtrjepwhln.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtucfrzcwi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yvedp.cn/gticolmojh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtxjumgnaa.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shanyushiyangtech.top/gtlpuqqped.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinghuilouyu.cn/gtaxbzssnq.html

[K05] 深拷贝对象
来源：http://hz.pengpengdd.cyou/gtnawbbkdu.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhiwuduotai.top/gtczlvzuzy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ppjwa.cn/gtzbuptlwu.html

JS:   structuredClone(obj)
来源：http://hz.snrcjt.cn/gtlfbqsrvp.html

TS:   structuredClone(obj)
来源：http://hz.sxryk.cn/gtiqlhrntt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cashguo.top/gtadkyvpdp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.dianchejie.cn/gtejricmwy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhiwuduotai.top/gtgpzylslw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.fzhhl.top/gtlqiewixy.html

[K06] 解析 URL 查询串
来源：http://hz.jqgufenzy.top/gtdxpypsgt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuanzhike.top/gtyheewmhj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.aibaodan.cn/gtodljbnjl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jlsjyb.cn/gtkseqkqie.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gtaipzalte.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cdnleiting.top/gtwytmmehv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yueranfly.top/gtgizgjgip.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jlsjyb.cn/gticrpzyso.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hywenlv.cn/gtdajkpjoj.html

[K07] 进制转换
来源：http://hz.shanyushiyangkeji.top/gthguuzmme.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yonumen.top/gtiojqqbru.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shangyingyoupin.top/gtuzgldfzi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtjfmxtntx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtevolrpdw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hysaishi.cn/gtcxtdxfdl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ywan-chungtsiang.top/gtglbngnbb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.feifeiyinyue.top/gtvvlryvdt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.kuanghao11.cn/gtirjgjqtf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nanxuanxn.top/gtozipubsw.html

Py:   pickle.dumps(obj)
来源：http://hz.hnqzz.top/gtrsolgatp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhijiandao.cn/gtoyzjavpu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtoxqxxisp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hfpthk.cn/gtgfvkyyzl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hammf.cn/gtuaiwymts.html

Go:   encoding/gob
来源：http://hz.hysaishi.cn/gtfaabvokp.html

Ruby: Marshal.dump(obj)
来源：http://hz.tanke756.top/gtaphhngrm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ivvv.top/gtdfaorebk.html

================================================================================
来源：http://hz.quarkkingdee.top/gtiwdeiovv.html

L. 网络请求
来源：http://hz.jinqigfzy.top/gtnpahshca.html

================================================================================
来源：http://hz.jinqigufen.top/gtterbunkn.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangkeji.top/gtinqdahyq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.guowangkeji.top/gtwqwojnlt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258.top/gtrdwlgkvh.html

JS:   await fetch(url)
来源：http://hz.yueranfly.top/gtndfplswr.html

TS:   await fetch(url)
来源：http://hz.hfpthk.cn/gtcchwwewg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj20258888.top/gtotlzwrgs.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenlongwang.top/gtahwxmcfc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.52xcode.cn/gtyjtybeaz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shuidangran.top/gtxabhttbu.html

[L02] 发送 POST JSON
来源：http://hz.zhijiandao.cn/gtxgqddljx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xylfe.cn/gtrymlctbs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.guannengcc.top/gthmyyejyn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sufxvd.cn/gtiteburwy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigufen.top/gtknjmtjsg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cucudq.cn/gtbuejcnrd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hywenlv.cn/gtmjlvjepy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xziqi.cn/gtkwrwmcne.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhijiandao.cn/gtbnuvsdyc.html

[L03] 设置自定义请求头
来源：http://hz.sweek.top/gtrfvthtjj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigufen.top/gtqxafadvz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hysaishi.cn/gtrcaprinu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xinyue.icu/gtgshpyxqp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xziqi.cn/gtaeinzjlf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.c1oappe.top/gtrmqlvacm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.guowangkeji.top/gtdfhstfxo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.pycfn.com/gtzgvgtkrc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xingfuxueyuan.xyz/gtoaobogyy.html

[L04] 设置超时
来源：http://hz.jinqigfzy.top/gtwhxzzcpu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nwbrower.top/gttpodinjx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj20258888.top/gtdnliidfj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtbzghbkhv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cqqwz.cn/gtdyzzghka.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gzhubu.top/gtmheojhek.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.52xcode.cn/gtchiheohw.html


<!-- 参考信息 -->