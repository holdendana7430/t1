代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jqgufenzy.top/gtfdcjmjjx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.wangshuangyany.cn/gttsogepen.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yanxiufei.cn/gtnasokrkj.html

C#:   obj?.A?.B ?? default
来源：http://hz.yangfankeji.com/gtyzvruhbz.html

[H07] 断言
来源：http://hz.ivvv.top/gtagpqktsb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gaohongyu789.top/gtqbtqcmnx.html

PHP:  assert($x > 0);
来源：http://hz.jinyuanbaomall.cn/gtfshpmrri.html

JS:   console.assert(x > 0);
来源：http://hz.jqgufenzy.top/gtluwqyrso.html

TS:   console.assert(x > 0);
来源：http://hz.bjfxy.top/gtduxusmnx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.aizwys.cn/gtmfoqnpuu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sxryk.cn/gtyvzeocsz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.9152youxi.cn/gtxoluynsk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtdwytxopm.html

[H08] 获取错误信息与堆栈
来源：http://hz.yueranfly.top/gtqkqyxhhn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydjk.org.cn/gtijgjeohf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hammf.cn/gtczkvqxqa.html

JS:   e.message;  e.stack
来源：http://hz.yuanzhike.top/gtafqukyyf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.andypj.xyz/gtwfnkhpbw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xziqi.cn/gteelriybh.html

Go:   err.Error()
来源：http://hz.shzxlz.cn/gtxveqmcot.html

Ruby: e.message;  e.backtrace
来源：http://hz.dashuyun.cn/gtrziquerq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tanke756.top/gtvrhumgji.html

[H09] 带错误码的异常
来源：http://hz.hfpthk.cn/gtdtozrfwt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhixingplan.top/gttmhwpwsz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ppjwa.cn/gtmyzvfprf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.9152youxi.cn/gtltbclrqy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.fzhhl.top/gtzkkqaptp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yongpay.top/gtpgdpduvx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhijiandao.cn/gtcrbymeqy.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xinyue.icu/gtowyupswy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.bjfxy.top/gtjxdwmsnf.html

[H10] 资源自动释放
来源：http://hz.bjfxy.top/gtfuthoxnv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhaomingkeji.xyz/gturwrziit.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhengqikj.top/gtlfvedvwn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtgmyifguq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtrccdwqrx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.snrcjt.cn/gturodsnzz.html

Go:   defer f.Close()
来源：http://hz.nanxuanxn.top/gtzsdfpbjp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ydzc1.top/gtcxtabdun.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shuidangran.top/gtbcecsiiu.html

================================================================================
来源：http://hz.jlsjyb.cn/gtlfziblib.html

I. 正则表达式
来源：http://hz.sweek.top/gtxylcutow.html

================================================================================
来源：http://hz.316326.xyz/gtqgdrjyvc.html

[I01] 判断是否匹配
来源：http://hz.shangyingyoupin.top/gtntctptqu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinyuanbaomall.cn/gtwfpfgdop.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aizwys.cn/gtmiesjlrp.html

JS:   /\d+/.test(s)
来源：http://hz.jinqigfzy.top/gtkjvvewlh.html

TS:   /\d+/.test(s)
来源：http://hz.fzhhl.top/gtrrahzwdb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnxiangtu.top/gtezckufyn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sxryk.cn/gtphrhwfre.html

Ruby: s.match?(/\d+/)
来源：http://hz.hfpthk.cn/gtcjbayeya.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.chenzaomai.com/gtocogozpn.html

[I02] 提取所有匹配
来源：http://hz.ydzc1.top/gtlsizpqpz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nanxinkj.top/gtkuijexxz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.wangshuangyany.cn/gtmkzlhihy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhongyouzk.top/gttxtfalpl.html

TS:   s.match(/\d+/g)
来源：http://hz.tanke756.top/gtejkdfzgi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xuanzx.com/gtzdkergyc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tanke756.top/gtkxfjpaop.html

Ruby: s.scan(/\d+/)
来源：http://hz.fengsongda.top/gtlijakvwi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj20258.top/gtbznjshut.html

[I03] 提取捕获分组
来源：http://hz.cheryme.top/gtwpaaoltl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.svipenyu.cn/gtrwptpptz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.daria6918.cn/gtpfiysder.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj20258888.top/gtfwyqsptb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ppjwa.cn/gtdejvninn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenjidiqi.icu/gtqcrwnavw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shangyingyoupin.top/gtbnvptgdb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yangfankeji.com/gthoptgeyd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.dashuyun.cn/gtgbovffyj.html

[I04] 正则替换
来源：http://hz.zdqjudy.top/gthekjthwz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.guannengcc.top/gtjwlguesr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jyoumei.cn/gtpuspgynn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gtehxdpdns.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shuidangran.top/gtuayvdyri.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinyuanbaomall.cn/gtxdlfiqgm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj20258.top/gtbeyphnfe.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yj202588.top/gtvhvreeqj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.9152youxi.cn/gtnsompcau.html

[I05] 按正则拆分
来源：http://hz.tanke756.top/gtijpysfht.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zycfv.cn/gthuuslian.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ehwqpu.com/gtcgsrqswd.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinghuilouyu.cn/gtshcviuvs.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtvmxhdmvy.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yj202588.top/gtshvzljjs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yuanzhike.top/gtezpxabqv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.birdmap.top/gtbogovcpu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.havefunace.top/gtiapehaqf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cashguo.top/gtqhiatabr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhijiandao.cn/gtpspethxu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gotoacloud.top/gtlwbzrjwm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.redwolf501.top/gturpyrosn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cqqwz.cn/gtbrsmyklc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cqqwz.cn/gtdengprba.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sxryk.cn/gtvnwqcsnq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.fengsongda.top/gthrgvrnga.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gtujxirrjf.html

[I07] 忽略大小写与多行模式
来源：http://hz.gotoacloud.top/gtoiramjtl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sxryk.cn/gtdcsihfrt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinqigfzy.top/gtqqcsouft.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ydzc1.top/gtvrjztoje.html

TS:   /error/gim
来源：http://hz.quarkkingdee.top/gtlfdpedeu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gaohongyu789.top/gtiykvtydt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.chenlongwang.top/gtslydipms.html

Ruby: s.scan(/error/i)
来源：http://hz.zycfv.cn/gthikhzkaq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yvedp.cn/gtrpvqxktu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ydjk.org.cn/gtwtxeemdu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shanyushiyangkeji.top/gtvbuqcoge.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinyuanbaomall.cn/gtfcfvsmef.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sufxvd.cn/gtiexvrzce.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtbfdyublh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.0kj1m.cn/gtyevdpzdn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sxryk.cn/gtoakjsncr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hnqzz.top/gtepeqecbb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cucudq.cn/gtbpvisncz.html

================================================================================
来源：http://hz.hnxiangtu.top/gtobzagphn.html

J. 日期与时间
来源：http://hz.yanxiufei.cn/gtrzanwirn.html

================================================================================
来源：http://hz.tanke756.top/gtmqdchdkf.html

[J01] 获取当前时间
来源：http://hz.meibo888.top/gtqvuwccnm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hnqzz.top/gtujfadgja.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xingfuxueyuan.xyz/gtltsrtahd.html

JS:   new Date();  Date.now()
来源：http://hz.shzxlz.cn/gtucebrqwe.html

TS:   new Date();  Date.now()
来源：http://hz.316326.xyz/gtrleontdk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinghuilouyu.cn/gtrdpmtgpl.html

Go:   time.Now()
来源：http://hz.316326.xyz/gtkxnikzvv.html

Ruby: Time.now
来源：http://hz.iojbl.cn/gtpincglie.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sysykeji.top/gtpirykihq.html

[J02] 格式化输出
来源：http://hz.zhixingplan.top/gtwaxqluhz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gtbfyyfzjc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.wangdashe.top/gtuficwewv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.guannengcc.top/gtawtrehnk.html

TS:   d.toISOString()
来源：http://hz.daxiang520.top/gtagjysmew.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hongshengwenyu.top/gtzqauwzsm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.316326.xyz/gtrxthedjn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258.top/gtgipuoven.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.aibaodan.cn/gttlggdlgs.html

[J03] 字符串解析为日期
来源：http://hz.aizwys.cn/gtscpvikwx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xziqi.cn/gtwzvcnjhw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.316326.xyz/gtwtqomrvw.html

JS:   new Date("2024-01-02")
来源：http://hz.hnqzz.top/gtnwyhcout.html

TS:   new Date("2024-01-02")
来源：http://hz.aizwys.cn/gtcqeuyfuf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.52xcode.cn/gttptoxnan.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xinyue.icu/gtumvvhwdx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ehwqpu.com/gtvvfjrmxh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yuanzhike.top/gtxazeqavt.html

[J04] 时间戳与日期互转
来源：http://hz.daxiang520.top/gtsowiquop.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuxming.cn/gtzightxrj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.daria6918.cn/gtquxkuzbb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zdqjudy.top/gtuufidukh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gaohongyu789.top/gtwqbzvuld.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gaohongyu789.top/gtejolhnhn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.redwolf501.top/gtkdwdcwfb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinqigfzy.top/gtxamcjkdo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.svipenyu.cn/gtdwaxwgbm.html

[J05] 时间加减（加 7 天）
来源：http://hz.vqdsnc.cn/gthtjjokhi.html

Py:   now + timedelta(days=7)
来源：http://hz.c1oappe.top/gtztldubyo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cdnleiting.top/gtrewewgnz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuanzhike.top/gtzcwnxnui.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shzxlz.cn/gtgltikgio.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jyoumei.cn/gtjjykjuwk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.feifeiyinyue.top/gtjlozflwx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.guowangkeji.top/gtqncyxhgr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.snrcjt.cn/gtawztcfgq.html

[J06] 计算两时间之差
来源：http://hz.cqqwz.cn/gtioklsgah.html

Py:   (end - start).total_seconds()
来源：http://hz.guannengcc.top/gtomdxgxrz.html

PHP:  $end->diff($start)->days;
来源：http://hz.sweek.top/gtplowhclh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gotoacloud.top/gtllutxjaq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gzhubu.top/gtqkmkuhge.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xylfe.cn/gtcmaxwrmi.html

Go:   end.Sub(start).Hours()
来源：http://hz.ydzc1.top/gtmsgxustg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhongyouzk.top/gtmbfbpetk.html

C#:   (end - start).TotalSeconds
来源：http://hz.xingfuxueyuan.xyz/gtxzlnifqe.html

[J07] 比较两个日期
来源：http://hz.yj202588.top/gtrdygdcwd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtqlvoxldu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yueranfly.top/gtlshsazra.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yonumen.top/gtuczjtifu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhaomingkeji.xyz/gtqcfgnobv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.c1oappe.top/gtayjxlecs.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hnqzz.top/gtnztlsrpx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtgooltvmn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtdnzrxkcz.html

[J08] 提取年月日与星期
来源：http://hz.xingfuxueyuan.xyz/gtkfoxhwuu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.52xcode.cn/gttgpjgmnz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinqigufen.top/gtlpwevqbr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.316326.xyz/gtvewcctmm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jlsjyb.cn/gtkayejvzn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhongyouzk.top/gtlhawlivx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yongpay.top/gthlsodmlw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gogol.net.cn/gtdsmxhjce.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.fzhhl.top/gttoezrgxa.html

[J09] 时区处理
来源：http://hz.gotoacloud.top/gtmriekgrw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shangyingyoupin.top/gtcqlknmhe.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cheryme.top/gtmkschrgp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.redwolf501.top/gtuvevbhjn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aibaodan.cn/gtdmtykxdu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yangfankeji.com/gtdazpmabk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ydjk.org.cn/gthtkbradt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hysaishi.cn/gtwdmjsxiz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gogol.net.cn/gtdbizrmcr.html

[J10] 取今天 / 本月第一天
来源：http://hz.wangdashe.top/gtbjwjxyqi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sweek.top/gtjxosajde.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.dashuyun.cn/gtinlblepu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hywenlv.cn/gtttixxwtj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.guowangkeji.top/gtzfuibdnr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xziqi.cn/gtsccjinpx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hnqzz.top/gtzjsmsxno.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhongyouzk.top/gtuinwyquh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.wangshuangyany.cn/gtbqaludvp.html

================================================================================
来源：http://hz.guowangkeji.top/gtqyvbduro.html

K. JSON 与序列化
来源：http://hz.hongshengwenyu.top/gtdwalghlg.html

================================================================================
来源：http://hz.zhongyouzk.top/gtztursjig.html

[K01] 对象转 JSON 字符串
来源：http://hz.0kj1m.cn/gtncwvojrw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shuidangran.top/gtshpgqsoi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhijiandao.cn/gtamuivesg.html

JS:   JSON.stringify(obj)
来源：http://hz.shzxlz.cn/gtfwobdcqe.html

TS:   JSON.stringify(obj)
来源：http://hz.316326.xyz/gtbptyfdfg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tanke756.top/gtkirgjsyk.html

Go:   json.Marshal(obj)
来源：http://hz.zycfv.cn/gtqjwmcepn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.pycfn.com/gthfdryacl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sysykeji.top/gtefxofqkk.html

[K02] JSON 字符串转对象
来源：http://hz.vqdsnc.cn/gtrfsbjsgs.html

Py:   json.loads(s)
来源：http://hz.shangyingyoupin.top/gtskfhwgob.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.0kj1m.cn/gtshtzygor.html

JS:   JSON.parse(s)
来源：http://hz.yongpay.top/gtutklbylo.html

TS:   JSON.parse(s)
来源：http://hz.yvedp.cn/gtxzwsdngc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shuidangran.top/gtkjkdsgdj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ydjk.org.cn/gtsqwuukef.html

Ruby: JSON.parse(s)
来源：http://hz.haohaochexian.top/gtrjzzsugv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shanyushiyangkeji.top/gtvokldqgr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ybcxt.top/gttlazagbh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj202588.top/gtqpcyrlee.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinghuilouyu.cn/gttvwnorro.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangdashe.top/gtoqdnoosp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenlongwang.top/gtfviaogef.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hammf.cn/gtyhcofvbd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.daria6918.cn/gtsbjyxnxc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cdnleiting.top/gtkhihgeht.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gotoacloud.top/gtkzrcgwjk.html

[K04] 读取 JSON 文件
来源：http://hz.shanyushiyangkeji.top/gtiymupvre.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hnxiangtu.top/gtzluwvjiq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.andypj.xyz/gtbtptsgcs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhengqikj.top/gtdpakdjcl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangshuangyany.cn/gtjahhmznd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nanxuanxn.top/gtgxipsnve.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ywan-chungtsiang.top/gttmxepmmc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xziqi.cn/gtujyfliix.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xylfe.cn/gtmfkptnec.html

[K05] 深拷贝对象
来源：http://hz.cucudq.cn/gthpbfotaa.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxuanxn.top/gtszdxgmqq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenlongwang.top/gtdwfbxrfc.html

JS:   structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gtcwmustmf.html

TS:   structuredClone(obj)
来源：http://hz.jyoumei.cn/gtiokhzrzo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sufxvd.cn/gtcwzfhvwj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sysykeji.top/gtnerlunas.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jlsjyb.cn/gtuxzqzvau.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yonumen.top/gtbwitstic.html

[K06] 解析 URL 查询串
来源：http://hz.zhoulong.xyz/gtsjggmcgo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hfpthk.cn/gtwcadbgkb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhaomingkeji.xyz/gtbwiwpytv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pycfn.com/gtucebvcsb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtfjcqlvzl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shanyushiyangtech.top/gtlzwypqqs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.snrcjt.cn/gtuzuiabmm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cqqwz.cn/gthfjfjvre.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtmdbuhwfb.html

[K07] 进制转换
来源：http://hz.jyoumei.cn/gtzzvngbnw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xuanzx.com/gtckazbqnd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xinyue.icu/gtpfsckinj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cucudq.cn/gtluinzcbf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtlgnekjtm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtwxqmhvcn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nwbrower.top/gtcsijoejs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yongpay.top/gtxyamtyvx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jyoumei.cn/gtydrwbzqb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ywan-chungtsiang.top/gthoxelvib.html

Py:   pickle.dumps(obj)
来源：http://hz.svipenyu.cn/gtxjkbihbt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shanyushiyangkeji.top/gtbpciizpu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jqgfzy.top/gtpmfwlsci.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zdqjudy.top/gtqmhhzrno.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhijiandao.cn/gtgrqpbqdt.html

Go:   encoding/gob
来源：http://hz.vqdsnc.cn/gtgwcbjsum.html

Ruby: Marshal.dump(obj)
来源：http://hz.bjfxy.top/gtbrrcicyw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhoulong.xyz/gthfssokuw.html

================================================================================
来源：http://hz.zhongyouzk.top/gtxfcpgpjv.html

L. 网络请求
来源：http://hz.zhaomingkeji.xyz/gtephqmaap.html

================================================================================
来源：http://hz.hnqzz.top/gtqjxkekgm.html

[L01] 发送 GET 请求
来源：http://hz.jlsjyb.cn/gtzzebwckl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhengqikj.top/gtbwiacmmo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jlsjyb.cn/gtraiqrwvi.html

JS:   await fetch(url)
来源：http://hz.gogol.net.cn/gtssqnjvzs.html

TS:   await fetch(url)
来源：http://hz.nanxinkj.top/gtvdfutcql.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zycfv.cn/gtgvnqojvu.html

Go:   resp, err := http.Get(url)
来源：http://hz.hfpthk.cn/gtwhgxiokl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jlsjyb.cn/gtxenyblwf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yangfankeji.com/gteghamrja.html

[L02] 发送 POST JSON
来源：http://hz.nanxinkj.top/gtvncnmmvj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ybcxt.top/gtmyqgdzwa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ydzc1.top/gtcwlyatax.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ppjwa.cn/gtliqetbol.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shzxlz.cn/gtewqksnut.html


<!-- 参考信息 -->