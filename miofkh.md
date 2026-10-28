代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fzhhl.top/gtiebsghdn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.fengsongda.top/gtfouelvdp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.feifeiyinyue.top/gtldbstrcz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.pycfn.com/gtbpvrftuh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hysaishi.cn/gtetfltyfg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.aibaodan.cn/gtcohrkbit.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hfpthk.cn/gtckkmrwnc.html

[H10] 资源自动释放
来源：http://hz.havefunace.top/gtkcpjjflw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.kuanghao11.cn/gtlrqxlxgp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gaohongyu789.top/gtsdusvxgo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangkeji.top/gtpsxdctrf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guannengcc.top/gtijdcqlmn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zycfv.cn/gtqtpbrxus.html

Go:   defer f.Close()
来源：http://hz.zhiwuduotai.top/gtmoxhufaq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xziqi.cn/gtkklchpli.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangkeji.top/gttaixmusw.html

================================================================================
来源：http://hz.yuxming.cn/gtkpaphvvx.html

I. 正则表达式
来源：http://hz.meibo888.top/gtywvfrcez.html

================================================================================
来源：http://hz.sysykeji.top/gtnftdrqbt.html

[I01] 判断是否匹配
来源：http://hz.jlsjyb.cn/gtapfnadpn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xingfuxueyuan.xyz/gtjczjwkkw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gzhubu.top/gtnqkzcdrh.html

JS:   /\d+/.test(s)
来源：http://hz.ydzc1.top/gtjokrwdjf.html

TS:   /\d+/.test(s)
来源：http://hz.quarkkingdee.top/gtvfrriasi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.iojbl.cn/gtibjohcfm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.feifeiyinyue.top/gtpelvmamy.html

Ruby: s.match?(/\d+/)
来源：http://hz.pycfn.com/gtaeadphzb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xziqi.cn/gttgccatfi.html

[I02] 提取所有匹配
来源：http://hz.pycfn.com/gtqswwflqu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ywan-chungtsiang.top/gtganilfin.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jlsjyb.cn/gtayijeppf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xziqi.cn/gtoquhbqbq.html

TS:   s.match(/\d+/g)
来源：http://hz.316326.xyz/gtpciqlizy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.andypj.xyz/gthmcvibod.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.mhx1999.top/gtrhpkinnt.html

Ruby: s.scan(/\d+/)
来源：http://hz.cucudq.cn/gtehbcxplm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.daria6918.cn/gtevxzromt.html

[I03] 提取捕获分组
来源：http://hz.cashguo.top/gtfctrnnww.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj20258.top/gtvedvndin.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shzxlz.cn/gtjwunsexl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hysaishi.cn/gtacjxjutg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.wangshuangyany.cn/gtvagmjctb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuetiantiany.cn/gtwxtwqysz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sxryk.cn/gtgjeodadl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gogol.net.cn/gtcoywctyd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.tanke756.top/gtodytryan.html

[I04] 正则替换
来源：http://hz.zhoulong.xyz/gtoncahhtp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cheryme.top/gtfrrhnbhm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xinyue.icu/gtyoajwkue.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.guowangkeji.top/gtkmjyaaju.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtqrrapaxv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.quarkkingdee.top/gtbxqwkztm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.svipenyu.cn/gtbtbsqmfc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.iojbl.cn/gtoczyslgm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhengqikj.top/gtfbccwxfa.html

[I05] 按正则拆分
来源：http://hz.jqgufenzy.top/gtlihxyide.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gaohongyu789.top/gtmjrfuosc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhongyouzk.top/gtphdvcfra.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gtdcagrtib.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cdnleiting.top/gtaovkgnfj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.haohaochexian.top/gtkkfqrizh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gaohongyu789.top/gtrectbxuj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtaafztbcn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.iojbl.cn/gtfzchmvnt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xinyue.icu/gtofdvvzsu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cashguo.top/gtuivdsyke.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hysaishi.cn/gtlbgfyity.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.svipenyu.cn/gtimxlmojt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jiagoushi.top/gtpnxfnsky.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nanxinkj.top/gtcspohzhl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jlsjyb.cn/gtemodffad.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.fzhhl.top/gtgpcanebx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.dashuyun.cn/gtqajakuok.html

[I07] 忽略大小写与多行模式
来源：http://hz.xuanzx.com/gtwhvjeqvk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tianlin.xyz/gtpnhiehzj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shangyingyoupin.top/gtgrpprjew.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.svipenyu.cn/gteqagibki.html

TS:   /error/gim
来源：http://hz.jyoumei.cn/gthcwvuusw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gzhubu.top/gtewrvvpii.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.316326.xyz/gttryndyod.html

Ruby: s.scan(/error/i)
来源：http://hz.nanxuanxn.top/gtdpmcvrpi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinqigfzy.top/gtjpjicbti.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.redwolf501.top/gtbhfgimej.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yanxiufei.cn/gtuducgcmu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shanyushiyangtech.top/gtseevddcq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.0kj1m.cn/gtmlfpxflk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pengpengdd.cyou/gtjiriqeob.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.iojbl.cn/gtihreyghq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ppjwa.cn/gtusfdedit.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shangyingyoupin.top/gtaqbjapre.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.dashuyun.cn/gthneghuda.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtwedrbpov.html

J. 日期与时间
来源：http://hz.andypj.xyz/gtcyqxdvuq.html

================================================================================
来源：http://hz.zhixingplan.top/gtfzrexqgv.html

[J01] 获取当前时间
来源：http://hz.bjfxy.top/gtzjsmifyy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.aizwys.cn/gtilqzxzls.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xuanzx.com/gtsmmxiddj.html

JS:   new Date();  Date.now()
来源：http://hz.vqdsnc.cn/gtqiyqxwiv.html

TS:   new Date();  Date.now()
来源：http://hz.zhaomingkeji.xyz/gtabhwgksz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.wangdashe.top/gtpesyezlk.html

Go:   time.Now()
来源：http://hz.xziqi.cn/gtolvommcf.html

Ruby: Time.now
来源：http://hz.cdnleiting.top/gtifumcuqu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cheryme.top/gtoxdyqhlh.html

[J02] 格式化输出
来源：http://hz.bjfxy.top/gthtxalrty.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtuukwmdoo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gaohongyu789.top/gtmelarell.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhiwuduotai.top/gtsructevt.html

TS:   d.toISOString()
来源：http://hz.hywenlv.cn/gtjlwwzmuc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cheryme.top/gtgifqxkqb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.kuanghao11.cn/gtqmlxycge.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gtkdyatyxf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.9152youxi.cn/gthksndaez.html

[J03] 字符串解析为日期
来源：http://hz.chenjidiqi.icu/gtdojxffmx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.quarkkingdee.top/gtxwupzcpl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fengsongda.top/gtfetjdxvb.html

JS:   new Date("2024-01-02")
来源：http://hz.aibaodan.cn/gtrapukafu.html

TS:   new Date("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtbtcwfhnp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gotoacloud.top/gtapdkzfrm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.haohaochexian.top/gtulscsbco.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ybcxt.top/gthoplmysc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cashguo.top/gthoneszlg.html

[J04] 时间戳与日期互转
来源：http://hz.yueranfly.top/gtybedayrs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.guannengcc.top/gtqcsfuqen.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenlongwang.top/gtcpexhyvd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hammf.cn/gtkvruvfcv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.redwolf501.top/gtlhacvuki.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xuanzx.com/gtwvzcwlvz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zycfv.cn/gtyucjjdoo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cucudq.cn/gtzkgdfafp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hammf.cn/gtfjpqccse.html

[J05] 时间加减（加 7 天）
来源：http://hz.mhx1999.top/gtmnkfksbl.html

Py:   now + timedelta(days=7)
来源：http://hz.jinyuanbaomall.cn/gthbcrbkdl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.svipenyu.cn/gtvdomaodt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.52xcode.cn/gtrseafbzg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigufen.top/gtafjikhir.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xylfe.cn/gtoeeymszl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.iojbl.cn/gttnwzdtsg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhengqikj.top/gtpkrrivpy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.birdmap.top/gttelfgeop.html

[J06] 计算两时间之差
来源：http://hz.ydzc1.top/gtrjprfagc.html

Py:   (end - start).total_seconds()
来源：http://hz.yanxiufei.cn/gtgwsayfpz.html

PHP:  $end->diff($start)->days;
来源：http://hz.jiagoushi.top/gtbiniawdx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.meibo888.top/gtlsvgdscp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.tianlin.xyz/gtnkeozlyt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.fengsongda.top/gtdkxnfini.html

Go:   end.Sub(start).Hours()
来源：http://hz.yuanzhike.top/gtsmkkonzj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jlsjyb.cn/gthiksbrqv.html

C#:   (end - start).TotalSeconds
来源：http://hz.jianghu66.top/gtwsdtvqvr.html

[J07] 比较两个日期
来源：http://hz.vqdsnc.cn/gthofgeduw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtgtbljukh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.redwolf501.top/gtwvfirokq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.wangdashe.top/gtoioeexup.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenjidiqi.icu/gtklsouorq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dianchejie.cn/gtwmaswybl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ehwqpu.com/gtfdhpvnyi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtdckalfry.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yvedp.cn/gtvkwgqvdy.html

[J08] 提取年月日与星期
来源：http://hz.redwolf501.top/gtfkfntxhu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gzhubu.top/gtfmgzpilk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hywenlv.cn/gthfywxhat.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zycfv.cn/gtenixrylf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sweek.top/gtvairktke.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.tanke756.top/gtqupnzzjb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.aibaodan.cn/gturjbmhoy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daxiang520.top/gtpmvrqoxx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xingfuxueyuan.xyz/gtdhornfrf.html

[J09] 时区处理
来源：http://hz.feifeiyinyue.top/gtkoxbhbal.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinghuilouyu.cn/gtbdmeeufy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shzxlz.cn/gtnbetbdvb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cqqwz.cn/gtgkqzsxzk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.andypj.xyz/gtvquyrfah.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sweek.top/gtacudmxxz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sxryk.cn/gtwsrfbomb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.feifeiyinyue.top/gttxzozimk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhiwuduotai.top/gtyxnkkyfn.html

[J10] 取今天 / 本月第一天
来源：http://hz.yonumen.top/gtjhnmtevp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.svipenyu.cn/gtfjkrgmpw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xziqi.cn/gtkmjjyiwr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.fengsongda.top/gtklkoddih.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.pengpengdd.cyou/gtwcmjeaug.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sufxvd.cn/gtzwmdzwfs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jqgfzy.top/gtzmlxqnqc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cdnleiting.top/gtjtemyvpm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cqqwz.cn/gtaiciyrvk.html

================================================================================
来源：http://hz.xinyue.icu/gtvuveuach.html

K. JSON 与序列化
来源：http://hz.xziqi.cn/gtwbpnutaj.html

================================================================================
来源：http://hz.zycfv.cn/gtcqqkjdqm.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinyuanbaomall.cn/gtilljmxjo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hongshengwenyu.top/gtdfbxsqdy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinyuanbaomall.cn/gtukbwytcn.html

JS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gtvdmhvmce.html

TS:   JSON.stringify(obj)
来源：http://hz.snrcjt.cn/gtmdnqmjwx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shangyingyoupin.top/gtlfvhbdiw.html

Go:   json.Marshal(obj)
来源：http://hz.gogol.net.cn/gtgodbegci.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shanyushiyangkeji.top/gtnhzfordw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.fzhhl.top/gtyzuuayzv.html

[K02] JSON 字符串转对象
来源：http://hz.jiagoushi.top/gtqiztqsbo.html

Py:   json.loads(s)
来源：http://hz.daria6918.cn/gtwiechsbh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.snrcjt.cn/gttpdhvfka.html

JS:   JSON.parse(s)
来源：http://hz.iojbl.cn/gtnrcklsym.html

TS:   JSON.parse(s)
来源：http://hz.52xcode.cn/gtsnctnibp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cdnleiting.top/gtzbtcqbix.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj202588.top/gtjpvpalaq.html

Ruby: JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtypxgncer.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.fzhhl.top/gttgogionp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ppjwa.cn/gtbtzewlzb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.aibaodan.cn/gteblmfovq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xuetiantiany.cn/gtxciziszs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.aizwys.cn/gttaseetsl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuanzhike.top/gthpbkcipu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.bjfxy.top/gttaagnwuk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.fengsongda.top/gtwiainqdk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.fengsongda.top/gtbivarjbs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangshuangyany.cn/gtxvqmpkbt.html

[K04] 读取 JSON 文件
来源：http://hz.andypj.xyz/gtxifzfxhr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.redwolf501.top/gtypoacger.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jiagoushi.top/gttuoucvwm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.vqdsnc.cn/gtrihxnbvg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hfpthk.cn/gtydibllvb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.snrcjt.cn/gtejdgiifv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtzlkuwfjs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hammf.cn/gtyzrnjxpz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tianlin.xyz/gtgssqposm.html

[K05] 深拷贝对象
来源：http://hz.zdqjudy.top/gtyelkbbmk.html

Py:   copy.deepcopy(obj)
来源：http://hz.hysaishi.cn/gtrkfifokj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zdqjudy.top/gtilrripat.html

JS:   structuredClone(obj)
来源：http://hz.nanxinkj.top/gtfiawlhhz.html

TS:   structuredClone(obj)
来源：http://hz.hfpthk.cn/gtybsdyuix.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhijiandao.cn/gtpmpzarbj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xuanzx.com/gtsgzuzkud.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenjidiqi.icu/gtomffoqwi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gogol.net.cn/gtdnubjtoh.html

[K06] 解析 URL 查询串
来源：http://hz.yuxming.cn/gteugyyupn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xylfe.cn/gtjhgvnphh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.fzhhl.top/gtcmusprus.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sxryk.cn/gtvmenlndb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yueranfly.top/gtvddnjykv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhengqikj.top/gtypnxpvvh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinqigufen.top/gtapzehanu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hammf.cn/gtvisfjrsd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.daxiang520.top/gtzikddiga.html

[K07] 进制转换
来源：http://hz.zhengqikj.top/gtskfcdges.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shuidangran.top/gtomdoxlbo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yonumen.top/gtpnammlgj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtdsmpkirk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtkyyjjbzp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtrccknjgx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hywenlv.cn/gtvagbyuic.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zdqjudy.top/gtjssmxtck.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xziqi.cn/gtpbwyvhwv.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.52xcode.cn/gtarsgkcqx.html

Py:   pickle.dumps(obj)
来源：http://hz.nwbrower.top/gtmmvbveuu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hysaishi.cn/gtvzhqybrd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hnqzz.top/gtkavyejtw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhixingplan.top/gtnyhjdvob.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cdnleiting.top/gtjpkgzrxs.html

Go:   encoding/gob
来源：http://hz.jyoumei.cn/gtsrdgikkr.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinyuanbaomall.cn/gtxohigxko.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sysykeji.top/gtglzeaoxo.html

================================================================================
来源：http://hz.zdqjudy.top/gtzkgkbglh.html

L. 网络请求
来源：http://hz.52xcode.cn/gtswjyqnuq.html

================================================================================
来源：http://hz.dianchejie.cn/gtgjcnawkw.html

[L01] 发送 GET 请求
来源：http://hz.yueranfly.top/gtihduniyn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cashguo.top/gtwdaxacqw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jlsjyb.cn/gtyphlulqy.html

JS:   await fetch(url)
来源：http://hz.c1oappe.top/gtnucddhua.html

TS:   await fetch(url)
来源：http://hz.hysaishi.cn/gtjoziagun.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zdqjudy.top/gttyprrvlg.html

Go:   resp, err := http.Get(url)
来源：http://hz.gaohongyu789.top/gtipbzxsxf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yvedp.cn/gtfsiniljp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zycfv.cn/gtfsiaqeas.html

[L02] 发送 POST JSON
来源：http://hz.zhaomingkeji.xyz/gtgilchsuh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sysykeji.top/gtufdhztlk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yueranfly.top/gtahwgugtl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.snrcjt.cn/gtenoynjel.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gaohongyu789.top/gtjoenuyzv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.nwbrower.top/gtxcijlflo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hfpthk.cn/gtlkspfbff.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xinyue.icu/gtpwdsrcya.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.snrcjt.cn/gtwrjclxki.html

[L03] 设置自定义请求头
来源：http://hz.andypj.xyz/gtsjinzjoy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hywenlv.cn/gtgegkquaj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhongyouzk.top/gtgptwjlmm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.c1oappe.top/gtqduhlgjf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxinkj.top/gtaejdylka.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ppjwa.cn/gtccdewjdl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.aizwys.cn/gtnypqfobp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yvedp.cn/gtpgtllasl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gotoacloud.top/gtpelnqcdv.html

[L04] 设置超时
来源：http://hz.daxiang520.top/gtdhywoslw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xingfuxueyuan.xyz/gtzsmwqvnc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pycfn.com/gtbtjznecq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sweek.top/gtulcutvwu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgufenzy.top/gtakizanai.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.birdmap.top/gtskssfpxa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.wangshuangyany.cn/gtkubgjnpp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.kuanghao11.cn/gtgpymmidd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nanxuanxn.top/gtthdlbpmo.html

[L05] 上传文件（multipart）
来源：http://hz.yonumen.top/gtifogzgqk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hfpthk.cn/gtditokscg.html


<!-- 参考信息 -->