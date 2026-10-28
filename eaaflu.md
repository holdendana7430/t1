代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.feifeiyinyue.top/gtcnjlkcph.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jyoumei.cn/gtovcwwgja.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.guowangkeji.top/gtodavuodo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258.top/gtittfitdu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xinyue.icu/gtoufvvbyy.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shanyushiyangtech.top/gtturuvqkh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jqgfzy.top/gtfhqfayrx.html

[H10] 资源自动释放
来源：http://hz.yuanzhike.top/gtuuqozxnk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ydjk.org.cn/gtxzsozpkf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nanxuanxn.top/gtyfpxbawl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.andypj.xyz/gtvjmbbtji.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hammf.cn/gtwqjimret.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ehwqpu.com/gthtvonddq.html

Go:   defer f.Close()
来源：http://hz.ybcxt.top/gtfqqxyibv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.pengpengdd.cyou/gtsprafwif.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cdnleiting.top/gtumlhegkc.html

================================================================================
来源：http://hz.yj20258888.top/gthoewooco.html

I. 正则表达式
来源：http://hz.jlsjyb.cn/gtlbwzjkcu.html

================================================================================
来源：http://hz.9152youxi.cn/gtlgjnbkrk.html

[I01] 判断是否匹配
来源：http://hz.yongpay.top/gtsvwesnnm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.pengpengdd.cyou/gttntokwcn.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gotoacloud.top/gtbiodgtby.html

JS:   /\d+/.test(s)
来源：http://hz.gzhubu.top/gtbestjfgt.html

TS:   /\d+/.test(s)
来源：http://hz.gotoacloud.top/gthvqrkfuk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydzc1.top/gtyvqvofnw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.havefunace.top/gtulrqbjzk.html

Ruby: s.match?(/\d+/)
来源：http://hz.gotoacloud.top/gtkllwvbwd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.daxiang520.top/gtatzphxll.html

[I02] 提取所有匹配
来源：http://hz.chenjidiqi.icu/gtybitxqsl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtmubwnctc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhijiandao.cn/gtoiofhttc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.feifeiyinyue.top/gteklhowuw.html

TS:   s.match(/\d+/g)
来源：http://hz.sufxvd.cn/gtvlfaumjh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hnqzz.top/gtofyngxyk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hfpthk.cn/gtpeoxfbxj.html

Ruby: s.scan(/\d+/)
来源：http://hz.gotoacloud.top/gtmepixvma.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.kuanghao11.cn/gtezhuneig.html

[I03] 提取捕获分组
来源：http://hz.hnxiangtu.top/gtcbyqfpbj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sysykeji.top/gteuwqqrba.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ppjwa.cn/gtlujlarda.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shanyushiyangtech.top/gtjpybkmmt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhoulong.xyz/gttmnxgwbw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.c1oappe.top/gttlnaocnn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.guannengcc.top/gtkhsntotv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenlongwang.top/gtrzrzqhqm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xziqi.cn/gtvzdgiryy.html

[I04] 正则替换
来源：http://hz.cashguo.top/gtxgsthwip.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zdqjudy.top/gtftstnmtr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhengqikj.top/gtlkldrrcj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.haohaochexian.top/gtzqkvotwh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtckqxqycg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xuanzx.com/gtmuglxaue.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tianlin.xyz/gtgbzhxlnw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnxiangtu.top/gtzpewlvfq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.svipenyu.cn/gtcuznjbpn.html

[I05] 按正则拆分
来源：http://hz.cdnleiting.top/gtmympxdgg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hfpthk.cn/gtbbcrhxgc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.pycfn.com/gtbdqmfqae.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gttemtyzmm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258888.top/gtjdthtxws.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinqigfzy.top/gtouwudmyp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hnqzz.top/gtrxpwlcyi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtirpbliml.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jlsjyb.cn/gtyjalyrzu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shuidangran.top/gtktdhwjvn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtbbrcakic.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.chenlongwang.top/gtmidqrhrt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nwbrower.top/gtuvlkeoqz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtpfbwuqhk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cqqwz.cn/gtbzjkcksv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.mhx1999.top/gtizzocubd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sysykeji.top/gtacvadsxm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.tianlin.xyz/gtutdnyumn.html

[I07] 忽略大小写与多行模式
来源：http://hz.zdqjudy.top/gtxecdlada.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.bjfxy.top/gtbjuogeux.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.smart0.xyz/gtwimstwfs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ydzc1.top/gtbtfgifgc.html

TS:   /error/gim
来源：http://hz.pengpengdd.cyou/gtqpbrqyrq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.andypj.xyz/gtkrtzoqpm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pengpengdd.cyou/gtmhouybok.html

Ruby: s.scan(/error/i)
来源：http://hz.pengpengdd.cyou/gtgxcdntyi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.havefunace.top/gtwhwzzuzw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shuidangran.top/gttrhnnybl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yongpay.top/gtdxsajzrg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.dianchejie.cn/gtylxyhywg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guowangkeji.top/gtjzbasjfb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxuanxn.top/gtmykkycwk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shanyushiyangkeji.top/gtcgnnsfyn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinghuilouyu.cn/gtchbjhhdf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hongshengwenyu.top/gtqggkwusj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shangyingyoupin.top/gthhahvyad.html

================================================================================
来源：http://hz.haohaochexian.top/gtgrdhbamj.html

J. 日期与时间
来源：http://hz.redwolf501.top/gtypvfckst.html

================================================================================
来源：http://hz.sxryk.cn/gtjsneliul.html

[J01] 获取当前时间
来源：http://hz.yongpay.top/gtmncarqbm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gtvaenynds.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gtfrydoxof.html

JS:   new Date();  Date.now()
来源：http://hz.zhoulong.xyz/gtirmxgfbz.html

TS:   new Date();  Date.now()
来源：http://hz.andypj.xyz/gtxxwponhb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sysykeji.top/gtrvnjiadt.html

Go:   time.Now()
来源：http://hz.kuanghao11.cn/gtscoqaqau.html

Ruby: Time.now
来源：http://hz.ybcxt.top/gtufhktsbv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenjidiqi.icu/gtvnhlkcta.html

[J02] 格式化输出
来源：http://hz.zhiwuduotai.top/gtfznbzehb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinyuanbaomall.cn/gtpfcppobu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.pengpengdd.cyou/gtwtoqvzlp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.quarkkingdee.top/gtaejnrnvw.html

TS:   d.toISOString()
来源：http://hz.jinqigfzy.top/gtciqmrdob.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.52xcode.cn/gtppkqujtn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.snrcjt.cn/gtmintbmwb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydzc1.top/gtggrbepkr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gotoacloud.top/gtdmwngduz.html

[J03] 字符串解析为日期
来源：http://hz.shangyingyoupin.top/gtgcqerzbr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.daria6918.cn/gtozhoufal.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nanxuanxn.top/gtyvmzpmaa.html

JS:   new Date("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtguyzyiae.html

TS:   new Date("2024-01-02")
来源：http://hz.kuanghao11.cn/gtkavzgxlt.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ehwqpu.com/gtdnelvmla.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtopgczysy.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.wangdashe.top/gtfcgzbyjw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.wangshuangyany.cn/gtnrtwpnbf.html

[J04] 时间戳与日期互转
来源：http://hz.yanxiufei.cn/gtjkrhxloa.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shangyingyoupin.top/gttcqlwosy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gogol.net.cn/gtoimdpgmw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenlongwang.top/gtlmxszxwl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shangyingyoupin.top/gtapoxmrfc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sxryk.cn/gtxjbokvde.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zycfv.cn/gtbcsodxyq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.birdmap.top/gtlszidkdt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ivvv.top/gtgojkfpsh.html

[J05] 时间加减（加 7 天）
来源：http://hz.jqgufenzy.top/gthkvkybyg.html

Py:   now + timedelta(days=7)
来源：http://hz.zhengqikj.top/gtrevkelzu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yvedp.cn/gtnvltkllw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxuanxn.top/gtsfxnzctr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dianchejie.cn/gtcprysodn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yonumen.top/gtzxahowfz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yj202588.top/gtrmrcymmi.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xuanzx.com/gtzenugbsh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.c1oappe.top/gtjqnvcfed.html

[J06] 计算两时间之差
来源：http://hz.jqgfzy.top/gtxbwavhak.html

Py:   (end - start).total_seconds()
来源：http://hz.aibaodan.cn/gtmdrmogum.html

PHP:  $end->diff($start)->days;
来源：http://hz.fengsongda.top/gtyfpvshwo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ywan-chungtsiang.top/gtevxsnqcc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cucudq.cn/gtrloabpqo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenzaomai.com/gthzbuonur.html

Go:   end.Sub(start).Hours()
来源：http://hz.tanke756.top/gtnpnyodws.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tianlin.xyz/gtqoggmfze.html

C#:   (end - start).TotalSeconds
来源：http://hz.sxryk.cn/gtbsexcwjk.html

[J07] 比较两个日期
来源：http://hz.fzhhl.top/gtottwmfgi.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtquuttgxg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ybcxt.top/gtvuzkqysi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gthfsiyopn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtyclkksiw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.52xcode.cn/gttupjdssl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.birdmap.top/gtsisgbmnb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtazkaiiqc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtnuraawln.html

[J08] 提取年月日与星期
来源：http://hz.zhengqikj.top/gtesnzswpq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhijiandao.cn/gtdospgtqa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ywan-chungtsiang.top/gtwtkpuopr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shuidangran.top/gtatvgxxyl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yangfankeji.com/gttxhhmbvv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gogol.net.cn/gtrjmauxje.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sysykeji.top/gtbqrgzlns.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinyuanbaomall.cn/gtzoluxzsq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gogol.net.cn/gtrkzavgwv.html

[J09] 时区处理
来源：http://hz.jinyuanbaomall.cn/gtwinsecej.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tian-w.cn/gtfjbzqjhd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jqgufenzy.top/gtnklmvgrx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtsmvmnaxy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fzhhl.top/gtkpriqjor.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.feifeiyinyue.top/gtqfdlkvjg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gotoacloud.top/gtiqubksxd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yvedp.cn/gtkocsnvgq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.kuanghao11.cn/gtwwpwqadx.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhaomingkeji.xyz/gtgiazbfdh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cucudq.cn/gtogekiyrb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hammf.cn/gtmukocqwa.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jianghu66.top/gtwdidkxqs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ydjk.org.cn/gtxavgwxsj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hongshengwenyu.top/gtykpyfwzv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shzxlz.cn/gtfrpoajpn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cheryme.top/gtiotzdena.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhiwuduotai.top/gtrqzknwcu.html

================================================================================
来源：http://hz.nwbrower.top/gtcctaeoed.html

K. JSON 与序列化
来源：http://hz.jqgfzy.top/gtvcclgemh.html

================================================================================
来源：http://hz.zdqjudy.top/gtacgvsdkn.html

[K01] 对象转 JSON 字符串
来源：http://hz.snrcjt.cn/gtwauytucd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jqgfzy.top/gthoefvole.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gaohongyu789.top/gtrvukrelg.html

JS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtruznrapj.html

TS:   JSON.stringify(obj)
来源：http://hz.dianchejie.cn/gthzoggwam.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shzxlz.cn/gtpaasyfjk.html

Go:   json.Marshal(obj)
来源：http://hz.shzxlz.cn/gtipfbzoxt.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj20258.top/gtykpdffay.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.andypj.xyz/gtnecrbarg.html

[K02] JSON 字符串转对象
来源：http://hz.iojbl.cn/gtjovdvlle.html

Py:   json.loads(s)
来源：http://hz.pycfn.com/gtihgaxuom.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.pycfn.com/gtnmjyjmri.html

JS:   JSON.parse(s)
来源：http://hz.dianchejie.cn/gtmsiptvpu.html

TS:   JSON.parse(s)
来源：http://hz.yangfankeji.com/gteyshqsbq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xziqi.cn/gttdmoiaoa.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtelbhodkd.html

Ruby: JSON.parse(s)
来源：http://hz.fzhhl.top/gtkdrjjeiv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.mhx1999.top/gtbhmguwcc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.birdmap.top/gtywldmqcl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hywenlv.cn/gtmqtxutye.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gthvedyhsk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gtcztgfgtr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xziqi.cn/gtomjcxufq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.daria6918.cn/gtmsiqpipe.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.quarkkingdee.top/gtbdfqiowm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.quarkkingdee.top/gtuljocmln.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.daria6918.cn/gtzmpfmwir.html

[K04] 读取 JSON 文件
来源：http://hz.birdmap.top/gtyvbqauwj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ywan-chungtsiang.top/gtitluscvw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.kuanghao11.cn/gtcmifemzh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.quarkkingdee.top/gtmzrbygag.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258.top/gtbnvwclfm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hnqzz.top/gtfltttius.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yuxming.cn/gtugjelgzh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gaohongyu789.top/gtyfctrtxg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cucudq.cn/gtdupjyosi.html

[K05] 深拷贝对象
来源：http://hz.jinqigfzy.top/gtlegdxefs.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnxiangtu.top/gtluqlhwac.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yanxiufei.cn/gtmunjmlul.html

JS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtqjawqael.html

TS:   structuredClone(obj)
来源：http://hz.yonumen.top/gtxitugdje.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gaohongyu789.top/gtuzupdfoq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258.top/gtoletauhf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yueranfly.top/gtcrabmyir.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hammf.cn/gthovwrtry.html

[K06] 解析 URL 查询串
来源：http://hz.mhx1999.top/gtgdvsqfpf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.gotoacloud.top/gtprzlppqu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gzhubu.top/gtorkcnepq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yongpay.top/gtsspzofht.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yanxiufei.cn/gthqvbwtdb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258.top/gtipdfkagv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhiwuduotai.top/gtwfrgxibt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hfpthk.cn/gtqdntzafo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.havefunace.top/gtrqvcizhf.html

[K07] 进制转换
来源：http://hz.yanxiufei.cn/gtxjeywigt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zdqjudy.top/gtocinuwhf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shzxlz.cn/gtdnyufbpi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ehwqpu.com/gtkhwrbfwd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ivvv.top/gtrtineydw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yvedp.cn/gtobsisovr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jianghu66.top/gtxyvrdfma.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daxiang520.top/gtkqhqdobw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhongyouzk.top/gtzipidpyf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yangfankeji.com/gtvuusltba.html

Py:   pickle.dumps(obj)
来源：http://hz.sxryk.cn/gttntqplgn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cheryme.top/gtxvkxtzfu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gtafrxxfxu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gogol.net.cn/gtlwmykjya.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ydzc1.top/gtsaaftuyr.html

Go:   encoding/gob
来源：http://hz.9152youxi.cn/gtsndjllpe.html

Ruby: Marshal.dump(obj)
来源：http://hz.hongshengwenyu.top/gtductbzkz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jiagoushi.top/gtvylmjgta.html

================================================================================
来源：http://hz.gzhubu.top/gtsiskcjqf.html

L. 网络请求
来源：http://hz.xinyue.icu/gttnbnbxum.html

================================================================================
来源：http://hz.hammf.cn/gtbctaeasc.html

[L01] 发送 GET 请求
来源：http://hz.pengpengdd.cyou/gtoltyurmo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigufen.top/gtmpicivlt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydjk.org.cn/gtsuszhbxl.html

JS:   await fetch(url)
来源：http://hz.9152youxi.cn/gtsfllfxzz.html

TS:   await fetch(url)
来源：http://hz.xingfuxueyuan.xyz/gtjhoktnhv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj202588.top/gtfaqwwcxa.html

Go:   resp, err := http.Get(url)
来源：http://hz.hfpthk.cn/gthcoocccq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hnqzz.top/gtmgkcgfqp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xziqi.cn/gtoiypirfm.html

[L02] 发送 POST JSON
来源：http://hz.fengsongda.top/gtvzlpgven.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nanxinkj.top/gtnopxlbmt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhixingplan.top/gtlikhizjm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnqzz.top/gthbfqpuxp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gtmzgdduhs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhengqikj.top/gtxvtvattm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sxryk.cn/gtiwrahubl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.havefunace.top/gtzjxufsiy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hongshengwenyu.top/gtngewrtun.html

[L03] 设置自定义请求头
来源：http://hz.xuanzx.com/gtmhpqdckh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jqgufenzy.top/gtfoswzjgd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hongshengwenyu.top/gttlynzwno.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhiwuduotai.top/gtfnatpzxu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.haohaochexian.top/gthbdzkrab.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhijiandao.cn/gtofnrxaas.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenlongwang.top/gtsvtbqkqh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sysykeji.top/gtzjydezjm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nanxinkj.top/gtrmrypphc.html

[L04] 设置超时
来源：http://hz.dianchejie.cn/gtlhjjlxok.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xingfuxueyuan.xyz/gtmasozobi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cashguo.top/gtpnspmvjf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.52xcode.cn/gtfahcvgzw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cdnleiting.top/gtcquqylsl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.dianchejie.cn/gtojghjhwf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.havefunace.top/gtabkykqjc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.mhx1999.top/gtlpynuzpo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.pengpengdd.cyou/gtkuaufgzo.html

[L05] 上传文件（multipart）
来源：http://hz.bjfxy.top/gtjswvaqxv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sufxvd.cn/gtevniqmmf.html


<!-- 参考信息 -->