代发 wailian999

JS:   e.message;  e.stack
来源：http://hz.yanxiufei.cn/gtzjmtawsn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yonumen.top/gtjmjjzjhj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhixingplan.top/gtyssbnzmo.html

Go:   err.Error()
来源：http://hz.yuxming.cn/gtytqdlplu.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnqzz.top/gtdedbcnag.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shuidangran.top/gtifmchtln.html

[H09] 带错误码的异常
来源：http://hz.ydzc1.top/gtvzrpcdyp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.haohaochexian.top/gtsqvugllg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.iojbl.cn/gtjmejczxg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinqigufen.top/gtpdhxrwyv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.9152youxi.cn/gtzocqwkvb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cqqwz.cn/gtnaphragf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sweek.top/gtqzrepwnt.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jianghu66.top/gtfgqgjdxi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.52xcode.cn/gtxcxftzpr.html

[H10] 资源自动释放
来源：http://hz.wangshuangyany.cn/gtoizlrfje.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinqigfzy.top/gtfxxyrmmu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.316326.xyz/gtndsylhwo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cucudq.cn/gtsvjvaehy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jiagoushi.top/gtjxyijkaf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sweek.top/gtuuycrzvk.html

Go:   defer f.Close()
来源：http://hz.cdnleiting.top/gtrejrwspp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.c1oappe.top/gtjvjppxtg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tianlin.xyz/gtxmiwaurx.html

================================================================================
来源：http://hz.cdnleiting.top/gtdillovjz.html

I. 正则表达式
来源：http://hz.yj20258888.top/gtetqrcbxn.html

================================================================================
来源：http://hz.hnxiangtu.top/gtnackpegq.html

[I01] 判断是否匹配
来源：http://hz.ywan-chungtsiang.top/gtbqtsgory.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.9152youxi.cn/gtvlxdxgkd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.iojbl.cn/gtuppmkxsp.html

JS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gtdigigdst.html

TS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gtkrxwtjne.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xylfe.cn/gtpcpalodx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.aibaodan.cn/gtwlprqpvt.html

Ruby: s.match?(/\d+/)
来源：http://hz.yangfankeji.com/gtawhroklp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xinyue.icu/gtfulflxwo.html

[I02] 提取所有匹配
来源：http://hz.sysykeji.top/gtznwmvcpq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cdnleiting.top/gtngzbyzpy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hysaishi.cn/gtvwchnkuf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xylfe.cn/gtarjpokpc.html

TS:   s.match(/\d+/g)
来源：http://hz.wangdashe.top/gtjowzdgyc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sxryk.cn/gtaoahwkbj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.9152youxi.cn/gtvhuczbyl.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhiwuduotai.top/gtbyjccmsn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.kuanghao11.cn/gtgwaxvere.html

[I03] 提取捕获分组
来源：http://hz.daria6918.cn/gtipshlkys.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.tianlin.xyz/gtalsfvcqh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cucudq.cn/gtmbbgxral.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.c1oappe.top/gtkfagfmhb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tanke756.top/gthsadweok.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.andypj.xyz/gtfadtfxmr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.c1oappe.top/gtxvzuotrf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yonumen.top/gtttfcpaif.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yanxiufei.cn/gtnetpjwhf.html

[I04] 正则替换
来源：http://hz.tian-w.cn/gtaqjzxznt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gogol.net.cn/gtmxqwqmri.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gtnmkgkgzi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.quarkkingdee.top/gtkkpmxotf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtyxzpypwu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nwbrower.top/gtpopjuwux.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cheryme.top/gtawoxfdwg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sxryk.cn/gtebnnixud.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hongshengwenyu.top/gtagmoadwm.html

[I05] 按正则拆分
来源：http://hz.chenzaomai.com/gtfkadhepr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gaohongyu789.top/gtyzdmdsyg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jqgufenzy.top/gtzoailvhc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtiawevqsm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtfhujalpr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.tianlin.xyz/gtozhcrvjo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shzxlz.cn/gtvfspbfdz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtaczmhcxv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhengqikj.top/gtuzdqgmrn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hysaishi.cn/gthwpnrgdh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jlsjyb.cn/gtawctoeda.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.guowangkeji.top/gtokphykps.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aizwys.cn/gtqkvnqiuv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gtywwpsqjn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhijiandao.cn/gtqmtxasdl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangshuangyany.cn/gtnlbuacrc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhengqikj.top/gtamhcbikw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cheryme.top/gtccdrzzch.html

[I07] 忽略大小写与多行模式
来源：http://hz.cheryme.top/gtuzeisfpv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tian-w.cn/gtqvnylilo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jyoumei.cn/gtpzuafogg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hammf.cn/gtoewioryj.html

TS:   /error/gim
来源：http://hz.tianlin.xyz/gtytblgvlu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gotoacloud.top/gtixzbsagr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ybcxt.top/gtaaumhjju.html

Ruby: s.scan(/error/i)
来源：http://hz.shanyushiyangtech.top/gtlaawyytn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yongpay.top/gtrqpdqgtm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yongpay.top/gtjysgaqsg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.52xcode.cn/gtukumbkbz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yonumen.top/gtljsnqaul.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.snrcjt.cn/gtibmzrulf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuetiantiany.cn/gtqhbzkxjo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cdnleiting.top/gtsizmcxca.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.c1oappe.top/gtsbflnnhq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.dashuyun.cn/gtlcjwkihc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.mhx1999.top/gtjmpzroka.html

================================================================================
来源：http://hz.c1oappe.top/gtfsdeuvbl.html

J. 日期与时间
来源：http://hz.ivvv.top/gthcmtssdj.html

================================================================================
来源：http://hz.yuxming.cn/gtyqyynndr.html

[J01] 获取当前时间
来源：http://hz.pengpengdd.cyou/gtardiqwhg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gaohongyu789.top/gthcsfukft.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gtwgdqokbc.html

JS:   new Date();  Date.now()
来源：http://hz.nanxinkj.top/gtwcrijpjl.html

TS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gtkjbzsdht.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinqigufen.top/gtlqzarrci.html

Go:   time.Now()
来源：http://hz.hysaishi.cn/gtqdrjxbfc.html

Ruby: Time.now
来源：http://hz.xylfe.cn/gtjefdnhuu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tian-w.cn/gtyeaxdqgm.html

[J02] 格式化输出
来源：http://hz.bjfxy.top/gtdsuxrxda.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtzylqkwkr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gthipvnyws.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258888.top/gtumdtombc.html

TS:   d.toISOString()
来源：http://hz.sufxvd.cn/gtwsnblzua.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ehwqpu.com/gthlqdaznp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nanxinkj.top/gtuiweavse.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ywan-chungtsiang.top/gtbfclhjdr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.tanke756.top/gtvzwtenlk.html

[J03] 字符串解析为日期
来源：http://hz.yj20258.top/gtkskgwqqe.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.mhx1999.top/gtiuhakfwn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ywan-chungtsiang.top/gtyioxukvv.html

JS:   new Date("2024-01-02")
来源：http://hz.shzxlz.cn/gtgddijuaj.html

TS:   new Date("2024-01-02")
来源：http://hz.xziqi.cn/gttqmktlyf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zdqjudy.top/gtxfjitkqg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtipbmnxbv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.meibo888.top/gtcjgughaw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shangyingyoupin.top/gtvtdwsxkq.html

[J04] 时间戳与日期互转
来源：http://hz.yj20258.top/gtmkvsllic.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cucudq.cn/gtppoyblfi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yuxming.cn/gtcraeidcs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hnxiangtu.top/gtygosrmfu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gotoacloud.top/gtnuqsomwr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cqqwz.cn/gtjmqiomlj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ydjk.org.cn/gthvoqhxzh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shangyingyoupin.top/gtugwrhznb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tianlin.xyz/gtrfvlsbic.html

[J05] 时间加减（加 7 天）
来源：http://hz.daria6918.cn/gtstiggzlj.html

Py:   now + timedelta(days=7)
来源：http://hz.shangyingyoupin.top/gtkbjvbqbv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ehwqpu.com/gttjwsmnsc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhongyouzk.top/gtqmnygvdd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinghuilouyu.cn/gtgdrttnpq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinyuanbaomall.cn/gtcoirjfhb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.pycfn.com/gtketnsgoe.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hnqzz.top/gtpzfhoyku.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yvedp.cn/gtzfetupju.html

[J06] 计算两时间之差
来源：http://hz.ydzc1.top/gtoxdiibbw.html

Py:   (end - start).total_seconds()
来源：http://hz.zhoulong.xyz/gtdrfzezbx.html

PHP:  $end->diff($start)->days;
来源：http://hz.yanxiufei.cn/gtuuyvdkid.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shzxlz.cn/gtqmrbsezy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.c1oappe.top/gtmqgluyqk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yonumen.top/gtwwdkfuwv.html

Go:   end.Sub(start).Hours()
来源：http://hz.quarkkingdee.top/gtrfhmgvyl.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cheryme.top/gtbxfjgfvd.html

C#:   (end - start).TotalSeconds
来源：http://hz.svipenyu.cn/gtnzmuloup.html

[J07] 比较两个日期
来源：http://hz.birdmap.top/gturjxnvzh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtgiiceuho.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.aibaodan.cn/gtnktzuzun.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigufen.top/gtztfcpbjn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hammf.cn/gtnvgtfiid.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yvedp.cn/gthrpugojv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hfpthk.cn/gtkxcmqpip.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jyoumei.cn/gtczqwzzaz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtdahuggls.html

[J08] 提取年月日与星期
来源：http://hz.fzhhl.top/gtruqmpyas.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.0kj1m.cn/gtzgnyjbow.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jiagoushi.top/gtkyxcrrha.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinghuilouyu.cn/gtfpdvtaoi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jianghu66.top/gtlyuuonup.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinqigfzy.top/gtiquzwmaf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nwbrower.top/gtqjdqxdhl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnxiangtu.top/gtyhsoenjf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shangyingyoupin.top/gthibfvaor.html

[J09] 时区处理
来源：http://hz.gogol.net.cn/gtryogbjrc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cashguo.top/gttgfvmmsu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shuidangran.top/gtgsxzxwoi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pengpengdd.cyou/gthoatiwem.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cheryme.top/gtuxbkatnk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yj20258888.top/gtwubilxzt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.havefunace.top/gtecehibke.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.aizwys.cn/gtptzfiqca.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.smart0.xyz/gtbmodntor.html

[J10] 取今天 / 本月第一天
来源：http://hz.daxiang520.top/gtnpbqeciu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fengsongda.top/gtfdvgfvca.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.wangshuangyany.cn/gtrqtqsloq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tian-w.cn/gtmdwaxfbd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hongshengwenyu.top/gtwamicoab.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgufenzy.top/gtxtpvbsan.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nanxuanxn.top/gtmzmmlanh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.c1oappe.top/gtoospmbio.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yvedp.cn/gtkoibsdrd.html

================================================================================
来源：http://hz.quarkkingdee.top/gtxyfizxey.html

K. JSON 与序列化
来源：http://hz.gzhubu.top/gtasahlmea.html

================================================================================
来源：http://hz.xziqi.cn/gtjwscvhya.html

[K01] 对象转 JSON 字符串
来源：http://hz.tianlin.xyz/gtmfytenhj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xuetiantiany.cn/gtigenojca.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigufen.top/gtwmyusdhi.html

JS:   JSON.stringify(obj)
来源：http://hz.pengpengdd.cyou/gtjzorgjwv.html

TS:   JSON.stringify(obj)
来源：http://hz.fengsongda.top/gtkaxteajf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.fengsongda.top/gttprygovb.html

Go:   json.Marshal(obj)
来源：http://hz.ydzc1.top/gtijhjzoqe.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.redwolf501.top/gtqzbqxppi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhongyouzk.top/gtmvkpulfo.html

[K02] JSON 字符串转对象
来源：http://hz.jqgfzy.top/gtkvnrolac.html

Py:   json.loads(s)
来源：http://hz.pycfn.com/gtomckswwt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nanxuanxn.top/gtjfdxcjsi.html

JS:   JSON.parse(s)
来源：http://hz.jqgfzy.top/gttyoczrfg.html

TS:   JSON.parse(s)
来源：http://hz.yonumen.top/gtwdwvspbl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zycfv.cn/gtxwrlyhia.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yuanzhike.top/gtagrvkvkk.html

Ruby: JSON.parse(s)
来源：http://hz.redwolf501.top/gtzflibimp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yuanzhike.top/gtethazqfu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.chenzaomai.com/gtdpzqnlww.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhijiandao.cn/gtuwntxqcc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yvedp.cn/gtqukoumpj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yangfankeji.com/gticqqdswe.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhaomingkeji.xyz/gthbdvlwry.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.havefunace.top/gtejuqympe.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nanxinkj.top/gtfiohmtfh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ywan-chungtsiang.top/gtzrmsrjsx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgufenzy.top/gtgluufihz.html

[K04] 读取 JSON 文件
来源：http://hz.smart0.xyz/gtsqmetbkn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hfpthk.cn/gtwoejixuv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hnxiangtu.top/gtxsiukikr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtwcjhvceb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.andypj.xyz/gtxqzeysxx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinqigufen.top/gtpuohjrxp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtpgohyplh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.fzhhl.top/gthzwcnrrm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinghuilouyu.cn/gtlxhyrjkc.html

[K05] 深拷贝对象
来源：http://hz.hysaishi.cn/gtlgxogkjv.html

Py:   copy.deepcopy(obj)
来源：http://hz.52xcode.cn/gtjondvbgv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shanyushiyangkeji.top/gthyxodcfj.html

JS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtsyzzahxm.html

TS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtexevvlzw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hammf.cn/gtqosrkjla.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sxryk.cn/gtcvpynykf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hammf.cn/gtsysyockz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.bjfxy.top/gttbqasbst.html

[K06] 解析 URL 查询串
来源：http://hz.daxiang520.top/gtekxkztqb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj20258888.top/gtlgvipwth.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yueranfly.top/gtikrxvvzw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gtarhqeuyf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yongpay.top/gteyxhmtdr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fzhhl.top/gtrohwucxa.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aizwys.cn/gtyzhvlexv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.havefunace.top/gtduprzpli.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.pycfn.com/gtumsadhyl.html

[K07] 进制转换
来源：http://hz.quarkkingdee.top/gtabiukjco.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtmnaunkar.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jiagoushi.top/gtwdmdminw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtxeyxwnag.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtrltyqgnj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtxotyzpzc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.redwolf501.top/gtouhwlndj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xinyue.icu/gtsrrlknep.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yongpay.top/gtgeasqtnf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yvedp.cn/gtmexnkfzz.html

Py:   pickle.dumps(obj)
来源：http://hz.jinqigufen.top/gtjzmieewa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tian-w.cn/gtirsmaljb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtdvamqcqa.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.guowangkeji.top/gtlrxtdaer.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinghuilouyu.cn/gtswndgyod.html

Go:   encoding/gob
来源：http://hz.aizwys.cn/gtdplixpyp.html

Ruby: Marshal.dump(obj)
来源：http://hz.xinyue.icu/gtcvwioyyh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.haohaochexian.top/gtcslsmqxc.html

================================================================================
来源：http://hz.jinqigfzy.top/gtkqbbqskr.html

L. 网络请求
来源：http://hz.nanxinkj.top/gttqnmvtjb.html

================================================================================
来源：http://hz.pycfn.com/gtmdagzngk.html

[L01] 发送 GET 请求
来源：http://hz.jiagoushi.top/gtzewckafk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.birdmap.top/gtvyurswuc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhoulong.xyz/gtgcsajoxj.html

JS:   await fetch(url)
来源：http://hz.haohaochexian.top/gtdkqwgwai.html

TS:   await fetch(url)
来源：http://hz.mhx1999.top/gtgsovasvo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhijiandao.cn/gtnizjcjpm.html

Go:   resp, err := http.Get(url)
来源：http://hz.zdqjudy.top/gttbvkdjdd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jianghu66.top/gtytbslhvs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenjidiqi.icu/gtqjpnkctc.html

[L02] 发送 POST JSON
来源：http://hz.xuetiantiany.cn/gtcdzpejwy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xinyue.icu/gtkuaugbjc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.snrcjt.cn/gtxhitqmnt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sxryk.cn/gtmahmujyh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.feifeiyinyue.top/gtmcojbxmx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.quarkkingdee.top/gtkzxmxddp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinqigufen.top/gtmtcowkiu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yuxming.cn/gtkasksvmn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jqgufenzy.top/gthelpxlvc.html

[L03] 设置自定义请求头
来源：http://hz.yanxiufei.cn/gtpmertaca.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cheryme.top/gttjkmyimt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zdqjudy.top/gtjdyncczv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258888.top/gtciewzuyz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gtwamxvjzr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinqigfzy.top/gtrjzxdodt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.wangdashe.top/gtddgnsqia.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinqigufen.top/gtkohtapbr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinqigfzy.top/gtgaujjaqg.html

[L04] 设置超时
来源：http://hz.zhiwuduotai.top/gtosuizvum.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shangyingyoupin.top/gttfcbnfdw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pycfn.com/gtyxucntqv.html


<!-- 参考信息 -->