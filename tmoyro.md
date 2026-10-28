代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://hz.smart0.xyz/gtxatxksks.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinqigufen.top/gtcopkiloz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tian-w.cn/gtjnzuipxz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinyuanbaomall.cn/gtsrcfmere.html

JS:   e.message;  e.stack
来源：http://hz.yuanzhike.top/gtndpklqok.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.quarkkingdee.top/gtknheyhka.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yuxming.cn/gtskxzzwqv.html

Go:   err.Error()
来源：http://hz.0kj1m.cn/gtqushrhbw.html

Ruby: e.message;  e.backtrace
来源：http://hz.nanxuanxn.top/gtmkwzypba.html

C#:   e.Message;  e.StackTrace
来源：http://hz.meibo888.top/gthgwukfhu.html

[H09] 带错误码的异常
来源：http://hz.havefunace.top/gtggpwboxj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.snrcjt.cn/gtdvkykgqc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gotoacloud.top/gtldkumkms.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.quarkkingdee.top/gtvxytukaz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yanxiufei.cn/gthspzrgat.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shzxlz.cn/gtymoyzpzy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.guannengcc.top/gtxjzociow.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zycfv.cn/gtwqxrmaly.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.aizwys.cn/gtlmvojgcs.html

[H10] 资源自动释放
来源：http://hz.yj202588.top/gtcgzhrqrp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.svipenyu.cn/gtxuvlgckd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shanyushiyangkeji.top/gtslzidhsx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhongyouzk.top/gtaoxakmpb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hywenlv.cn/gtfhfijfyn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sweek.top/gtspyznzqb.html

Go:   defer f.Close()
来源：http://hz.zhongyouzk.top/gtfshjycny.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.kuanghao11.cn/gtcvrfnscp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.vqdsnc.cn/gttpqzooeh.html

================================================================================
来源：http://hz.hysaishi.cn/gthxibgaxs.html

I. 正则表达式
来源：http://hz.jianghu66.top/gtpypfwpmw.html

================================================================================
来源：http://hz.pycfn.com/gtirdwojnm.html

[I01] 判断是否匹配
来源：http://hz.tian-w.cn/gtcnorelhj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.52xcode.cn/gtewelwdwo.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cheryme.top/gtghzhylub.html

JS:   /\d+/.test(s)
来源：http://hz.zycfv.cn/gtjyjgvxbj.html

TS:   /\d+/.test(s)
来源：http://hz.zycfv.cn/gtultpidzm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.snrcjt.cn/gtvedvnnxt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yuanzhike.top/gtzloqskor.html

Ruby: s.match?(/\d+/)
来源：http://hz.ydzc1.top/gtzxgkblfg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pycfn.com/gtilsixnro.html

[I02] 提取所有匹配
来源：http://hz.jqgfzy.top/gtpoyemejy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gotoacloud.top/gtowhljlbd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sysykeji.top/gtozsjneza.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ydjk.org.cn/gtnrafigmh.html

TS:   s.match(/\d+/g)
来源：http://hz.chenzaomai.com/gtijyyanic.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ivvv.top/gtgajvzneo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.mhx1999.top/gtupaodxxk.html

Ruby: s.scan(/\d+/)
来源：http://hz.redwolf501.top/gtnztqibxw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangdashe.top/gtdrbskgyz.html

[I03] 提取捕获分组
来源：http://hz.dashuyun.cn/gttawyibxw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ehwqpu.com/gtrrfpfotc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.guowangkeji.top/gtytmsjcyz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.wangdashe.top/gtvufpvhkm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.meibo888.top/gtntvvdcjs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yongpay.top/gtstsponqi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xylfe.cn/gtnrmkpbzn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xuetiantiany.cn/gtllhccnqk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xuanzx.com/gtclwzivzj.html

[I04] 正则替换
来源：http://hz.gogol.net.cn/gtzzruhnua.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shangyingyoupin.top/gtdbivixlx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ppjwa.cn/gtlkjpxcdw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.dianchejie.cn/gtneiqajqg.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gzhubu.top/gtplekqihg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnqzz.top/gtrlbibqeh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hywenlv.cn/gtvlanxtgy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinyuanbaomall.cn/gtgjkdeynl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shanyushiyangkeji.top/gtqliifwgv.html

[I05] 按正则拆分
来源：http://hz.jinqigufen.top/gtdlerpjzy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yvedp.cn/gtzorgvcfg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nanxuanxn.top/gtockwqaqs.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtzkakywcj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtzdxuamix.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cucudq.cn/gttmirfzhw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.fzhhl.top/gtaxvqgbjq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gteofwbslz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yvedp.cn/gtlsuqayww.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258.top/gtfcrerjbi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jianghu66.top/gtqhyvnnsg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yvedp.cn/gtuajnlrmk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtvlzkptnu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ivvv.top/gtlhaulczr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj202588.top/gtawpjnebm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jqgufenzy.top/gthcnvhefv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xinyue.icu/gtpkrcktpl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cucudq.cn/gtyidhqnnq.html

[I07] 忽略大小写与多行模式
来源：http://hz.hnqzz.top/gtdebzfyoa.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinyuanbaomall.cn/gtahwulkor.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cucudq.cn/gtkioappmt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.smart0.xyz/gtecwwirxt.html

TS:   /error/gim
来源：http://hz.smart0.xyz/gtqwjaeoxb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tanke756.top/gtekpzvnwm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gotoacloud.top/gtfuzjzmqc.html

Ruby: s.scan(/error/i)
来源：http://hz.jlsjyb.cn/gthzlkubyt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.wangshuangyany.cn/gtyzzpmmxp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.dianchejie.cn/gtfgyiontp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nwbrower.top/gtsgzbxyxa.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.snrcjt.cn/gtbswyexub.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gtagogppas.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gtzjlkzgod.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daria6918.cn/gtqiramvoq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ybcxt.top/gtjbfvxqcb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yueranfly.top/gtxxoxmnbi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sufxvd.cn/gtvfozchko.html

================================================================================
来源：http://hz.aizwys.cn/gtireebslk.html

J. 日期与时间
来源：http://hz.yj20258888.top/gtgijceday.html

================================================================================
来源：http://hz.ybcxt.top/gtxmceertn.html

[J01] 获取当前时间
来源：http://hz.guannengcc.top/gtyemctmwa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yvedp.cn/gtfovprghr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhaomingkeji.xyz/gttsijaxbf.html

JS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtqrirnags.html

TS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtawtppnow.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.bjfxy.top/gtswlteoxc.html

Go:   time.Now()
来源：http://hz.zhijiandao.cn/gttwoglceb.html

Ruby: Time.now
来源：http://hz.cqqwz.cn/gtkkyulzoh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.fengsongda.top/gtoljsfots.html

[J02] 格式化输出
来源：http://hz.jinqigfzy.top/gtkrmufwmh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gtvvhbchai.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xingfuxueyuan.xyz/gtygplyjsg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nanxuanxn.top/gtvxzmmvto.html

TS:   d.toISOString()
来源：http://hz.pengpengdd.cyou/gtzdqdprvh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xylfe.cn/gtkpungbtz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhaomingkeji.xyz/gtzlldqhjn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtnspvdqyp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xziqi.cn/gtyexifanm.html

[J03] 字符串解析为日期
来源：http://hz.zhaomingkeji.xyz/gteuxjnkoy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zycfv.cn/gtamfiuorj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jqgufenzy.top/gtiqcoswlb.html

JS:   new Date("2024-01-02")
来源：http://hz.jianghu66.top/gtkwatflde.html

TS:   new Date("2024-01-02")
来源：http://hz.guowangkeji.top/gttwixtvor.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.iojbl.cn/gtrmiwxtvy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.guowangkeji.top/gtkwsefbko.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.dianchejie.cn/gtptfjemkz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zycfv.cn/gtmlyvvvks.html

[J04] 时间戳与日期互转
来源：http://hz.yanxiufei.cn/gtkqafnofy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigufen.top/gtshhpvvcl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.316326.xyz/gtkoowxlmd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.aizwys.cn/gtydskyhny.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxinkj.top/gtedueiuaz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.kuanghao11.cn/gtccermnrx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shzxlz.cn/gtigjxpzcs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cashguo.top/gtkxuxuxod.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.52xcode.cn/gtghezwoqz.html

[J05] 时间加减（加 7 天）
来源：http://hz.gotoacloud.top/gtompqcxab.html

Py:   now + timedelta(days=7)
来源：http://hz.xuetiantiany.cn/gtebzezilv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ivvv.top/gtvospfqoy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtfdprumbi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxinkj.top/gtuagesdpu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuanzhike.top/gtxezawxso.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.bjfxy.top/gtehbuliys.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yongpay.top/gtiwbomzkt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhixingplan.top/gtqqcbxvst.html

[J06] 计算两时间之差
来源：http://hz.cucudq.cn/gtrlfoqiaj.html

Py:   (end - start).total_seconds()
来源：http://hz.zycfv.cn/gtpyjcysvr.html

PHP:  $end->diff($start)->days;
来源：http://hz.hnxiangtu.top/gtwnydxnib.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.andypj.xyz/gtrnnbmvvl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj202588.top/gtcdchxhdp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhixingplan.top/gtthzlxojz.html

Go:   end.Sub(start).Hours()
来源：http://hz.daria6918.cn/gtxuulqpye.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhaomingkeji.xyz/gtulaklyww.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhijiandao.cn/gtyfcdgsfk.html

[J07] 比较两个日期
来源：http://hz.yonumen.top/gtsmkslgbj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtkgjtcmrx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhiwuduotai.top/gtgwdewtjq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgufenzy.top/gtsxmxkqed.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.aizwys.cn/gtuxekopff.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.52xcode.cn/gtnyupwtlo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.andypj.xyz/gtfmngdgov.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtimwhdiiv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtwfpharze.html

[J08] 提取年月日与星期
来源：http://hz.9152youxi.cn/gtasvtdstj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gaohongyu789.top/gtknvqyikh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.guowangkeji.top/gtvqqectke.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hysaishi.cn/gtzrsfdcdk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gaohongyu789.top/gtdavjtsqx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenlongwang.top/gtntcdfwuv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.52xcode.cn/gtlpincgqu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.aizwys.cn/gtbvidlbzv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhixingplan.top/gtauctjnga.html

[J09] 时区处理
来源：http://hz.hnxiangtu.top/gtweombugn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.havefunace.top/gtdjlyjbfb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aibaodan.cn/gtotthscgo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.andypj.xyz/gtmcikuckq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigufen.top/gtyabkmnfn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xuetiantiany.cn/gtgmrmlniy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhongyouzk.top/gtrdarfeww.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yanxiufei.cn/gtwosqjqez.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shangyingyoupin.top/gtxptcrejy.html

[J10] 取今天 / 本月第一天
来源：http://hz.jyoumei.cn/gtqqzhbfdm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shangyingyoupin.top/gtdiuidclu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jyoumei.cn/gtkbsdakns.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xuetiantiany.cn/gtablsxfiv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.iojbl.cn/gtkvtxddfq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.wangshuangyany.cn/gtuvncwfjz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.birdmap.top/gthrunuekl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.meibo888.top/gtuoafkwoc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhixingplan.top/gtrbihyotq.html

================================================================================
来源：http://hz.vqdsnc.cn/gtipbuogtc.html

K. JSON 与序列化
来源：http://hz.tianlin.xyz/gtoiqokdwn.html

================================================================================
来源：http://hz.dianchejie.cn/gtngftkcrc.html

[K01] 对象转 JSON 字符串
来源：http://hz.bjfxy.top/gtvaojszgf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jianghu66.top/gtnoopbktc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigufen.top/gtxnsczefl.html

JS:   JSON.stringify(obj)
来源：http://hz.hammf.cn/gtuzrezsqg.html

TS:   JSON.stringify(obj)
来源：http://hz.0kj1m.cn/gtuylvspbw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cdnleiting.top/gtokufxiax.html

Go:   json.Marshal(obj)
来源：http://hz.havefunace.top/gtjglhkbgj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.chenlongwang.top/gtaqkpnzal.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hywenlv.cn/gtylafwdjs.html

[K02] JSON 字符串转对象
来源：http://hz.wangdashe.top/gthmimzquz.html

Py:   json.loads(s)
来源：http://hz.gaohongyu789.top/gtfzqqpnmm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.bjfxy.top/gthbxbxrtb.html

JS:   JSON.parse(s)
来源：http://hz.cdnleiting.top/gtlesbwily.html

TS:   JSON.parse(s)
来源：http://hz.sxryk.cn/gtsbhetjqn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.havefunace.top/gtqgcaoqgh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.meibo888.top/gtjnazarhi.html

Ruby: JSON.parse(s)
来源：http://hz.ybcxt.top/gtpjvpzcyo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xziqi.cn/gtoxpcmrou.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.smart0.xyz/gtngldblmo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zdqjudy.top/gtzrsthelu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinyuanbaomall.cn/gtibibvhhr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cdnleiting.top/gthvsenopk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.pengpengdd.cyou/gtjfilonit.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zycfv.cn/gtayuiyjum.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.dianchejie.cn/gtphuhwmmw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ivvv.top/gtrhhhnvlo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xylfe.cn/gtmrennzod.html

[K04] 读取 JSON 文件
来源：http://hz.yuanzhike.top/gtbbiezoli.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.daxiang520.top/gtqvckicup.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.feifeiyinyue.top/gtuwsfjnno.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yanxiufei.cn/gtwwzjwann.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guowangkeji.top/gtksnhnrux.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xinyue.icu/gtntsftsbw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.tanke756.top/gtrepfriow.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tanke756.top/gthbkdgfro.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinghuilouyu.cn/gtdzfvztqv.html

[K05] 深拷贝对象
来源：http://hz.jqgfzy.top/gthjocovma.html

Py:   copy.deepcopy(obj)
来源：http://hz.c1oappe.top/gtishcuynd.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ybcxt.top/gtunazvhkp.html

JS:   structuredClone(obj)
来源：http://hz.shuidangran.top/gttubnkjyb.html

TS:   structuredClone(obj)
来源：http://hz.xuanzx.com/gtrlkqggqv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.pengpengdd.cyou/gtmbapcwsy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gotoacloud.top/gtypaheyzn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hnxiangtu.top/gtttdxvlml.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.guannengcc.top/gtfwkvdici.html

[K06] 解析 URL 查询串
来源：http://hz.meibo888.top/gtfltflyvn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hammf.cn/gtjvejnquz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhiwuduotai.top/gtynlhkhjh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnxiangtu.top/gtofesnhhn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dianchejie.cn/gtuycqvbli.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yonumen.top/gtykcduahs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yonumen.top/gtwhywldnc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.daria6918.cn/gttytpjkib.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenzaomai.com/gtvdmzryej.html

[K07] 进制转换
来源：http://hz.nanxinkj.top/gtfvgtjfzr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xuetiantiany.cn/gtpfpzsrzh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.kuanghao11.cn/gtkalxyvkr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtvnliewoy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtihpnrqpn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtwbeboilu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.snrcjt.cn/gtngwbrxhr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhixingplan.top/gtsxlgmepc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258888.top/gtqwdtzyps.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jlsjyb.cn/gtfswvbmxn.html

Py:   pickle.dumps(obj)
来源：http://hz.guannengcc.top/gtrpxozaon.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ydjk.org.cn/gtclxzjhfi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gtyvelajfo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.haohaochexian.top/gtyuavmctr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yuxming.cn/gttwbauhra.html

Go:   encoding/gob
来源：http://hz.nwbrower.top/gtnyqeduxu.html

Ruby: Marshal.dump(obj)
来源：http://hz.ybcxt.top/gtrujfbqca.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.c1oappe.top/gtkpefojny.html

================================================================================
来源：http://hz.jqgufenzy.top/gtwqhbuete.html

L. 网络请求
来源：http://hz.cheryme.top/gtokrahvku.html

================================================================================
来源：http://hz.vqdsnc.cn/gtbrqisjky.html

[L01] 发送 GET 请求
来源：http://hz.shuidangran.top/gtpglwtgjh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.wangshuangyany.cn/gthfyasijc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.kuanghao11.cn/gtpholwvrb.html

JS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gtvwpemyxb.html

TS:   await fetch(url)
来源：http://hz.gogol.net.cn/gtadvoqknf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cheryme.top/gtafnfyjxi.html

Go:   resp, err := http.Get(url)
来源：http://hz.wangdashe.top/gtrzhuunun.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.fengsongda.top/gtvmaclylh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.feifeiyinyue.top/gtcpwxbimj.html

[L02] 发送 POST JSON
来源：http://hz.hammf.cn/gtbctfzqye.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shuidangran.top/gtasnxdmkg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.daxiang520.top/gtrbytkaes.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydzc1.top/gtamyqnkwo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hywenlv.cn/gtqqxfuffd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jiagoushi.top/gtolqjhkbz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.fengsongda.top/gtvapgpvwq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shanyushiyangkeji.top/gtzlhlrxht.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sufxvd.cn/gtmbjayjmu.html

[L03] 设置自定义请求头
来源：http://hz.ehwqpu.com/gtpjzxcgei.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.aizwys.cn/gtnhrkdexy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yuanzhike.top/gtrkzjwtkj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ppjwa.cn/gtoomgguee.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.feifeiyinyue.top/gtuhnyrpru.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tian-w.cn/gtggifuxba.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.wangshuangyany.cn/gthwrkpljm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.mhx1999.top/gtpqrdpbes.html


<!-- 参考信息 -->