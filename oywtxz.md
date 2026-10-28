代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hnqzz.top/gthkjfotgn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.chenjidiqi.icu/gtdylpmbpi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhixingplan.top/gtalscnvnu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.quarkkingdee.top/gtcjezbqdv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zycfv.cn/gtthyglvwk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jianghu66.top/gtkqgmwjwv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yonumen.top/gtjxvcnybk.html

[H10] 资源自动释放
来源：http://hz.iojbl.cn/gtzzsiprfg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sweek.top/gtyjrrmsps.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shanyushiyangkeji.top/gtdrvvsfbk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daria6918.cn/gthshktmeo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yanxiufei.cn/gtmvjqldcm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gaohongyu789.top/gtiaryesij.html

Go:   defer f.Close()
来源：http://hz.andypj.xyz/gttntxkzwr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinqigfzy.top/gtnoesorto.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jlsjyb.cn/gtulqnvryu.html

================================================================================
来源：http://hz.yj20258888.top/gtbxfyukhx.html

I. 正则表达式
来源：http://hz.zdqjudy.top/gttkfswoku.html

================================================================================
来源：http://hz.andypj.xyz/gtndnsguxu.html

[I01] 判断是否匹配
来源：http://hz.tian-w.cn/gtrrhxivzu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.pycfn.com/gtqtlsukzj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.mhx1999.top/gtxxcztgym.html

JS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gtaatemjyc.html

TS:   /\d+/.test(s)
来源：http://hz.c1oappe.top/gtzbksxatv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yuxming.cn/gttpmgvmfq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gaohongyu789.top/gtdwinjkzp.html

Ruby: s.match?(/\d+/)
来源：http://hz.shuidangran.top/gtkxxzalpx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.redwolf501.top/gtuhkkulhi.html

[I02] 提取所有匹配
来源：http://hz.yj202588.top/gtpdxbgvqa.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ppjwa.cn/gtpkhiavzg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ivvv.top/gtktsyafle.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tianlin.xyz/gtoevozqyo.html

TS:   s.match(/\d+/g)
来源：http://hz.daxiang520.top/gterelmvqj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ehwqpu.com/gtwkgpgjwh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.kuanghao11.cn/gtulrykcpw.html

Ruby: s.scan(/\d+/)
来源：http://hz.zycfv.cn/gtncqodkbe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.quarkkingdee.top/gtnkqqajrq.html

[I03] 提取捕获分组
来源：http://hz.ivvv.top/gtjrhdsrhz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shanyushiyangtech.top/gtdheyovsq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yvedp.cn/gtmhnwlyre.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gogol.net.cn/gtopalpzhf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xziqi.cn/gtfsrohske.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuetiantiany.cn/gtfhnanooe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xingfuxueyuan.xyz/gtrbbvotks.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yonumen.top/gttksdaaxs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hysaishi.cn/gttwnqoass.html

[I04] 正则替换
来源：http://hz.cashguo.top/gtnnelupow.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cqqwz.cn/gtrhgspgxw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuanzhike.top/gtusyscrum.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xinyue.icu/gtffpmbwnw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gtmnfvwyxa.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenlongwang.top/gtcgvpjmjm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dashuyun.cn/gtjovstkse.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yj202588.top/gtoqkqbfei.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yj20258.top/gtsfkclsmm.html

[I05] 按正则拆分
来源：http://hz.feifeiyinyue.top/gtwajzshnl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.nanxuanxn.top/gtzfwgmaab.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ywan-chungtsiang.top/gtdxpnbrcu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gtffsmgwox.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtopgpfdrr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jianghu66.top/gtuiqnlumj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenlongwang.top/gtzxizijno.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtctsqarku.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gotoacloud.top/gtspmsbqqg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.fengsongda.top/gtwtckumlk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ydjk.org.cn/gtrfwbbuhr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.redwolf501.top/gtxfiyudvt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xinyue.icu/gtosvgrudg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhengqikj.top/gtyaaxietg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhijiandao.cn/gtzpvkveof.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cashguo.top/gtljqtclhk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.dashuyun.cn/gtiwtftcdh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.guowangkeji.top/gtrldkgyly.html

[I07] 忽略大小写与多行模式
来源：http://hz.gotoacloud.top/gthogpbpjr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shanyushiyangkeji.top/gtrixhivia.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ehwqpu.com/gtdowoyiek.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.iojbl.cn/gtqduqijpm.html

TS:   /error/gim
来源：http://hz.zhongyouzk.top/gtiwjiakcn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.quarkkingdee.top/gtklamxdaw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zycfv.cn/gtgpbsajwc.html

Ruby: s.scan(/error/i)
来源：http://hz.zhixingplan.top/gtixkyxflz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.dashuyun.cn/gtbneozbno.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.52xcode.cn/gtofnipcjs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cucudq.cn/gtkdxfsfwt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.aizwys.cn/gtpbxyypxr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuxming.cn/gtnjtciwof.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sufxvd.cn/gturadmofh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.fengsongda.top/gtomuatbvm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ehwqpu.com/gtsiyrjfqf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nwbrower.top/gtoyazucbn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ywan-chungtsiang.top/gtowpodgyx.html

================================================================================
来源：http://hz.pycfn.com/gtnikblouu.html

J. 日期与时间
来源：http://hz.dianchejie.cn/gtllfzermq.html

================================================================================
来源：http://hz.vqdsnc.cn/gtucyumuzf.html

[J01] 获取当前时间
来源：http://hz.hysaishi.cn/gtehpnkfgn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shuidangran.top/gtfnvrcvmg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtfhfahjif.html

JS:   new Date();  Date.now()
来源：http://hz.yangfankeji.com/gtohmxuokk.html

TS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gtchixndqk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.316326.xyz/gtwwrahjau.html

Go:   time.Now()
来源：http://hz.wangshuangyany.cn/gtfkxnmnwx.html

Ruby: Time.now
来源：http://hz.yonumen.top/gtandkctyt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangkeji.top/gtfuikzkmv.html

[J02] 格式化输出
来源：http://hz.xinyue.icu/gtcavpotuc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ivvv.top/gthynquqsv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtdjkhzgxf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cheryme.top/gtrihwhaag.html

TS:   d.toISOString()
来源：http://hz.fzhhl.top/gtnujfijyl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hfpthk.cn/gtncewugge.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.fengsongda.top/gtybuyqrst.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydjk.org.cn/gtfnldsysh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.feifeiyinyue.top/gtbjjzvwqb.html

[J03] 字符串解析为日期
来源：http://hz.nanxuanxn.top/gtjqatpbfy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgfzy.top/gtvhgqmiaz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj202588.top/gtlqjvbwlm.html

JS:   new Date("2024-01-02")
来源：http://hz.gogol.net.cn/gtivomkghy.html

TS:   new Date("2024-01-02")
来源：http://hz.316326.xyz/gtmcpyiela.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj20258.top/gtvtounjil.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sysykeji.top/gtungwmaiy.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtbxubtbvc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinghuilouyu.cn/gtgvrtyvmz.html

[J04] 时间戳与日期互转
来源：http://hz.cqqwz.cn/gthropexmu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.iojbl.cn/gtbmunlqso.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhoulong.xyz/gtfjuddukg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hnqzz.top/gtqlpawchh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxinkj.top/gtuyelsxpe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sufxvd.cn/gtyyielbwy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hnqzz.top/gtwrwkdhar.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.c1oappe.top/gtwkpeqzcc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hnqzz.top/gtucuwccsy.html

[J05] 时间加减（加 7 天）
来源：http://hz.bjfxy.top/gtosmplxru.html

Py:   now + timedelta(days=7)
来源：http://hz.dianchejie.cn/gtzsmfmhqt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shangyingyoupin.top/gtmrwhfikj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gtzrwtdxcx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hongshengwenyu.top/gtpjmffsqn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pycfn.com/gtnjqjhsgi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.52xcode.cn/gtqvdogcxk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.daxiang520.top/gtucmgctqw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.mhx1999.top/gtpohhsnqw.html

[J06] 计算两时间之差
来源：http://hz.yongpay.top/gtzopmyifa.html

Py:   (end - start).total_seconds()
来源：http://hz.aibaodan.cn/gtukbmhfte.html

PHP:  $end->diff($start)->days;
来源：http://hz.jqgufenzy.top/gtjbmlxzwv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.meibo888.top/gtgtedxfkm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xziqi.cn/gtsnnpvsdw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gogol.net.cn/gtfzlppjdc.html

Go:   end.Sub(start).Hours()
来源：http://hz.tanke756.top/gthcbmdyen.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yangfankeji.com/gthskficjn.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhixingplan.top/gtkrijmgag.html

[J07] 比较两个日期
来源：http://hz.bjfxy.top/gtxcdbqqyj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtxruajzbm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cucudq.cn/gtovzspbwe.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gogol.net.cn/gtduvwxbmb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cheryme.top/gtdtnvllqc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shanyushiyangtech.top/gtqguovczc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cqqwz.cn/gtpnubdibk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtadcokayh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinghuilouyu.cn/gtfxnwlavs.html

[J08] 提取年月日与星期
来源：http://hz.shangyingyoupin.top/gtlkmhloux.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xingfuxueyuan.xyz/gtgcpqdxaq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.havefunace.top/gtakzhmggl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yj202588.top/gtehdhfhsf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hfpthk.cn/gtjxwibgar.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sysykeji.top/gthifpkytp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xinyue.icu/gtxfcjllwe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gotoacloud.top/gtsrzawyev.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yvedp.cn/gtllybfend.html

[J09] 时区处理
来源：http://hz.zhongyouzk.top/gtmdsffbfx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jyoumei.cn/gtsruzyyjg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.316326.xyz/gtziebnumu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tianlin.xyz/gtkidcugfh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigfzy.top/gtpgtjkifj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenjidiqi.icu/gtiswgrere.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.mhx1999.top/gtboovpwff.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cheryme.top/gtxoxfgrva.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.feifeiyinyue.top/gtwifttyru.html

[J10] 取今天 / 本月第一天
来源：http://hz.svipenyu.cn/gtyvlgobsy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shuidangran.top/gtcmwdjjhq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gotoacloud.top/gtkvnghygj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aizwys.cn/gtacdlgtlm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yueranfly.top/gtcpegzjbn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.pengpengdd.cyou/gtegeoldpm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuxming.cn/gtfxbkemst.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yueranfly.top/gtijwyqcgu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nanxuanxn.top/gtnqcjprhl.html

================================================================================
来源：http://hz.birdmap.top/gthlxgwoym.html

K. JSON 与序列化
来源：http://hz.hnxiangtu.top/gtcykwutmo.html

================================================================================
来源：http://hz.yj202588.top/gtecxxdirr.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydjk.org.cn/gtfgufzhfg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zdqjudy.top/gtyavbxeob.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtuuhromls.html

JS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gtvfkltzqn.html

TS:   JSON.stringify(obj)
来源：http://hz.ivvv.top/gtautapbmh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yueranfly.top/gtefvqokqm.html

Go:   json.Marshal(obj)
来源：http://hz.haohaochexian.top/gtvqscjcfd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shangyingyoupin.top/gtregvmevv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yj20258.top/gtqkhagpwk.html

[K02] JSON 字符串转对象
来源：http://hz.sweek.top/gttgspodrm.html

Py:   json.loads(s)
来源：http://hz.jianghu66.top/gtoifjfvjx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.svipenyu.cn/gtdbtfneyi.html

JS:   JSON.parse(s)
来源：http://hz.9152youxi.cn/gtmuwjcwan.html

TS:   JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtsosyrtfh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhoulong.xyz/gticyjqxlr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.redwolf501.top/gtglbiwcgc.html

Ruby: JSON.parse(s)
来源：http://hz.hnqzz.top/gtvhwsewbx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.redwolf501.top/gtsmyijcyg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.guowangkeji.top/gtrfasltlb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenzaomai.com/gtimkpxsed.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ivvv.top/gtmoyyzoez.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnxiangtu.top/gtdkfbnwxl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtvuotqtel.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.9152youxi.cn/gtyglpavlg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.redwolf501.top/gtiydsfpem.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cucudq.cn/gtcvcljbld.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.pengpengdd.cyou/gtbzgnnxcm.html

[K04] 读取 JSON 文件
来源：http://hz.sxryk.cn/gtgppplcfo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuanzhike.top/gtpmufkmxd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shangyingyoupin.top/gtjmcmzauw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xylfe.cn/gtykbkmkem.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtqhhuizuu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yongpay.top/gtfxooirae.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gtejpyxmnb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jiagoushi.top/gtmqldkorm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yuxming.cn/gthacgkfpf.html

[K05] 深拷贝对象
来源：http://hz.vqdsnc.cn/gtjqjiyqrg.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinqigfzy.top/gtocuklokv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jianghu66.top/gtclozkvbu.html

JS:   structuredClone(obj)
来源：http://hz.gotoacloud.top/gthbwhgdxp.html

TS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtbnxhvzao.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhoulong.xyz/gtmmdzdlpk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenzaomai.com/gtowilhfht.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sysykeji.top/gtctnpzogr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.dianchejie.cn/gtdnxbpade.html

[K06] 解析 URL 查询串
来源：http://hz.xylfe.cn/gtoxmqcovj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cdnleiting.top/gtrvkgmgbw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.fzhhl.top/gtjrtspjlm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yangfankeji.com/gtmcxzdjuy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tianlin.xyz/gtfersddut.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenzaomai.com/gtrnlkaygs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yueranfly.top/gtnutkzumj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.mhx1999.top/gtyascwovw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shangyingyoupin.top/gtozpphpnw.html

[K07] 进制转换
来源：http://hz.haohaochexian.top/gtfwpsxfbz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.aizwys.cn/gtvwgxittj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydjk.org.cn/gtdvndvjjy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cashguo.top/gtoorztkss.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.52xcode.cn/gtncnnfxtk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtwuslrcgi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yueranfly.top/gtscbphwtf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.316326.xyz/gtzymqfzsz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.daxiang520.top/gtwuqnzfot.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.guannengcc.top/gtthotsvbe.html

Py:   pickle.dumps(obj)
来源：http://hz.tian-w.cn/gtbjpsdyte.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.chenjidiqi.icu/gtupkiqphw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gtzxmucpkb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.snrcjt.cn/gtedymapsp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gogol.net.cn/gtevsfwkzs.html

Go:   encoding/gob
来源：http://hz.mhx1999.top/gtmvnoxhzh.html

Ruby: Marshal.dump(obj)
来源：http://hz.yuanzhike.top/gtumigzfxp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cashguo.top/gtbawiamvg.html

================================================================================
来源：http://hz.gogol.net.cn/gtdepvduzy.html

L. 网络请求
来源：http://hz.ivvv.top/gtunphxdes.html

================================================================================
来源：http://hz.fengsongda.top/gtcveuupty.html

[L01] 发送 GET 请求
来源：http://hz.gaohongyu789.top/gtyrkxysmf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jlsjyb.cn/gtzxctydwz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.haohaochexian.top/gttbcpkaxp.html

JS:   await fetch(url)
来源：http://hz.aibaodan.cn/gtghseqyhl.html

TS:   await fetch(url)
来源：http://hz.sysykeji.top/gtoeebxwkx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ivvv.top/gtubfqgkui.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhongyouzk.top/gtdikanigj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xingfuxueyuan.xyz/gtypsnrwjd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yueranfly.top/gtdjnlptqa.html

[L02] 发送 POST JSON
来源：http://hz.xuanzx.com/gtrgfiemdm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgfzy.top/gtcwzexopz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.guannengcc.top/gthswktubz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtwbevafmh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jyoumei.cn/gtjcuwjcpf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.tian-w.cn/gtsqfzpgkj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yueranfly.top/gtbysjdpia.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.chenzaomai.com/gtaeqpcccp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sweek.top/gtwkuwlzjr.html

[L03] 设置自定义请求头
来源：http://hz.wangshuangyany.cn/gtftchovhw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigufen.top/gtlfynsjpw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gaohongyu789.top/gtwkxsmktd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtloqmznfh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shangyingyoupin.top/gtlmebwalo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hnqzz.top/gtiaxglffa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.smart0.xyz/gtojgtydvk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhiwuduotai.top/gthgedtjrn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nwbrower.top/gterxcoqdi.html

[L04] 设置超时
来源：http://hz.zhengqikj.top/gthjhpgcrl.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jyoumei.cn/gtsygmmkeu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhijiandao.cn/gtkjtwxhgi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shanyushiyangkeji.top/gtfdwnadgv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gtvrlwfhex.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.birdmap.top/gtgkbyykqx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ehwqpu.com/gtivdjwlar.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.smart0.xyz/gtjkcenyny.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.vqdsnc.cn/gtflrdtfzo.html

[L05] 上传文件（multipart）
来源：http://hz.quarkkingdee.top/gtursurvks.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yvedp.cn/gtuhpmdiji.html


<!-- 参考信息 -->