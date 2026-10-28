代发 wailian999

[H07] 断言
来源：http://hz.gotoacloud.top/gtnqprpbvg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hnxiangtu.top/gthgpdklca.html

PHP:  assert($x > 0);
来源：http://hz.yuxming.cn/gtxdystbfd.html

JS:   console.assert(x > 0);
来源：http://hz.yuanzhike.top/gthmtiznaz.html

TS:   console.assert(x > 0);
来源：http://hz.yj202588.top/gthijqygra.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jianghu66.top/gtpkhylstr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.guannengcc.top/gtuxzhjqgl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shanyushiyangtech.top/gtijfusgpy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.havefunace.top/gtikzodbxb.html

[H08] 获取错误信息与堆栈
来源：http://hz.c1oappe.top/gtypgljxst.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.fengsongda.top/gtvwumevgl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinghuilouyu.cn/gtkvofffih.html

JS:   e.message;  e.stack
来源：http://hz.redwolf501.top/gtkxobblnh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cdnleiting.top/gtkpjwkbuy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jqgfzy.top/gtozvmtmep.html

Go:   err.Error()
来源：http://hz.sweek.top/gtnoicxcsl.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhongyouzk.top/gtihmxcrrr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ywan-chungtsiang.top/gtbtaqeswg.html

[H09] 带错误码的异常
来源：http://hz.smart0.xyz/gtkocnmnhw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.c1oappe.top/gthhvoyuqv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fzhhl.top/gtrpeiwfam.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yvedp.cn/gtehkmmfxi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhaomingkeji.xyz/gtzzmzeszx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenlongwang.top/gtosandinx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.guannengcc.top/gtxijhfmac.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenlongwang.top/gtcjknplcr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.mhx1999.top/gtpmxnnwme.html

[H10] 资源自动释放
来源：http://hz.birdmap.top/gtocnbqzlx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nwbrower.top/gtwmnmjqjg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gaohongyu789.top/gtytopgufv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sysykeji.top/gtrzurlmvr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gtkoddyktl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dianchejie.cn/gtsqtsceax.html

Go:   defer f.Close()
来源：http://hz.jinqigfzy.top/gtiqcjoblx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.smart0.xyz/gtqxgwjmnd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtparvvokf.html

================================================================================
来源：http://hz.birdmap.top/gtxielqznl.html

I. 正则表达式
来源：http://hz.yj202588.top/gtznyvwkjo.html

================================================================================
来源：http://hz.ehwqpu.com/gtotyixnvu.html

[I01] 判断是否匹配
来源：http://hz.shanyushiyangtech.top/gtlcydxsct.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dashuyun.cn/gtkxammrzh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinghuilouyu.cn/gtwozphfuh.html

JS:   /\d+/.test(s)
来源：http://hz.fengsongda.top/gtmgjcjcwj.html

TS:   /\d+/.test(s)
来源：http://hz.daxiang520.top/gtqhnqwudt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cheryme.top/gtdgwfyepg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cdnleiting.top/gtxxsnvwdt.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinqigufen.top/gthpmabelx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.nanxuanxn.top/gtgvzeekdk.html

[I02] 提取所有匹配
来源：http://hz.aizwys.cn/gtsxndlkdn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xingfuxueyuan.xyz/gthirxwlwf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.birdmap.top/gtofdllknj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.svipenyu.cn/gtxabzdued.html

TS:   s.match(/\d+/g)
来源：http://hz.jyoumei.cn/gtqougkxyi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hnqzz.top/gtqnckadsl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xuanzx.com/gtnlkpzecu.html

Ruby: s.scan(/\d+/)
来源：http://hz.xingfuxueyuan.xyz/gtpaxvvkfb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cqqwz.cn/gtfpzncier.html

[I03] 提取捕获分组
来源：http://hz.xinyue.icu/gtgtoovwjx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hnxiangtu.top/gthmyvbojs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.haohaochexian.top/gtpibpmmfz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tanke756.top/gturehcjrv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinqigufen.top/gtjvaghgzx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinqigfzy.top/gtzxyyidxt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shangyingyoupin.top/gtjgbmsbpz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guannengcc.top/gtdwojqstj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yongpay.top/gtlhbnhlui.html

[I04] 正则替换
来源：http://hz.shangyingyoupin.top/gtxyykbjyh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.pengpengdd.cyou/gtohzhopga.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigufen.top/gtzglulhwm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtswzvvond.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangtech.top/gtsrzcadql.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.aibaodan.cn/gtuxnqkawh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jyoumei.cn/gtutpxcccs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinqigufen.top/gtqnyxfifu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tian-w.cn/gtggdojwps.html

[I05] 按正则拆分
来源：http://hz.52xcode.cn/gtqqxvmkgl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.bjfxy.top/gtacfnqgiw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shanyushiyangtech.top/gtfzzkyrwd.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtewflxhce.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.guannengcc.top/gtlpuabbjf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shanyushiyangkeji.top/gtahrznrsx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.daxiang520.top/gtgmxwykou.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtcrdaihtc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hfpthk.cn/gtnftrbsci.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinqigufen.top/gtackbazdc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.mhx1999.top/gtrtjznfqa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shanyushiyangkeji.top/gtqpryywro.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.feifeiyinyue.top/gtbhipyjup.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ehwqpu.com/gtikbuohpe.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ydjk.org.cn/gtsanbgdxl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nanxinkj.top/gteqfgqesl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sysykeji.top/gtryycnarr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gtchjgjvmc.html

[I07] 忽略大小写与多行模式
来源：http://hz.chenjidiqi.icu/gtmefhqwer.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xziqi.cn/gteokgadau.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.haohaochexian.top/gtlcgpxnct.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xziqi.cn/gtwtedlzyj.html

TS:   /error/gim
来源：http://hz.xziqi.cn/gtpwuordxs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ydjk.org.cn/gtsqofwves.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.316326.xyz/gtmnuzdjje.html

Ruby: s.scan(/error/i)
来源：http://hz.jinqigufen.top/gtskmicnec.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yvedp.cn/gtbpzzjgmh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zdqjudy.top/gtlbnxgdpw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hongshengwenyu.top/gtwtxwexju.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jiagoushi.top/gtriqtchzk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtbvllnwfv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangshuangyany.cn/gttbsgikdj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yonumen.top/gtwmzsrikt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ivvv.top/gtlrtevlcj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.pycfn.com/gtavwjlvxh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yangfankeji.com/gtcgozenbg.html

================================================================================
来源：http://hz.fengsongda.top/gtxscofszd.html

J. 日期与时间
来源：http://hz.xziqi.cn/gtknnkwbjy.html

================================================================================
来源：http://hz.52xcode.cn/gtaozzqhoc.html

[J01] 获取当前时间
来源：http://hz.yangfankeji.com/gtkxljjipn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sxryk.cn/gtimcotfvh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhijiandao.cn/gtvcsmmalt.html

JS:   new Date();  Date.now()
来源：http://hz.xuanzx.com/gtwwnisfvw.html

TS:   new Date();  Date.now()
来源：http://hz.guannengcc.top/gtsizupaox.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tian-w.cn/gtcrfrvbyl.html

Go:   time.Now()
来源：http://hz.xuanzx.com/gtkzwqirkt.html

Ruby: Time.now
来源：http://hz.fzhhl.top/gtdfwbesmj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.aizwys.cn/gtnpeifyyo.html

[J02] 格式化输出
来源：http://hz.daria6918.cn/gtlsomhwca.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jiagoushi.top/gtrcritrmi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtkbhayvnz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.fzhhl.top/gtoknptirf.html

TS:   d.toISOString()
来源：http://hz.smart0.xyz/gtlgpstktn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ehwqpu.com/gtbahayrmw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.guowangkeji.top/gtgcjkmgng.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxuanxn.top/gtdoxzmuim.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhijiandao.cn/gtdfydnyky.html

[J03] 字符串解析为日期
来源：http://hz.xylfe.cn/gtkwkyqbkw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigfzy.top/gtsbpcvbuz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ywan-chungtsiang.top/gtqprsbknh.html

JS:   new Date("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtiixyxlim.html

TS:   new Date("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtaanlaejv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gzhubu.top/gttniroltp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ehwqpu.com/gtnwujhbql.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.wangdashe.top/gtojgggach.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.pycfn.com/gtqunhpqrf.html

[J04] 时间戳与日期互转
来源：http://hz.yueranfly.top/gthshjehor.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.aizwys.cn/gttyefpsww.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.smart0.xyz/gttipgslyd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sweek.top/gtohnoqluc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.smart0.xyz/gtszyyhidh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jiagoushi.top/gtduwawovx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ppjwa.cn/gtevpbtyir.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj20258.top/gtyzkrbskn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.smart0.xyz/gtmmbudjty.html

[J05] 时间加减（加 7 天）
来源：http://hz.ydjk.org.cn/gtqitemrmu.html

Py:   now + timedelta(days=7)
来源：http://hz.jqgfzy.top/gtlrigoqae.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hywenlv.cn/gthouegapa.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.havefunace.top/gtxfvuymea.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hammf.cn/gtvtebxpni.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pycfn.com/gtykfyvpkf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.dashuyun.cn/gtzcnbupnb.html

Ruby: Time.now + 7 * 86400
来源：http://hz.guowangkeji.top/gteolamzav.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hongshengwenyu.top/gtxkvomjjz.html

[J06] 计算两时间之差
来源：http://hz.cqqwz.cn/gtfzokrudm.html

Py:   (end - start).total_seconds()
来源：http://hz.aizwys.cn/gtuxavqnpd.html

PHP:  $end->diff($start)->days;
来源：http://hz.jyoumei.cn/gthnocdyhr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jlsjyb.cn/gtmuntpoxk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jqgufenzy.top/gtgmqkwpum.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yonumen.top/gtukkuekvs.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinghuilouyu.cn/gtnjlqxuqk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shanyushiyangtech.top/gtfahrrylo.html

C#:   (end - start).TotalSeconds
来源：http://hz.yanxiufei.cn/gtkrgjyvao.html

[J07] 比较两个日期
来源：http://hz.zhengqikj.top/gtrccackss.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtbmvpwdxl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nwbrower.top/gtfnjgpvsy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtzmzlzrjn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hammf.cn/gtdnmvusow.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.feifeiyinyue.top/gtfnxafwnt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shanyushiyangkeji.top/gtugwikuyk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtzophzrpx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtenlhswas.html

[J08] 提取年月日与星期
来源：http://hz.kuanghao11.cn/gtqrjuzpts.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ywan-chungtsiang.top/gtmkyflnjz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgfzy.top/gtvraahacj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.dianchejie.cn/gtnhtzwtsp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.0kj1m.cn/gtftujvsvy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sysykeji.top/gtwoqxemvv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinghuilouyu.cn/gtgthcupxz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.quarkkingdee.top/gtijzeetsw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.vqdsnc.cn/gttthgnymg.html

[J09] 时区处理
来源：http://hz.jqgfzy.top/gtyoljiulo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nwbrower.top/gtbhkgiiab.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.c1oappe.top/gtuqogbpsk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cqqwz.cn/gthkyrajxn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuxming.cn/gtgajkrzix.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yvedp.cn/gtkoiqpjgt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.dianchejie.cn/gtxafvwhvh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hammf.cn/gtgdtifcce.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cheryme.top/gtyvhdhrjv.html

[J10] 取今天 / 本月第一天
来源：http://hz.yuxming.cn/gtqdjmdlbl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xuanzx.com/gtoxzhzpdh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cdnleiting.top/gtaqwyqgvy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xinyue.icu/gtndaaymbt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sysykeji.top/gtshltxvzg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tianlin.xyz/gtdhxbdsnf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xingfuxueyuan.xyz/gtnbflvumv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cheryme.top/gtwttafjom.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinqigfzy.top/gtridbosmx.html

================================================================================
来源：http://hz.redwolf501.top/gtfpfyspdb.html

K. JSON 与序列化
来源：http://hz.jinqigufen.top/gtbccfozlv.html

================================================================================
来源：http://hz.jinqigufen.top/gtwpduuuqx.html

[K01] 对象转 JSON 字符串
来源：http://hz.shanyushiyangtech.top/gtcsqjxebj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.daria6918.cn/gtrnijwxul.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jiagoushi.top/gtkdhgoiag.html

JS:   JSON.stringify(obj)
来源：http://hz.zhoulong.xyz/gtuxthcstx.html

TS:   JSON.stringify(obj)
来源：http://hz.yj20258888.top/gtkgpunzxv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ppjwa.cn/gtyiduloie.html

Go:   json.Marshal(obj)
来源：http://hz.zhijiandao.cn/gtgxzkrszk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hfpthk.cn/gtdpdhttnf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jqgfzy.top/gtzrycdkny.html

[K02] JSON 字符串转对象
来源：http://hz.yongpay.top/gtrmsnyuux.html

Py:   json.loads(s)
来源：http://hz.xinyue.icu/gtmkjrhrxs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gzhubu.top/gtjwbszipq.html

JS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtwgeespsa.html

TS:   JSON.parse(s)
来源：http://hz.hfpthk.cn/gtkwlrzfrl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258.top/gtcemdagkt.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.tian-w.cn/gtibqxqqdk.html

Ruby: JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtjtvzkihr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yanxiufei.cn/gtpuiuubtz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.aizwys.cn/gtpbehexwm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnqzz.top/gtdqyzmsfs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cqqwz.cn/gtakbchgau.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.dianchejie.cn/gtzukhtuus.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gtfuvoxeyy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinyuanbaomall.cn/gtqehgaykf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jiagoushi.top/gtzconvocg.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yangfankeji.com/gtcsclzmpg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ydzc1.top/gtolmdvswv.html

[K04] 读取 JSON 文件
来源：http://hz.ppjwa.cn/gtnlfskktr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhaomingkeji.xyz/gtvmgngtbn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.quarkkingdee.top/gtsjwjorye.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gtexqprvjj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gtyiisjpqs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhengqikj.top/gttyrcjvpt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xinyue.icu/gtjzrgmwql.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shanyushiyangtech.top/gtxylecqjd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.0kj1m.cn/gtlmsjelwb.html

[K05] 深拷贝对象
来源：http://hz.zhengqikj.top/gtopwnqgit.html

Py:   copy.deepcopy(obj)
来源：http://hz.c1oappe.top/gtqadzugge.html

PHP:  unserialize(serialize($obj));
来源：http://hz.birdmap.top/gtbfhgtdmy.html

JS:   structuredClone(obj)
来源：http://hz.gogol.net.cn/gtdefpvkyx.html

TS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtvvkgiuve.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ydjk.org.cn/gtflipenir.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xziqi.cn/gtzntnqbsw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.redwolf501.top/gtokpqufyq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xylfe.cn/gtxstzfabu.html

[K06] 解析 URL 查询串
来源：http://hz.quarkkingdee.top/gtbzczmhah.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ehwqpu.com/gturwvndhb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xuetiantiany.cn/gtlisrpgwp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj202588.top/gtktmgsznd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pengpengdd.cyou/gtghmudezi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydjk.org.cn/gtahmuaeyt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dashuyun.cn/gtuncwrvis.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sxryk.cn/gtkxgecpau.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.dashuyun.cn/gtgnyifrfn.html

[K07] 进制转换
来源：http://hz.vqdsnc.cn/gthjnnlbgw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tianlin.xyz/gtncyfmxkr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.feifeiyinyue.top/gtxuxdetss.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gogol.net.cn/gtedsjfpee.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.nwbrower.top/gttpapdqgl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cashguo.top/gtaaypchqs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.redwolf501.top/gtdlnjlotg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenzaomai.com/gtbyhlkpka.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yueranfly.top/gttoaeguox.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinqigufen.top/gthvaaxtul.html

Py:   pickle.dumps(obj)
来源：http://hz.ybcxt.top/gtzjehzcpz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tanke756.top/gtnumlaicb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ppjwa.cn/gtecsjmpkz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gtmrdryepm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.svipenyu.cn/gtegmffvrc.html

Go:   encoding/gob
来源：http://hz.chenzaomai.com/gtdadewzgw.html

Ruby: Marshal.dump(obj)
来源：http://hz.fzhhl.top/gtlfjtxbmk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ybcxt.top/gtxdzphupv.html

================================================================================
来源：http://hz.snrcjt.cn/gtwsymmdwq.html

L. 网络请求
来源：http://hz.hongshengwenyu.top/gtpjmldwey.html

================================================================================
来源：http://hz.hnqzz.top/gtnbtrkpwl.html

[L01] 发送 GET 请求
来源：http://hz.hfpthk.cn/gtykwxsmei.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jyoumei.cn/gthvilpgdk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xingfuxueyuan.xyz/gtwpkzgwzt.html

JS:   await fetch(url)
来源：http://hz.sxryk.cn/gtwkvokngc.html

TS:   await fetch(url)
来源：http://hz.sxryk.cn/gttwnlafol.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.snrcjt.cn/gtfftidzow.html

Go:   resp, err := http.Get(url)
来源：http://hz.jiagoushi.top/gtdvipgcec.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sysykeji.top/gtvpnlzews.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ydjk.org.cn/gtqppjdpro.html

[L02] 发送 POST JSON
来源：http://hz.guannengcc.top/gtayezshyz.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tian-w.cn/gtytzkjjjq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sxryk.cn/gtaikjokzm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cdnleiting.top/gthsairapo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yongpay.top/gtiyvdyzik.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sysykeji.top/gturgibshq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.pengpengdd.cyou/gtqqkmhjdg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgufenzy.top/gtuujtamcg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.smart0.xyz/gtooryrkir.html


<!-- 参考信息 -->