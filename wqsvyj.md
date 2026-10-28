代发 wailian999

JS:   e.message;  e.stack
来源：http://hz.xziqi.cn/gttyyjsays.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hnqzz.top/gtrbunqbyj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.bjfxy.top/gthzfaztdv.html

Go:   err.Error()
来源：http://hz.hfpthk.cn/gteauuzihw.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinqigufen.top/gtaexnicqc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jqgfzy.top/gtaekdpeos.html

[H09] 带错误码的异常
来源：http://hz.316326.xyz/gtxfustiml.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yuxming.cn/gtbruhsdsh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sweek.top/gtolohcieo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xylfe.cn/gtffgsqllb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xuetiantiany.cn/gtwdohhpay.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yongpay.top/gtlxmxkzzs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xingfuxueyuan.xyz/gtjhhhwfqc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.bjfxy.top/gtcttlcmam.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yj202588.top/gtctqatyxu.html

[H10] 资源自动释放
来源：http://hz.jinghuilouyu.cn/gtipicxlev.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jlsjyb.cn/gtmipcjxwm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zycfv.cn/gtwfstkrzj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.feifeiyinyue.top/gtqbhijwof.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhijiandao.cn/gtjnxsbiju.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ppjwa.cn/gttowcelyj.html

Go:   defer f.Close()
来源：http://hz.jinghuilouyu.cn/gtdkugtihm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.0kj1m.cn/gtofblzuwx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hongshengwenyu.top/gtxikxchga.html

================================================================================
来源：http://hz.gzhubu.top/gtjhvljjxh.html

I. 正则表达式
来源：http://hz.shzxlz.cn/gtpimlzwpj.html

================================================================================
来源：http://hz.tian-w.cn/gtkwxpgyhs.html

[I01] 判断是否匹配
来源：http://hz.jqgufenzy.top/gtrovkkexf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtrzlovfdb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.wangshuangyany.cn/gtpfzbpfdv.html

JS:   /\d+/.test(s)
来源：http://hz.nanxinkj.top/gtcdwtexqi.html

TS:   /\d+/.test(s)
来源：http://hz.tian-w.cn/gtxzzgjibd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jlsjyb.cn/gtavdufjmr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gaohongyu789.top/gtoojffgps.html

Ruby: s.match?(/\d+/)
来源：http://hz.tian-w.cn/gtzkfagwpy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinghuilouyu.cn/gtkhnofvvi.html

[I02] 提取所有匹配
来源：http://hz.sxryk.cn/gtrctcwslx.html

Py:   re.findall(r"\d+", s)
来源：http://hz.chenzaomai.com/gtzoamunjy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yonumen.top/gtpfnvhgqc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.wangdashe.top/gtoixomagu.html

TS:   s.match(/\d+/g)
来源：http://hz.xinyue.icu/gtkdjsujgx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xuanzx.com/gtmqhlmxwq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinqigfzy.top/gtfgthzbqx.html

Ruby: s.scan(/\d+/)
来源：http://hz.sxryk.cn/gtxmawdwvx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.aibaodan.cn/gtqifbmudz.html

[I03] 提取捕获分组
来源：http://hz.hnxiangtu.top/gtmtkhsuqh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.svipenyu.cn/gtqntxyfcn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shangyingyoupin.top/gtjydfhrfg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ivvv.top/gtiyohkixi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhiwuduotai.top/gtrgizetuz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shanyushiyangkeji.top/gtrugrbzat.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxinkj.top/gtjfdbogda.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.andypj.xyz/gtsquqhhho.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sxryk.cn/gtqcqbwbkn.html

[I04] 正则替换
来源：http://hz.bjfxy.top/gtubxyrtsd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jyoumei.cn/gtgivwvhpy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jyoumei.cn/gtwxitywud.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xingfuxueyuan.xyz/gthzwqqhet.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ywan-chungtsiang.top/gtgpaejhgi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sufxvd.cn/gtuutqqzzn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.pengpengdd.cyou/gtbrbxliay.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ybcxt.top/gtylvylvsg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.mhx1999.top/gtsgrjyqxg.html

[I05] 按正则拆分
来源：http://hz.ybcxt.top/gteihgovxv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zdqjudy.top/gtbsjcjpnu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cashguo.top/gteekpueyl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtdoafmxqb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nanxinkj.top/gtrvoesjft.html

Java: s.split("\\s*,\\s*")
来源：http://hz.kuanghao11.cn/gtmzobrxen.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sufxvd.cn/gtpcgapoci.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtwtgnsfcj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ivvv.top/gtohwaqmlg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jianghu66.top/gtavkuxywl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cheryme.top/gtsaycnqep.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.snrcjt.cn/gtbunerrnj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yonumen.top/gtaggxczvq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zdqjudy.top/gtyjpgizgo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yongpay.top/gtmppfqyxy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.bjfxy.top/gtwyghnsjw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hammf.cn/gtslzdmwmc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yanxiufei.cn/gtljmqgizr.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj202588.top/gtfkvqhdoi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ehwqpu.com/gtkhgfcvuq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.vqdsnc.cn/gtwgnjnfux.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.haohaochexian.top/gtamejlrni.html

TS:   /error/gim
来源：http://hz.chenzaomai.com/gtjlnwtpou.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tianlin.xyz/gtrfsyhwim.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.0kj1m.cn/gtfglyaagd.html

Ruby: s.scan(/error/i)
来源：http://hz.cashguo.top/gtgmnvatlr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sufxvd.cn/gtrlngovie.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.tianlin.xyz/gtgflszkyl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gaohongyu789.top/gtikwriqwv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.wangdashe.top/gtebgzxsyo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gtvwigivbt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhoulong.xyz/gtpryfvmbd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.aibaodan.cn/gtuwzhxffd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.feifeiyinyue.top/gtyosxqocb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinyuanbaomall.cn/gtxbzpmxfb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.havefunace.top/gtrlxjruhf.html

================================================================================
来源：http://hz.andypj.xyz/gtotftwopy.html

J. 日期与时间
来源：http://hz.zhiwuduotai.top/gtziiigadf.html

================================================================================
来源：http://hz.ehwqpu.com/gtuxxmgstw.html

[J01] 获取当前时间
来源：http://hz.yangfankeji.com/gttwgpyihu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.tanke756.top/gtdcyneagr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gaohongyu789.top/gteiimqwwu.html

JS:   new Date();  Date.now()
来源：http://hz.nwbrower.top/gtoxvixqvs.html

TS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gtymyursub.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cqqwz.cn/gtztknqmil.html

Go:   time.Now()
来源：http://hz.wangdashe.top/gtszxdfigm.html

Ruby: Time.now
来源：http://hz.xylfe.cn/gtssllmotu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhiwuduotai.top/gtbcooekdt.html

[J02] 格式化输出
来源：http://hz.yj20258.top/gtetgldkzr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tianlin.xyz/gtdvwkdydp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hnxiangtu.top/gtswautjwq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xinyue.icu/gtiiqzcgop.html

TS:   d.toISOString()
来源：http://hz.shzxlz.cn/gtuoiqnpzo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.quarkkingdee.top/gtwomgbndb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.snrcjt.cn/gtzkgwsoeu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cucudq.cn/gthuyuyjat.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cucudq.cn/gtwlyuwgeu.html

[J03] 字符串解析为日期
来源：http://hz.jinqigufen.top/gtktgblrki.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shanyushiyangtech.top/gtfpvcuond.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.bjfxy.top/gtujtxgren.html

JS:   new Date("2024-01-02")
来源：http://hz.jqgfzy.top/gtthrebfpf.html

TS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtrsvymjdg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tian-w.cn/gtfpcwxnaj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yanxiufei.cn/gtesqzppnn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jyoumei.cn/gtmywrfusz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.meibo888.top/gtfyiqazac.html

[J04] 时间戳与日期互转
来源：http://hz.yuanzhike.top/gttmvjpngh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jianghu66.top/gtfxsumjju.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gzhubu.top/gtuiyeomyb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.52xcode.cn/gtfyiuhzpu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jqgufenzy.top/gthpaiojsb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yvedp.cn/gticzzpxhd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tianlin.xyz/gtnuhdcolc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinqigufen.top/gtfxufzhfl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.daxiang520.top/gtoxchkhoi.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj20258.top/gtlsddhqps.html

Py:   now + timedelta(days=7)
来源：http://hz.jqgfzy.top/gtetcjegvk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.316326.xyz/gtarmgvqfh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gtyupqgucn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinghuilouyu.cn/gtwdqyuhda.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xinyue.icu/gtapiosqaf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jyoumei.cn/gtwlorihye.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jlsjyb.cn/gtrfnkjhsk.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ehwqpu.com/gtkustodcf.html

[J06] 计算两时间之差
来源：http://hz.zhixingplan.top/gthfevuzew.html

Py:   (end - start).total_seconds()
来源：http://hz.sysykeji.top/gtctrkmwpo.html

PHP:  $end->diff($start)->days;
来源：http://hz.zdqjudy.top/gtaikfsdra.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.svipenyu.cn/gtzcjaamnf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.52xcode.cn/gtjbsjmqws.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ydjk.org.cn/gtoulnyksb.html

Go:   end.Sub(start).Hours()
来源：http://hz.316326.xyz/gtjipesuxe.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinqigfzy.top/gtoycgjkwx.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhixingplan.top/gtgibduzen.html

[J07] 比较两个日期
来源：http://hz.haohaochexian.top/gtpahlhead.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtzserpqat.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.mhx1999.top/gtvrlzgcsn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtzjjozzzu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ehwqpu.com/gtbruocnja.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cdnleiting.top/gtstpftfdg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shanyushiyangtech.top/gtdltusmpg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtzbzcojbq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtdtlcansi.html

[J08] 提取年月日与星期
来源：http://hz.jianghu66.top/gthnvgufbq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.tanke756.top/gtxwhlthkh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258.top/gtbmbgwtpv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aizwys.cn/gtpoldsfls.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yanxiufei.cn/gtsogwyxyc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ydjk.org.cn/gtevnckoic.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shuidangran.top/gtzevcifza.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cheryme.top/gtaikcvwes.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yueranfly.top/gtwkfccyay.html

[J09] 时区处理
来源：http://hz.sxryk.cn/gtpursiqty.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jianghu66.top/gtnmfuhbfj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.guannengcc.top/gtsrhhbmwp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtkjrjzwub.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aizwys.cn/gtgrexbjmk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hongshengwenyu.top/gtzczcamck.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.havefunace.top/gtpwhmafyd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yuxming.cn/gtamcaeuxj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.aizwys.cn/gtaoigmrbf.html

[J10] 取今天 / 本月第一天
来源：http://hz.0kj1m.cn/gtlbymxyvv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tian-w.cn/gtasjzxaan.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj20258.top/gtfxkrdwpv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.fzhhl.top/gttgrifoov.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenjidiqi.icu/gtsoodfbbw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.52xcode.cn/gtshtuocon.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.c1oappe.top/gtfqxxzkev.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shzxlz.cn/gtmgjkkeyc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.0kj1m.cn/gtxftbmlqv.html

================================================================================
来源：http://hz.cheryme.top/gtgahrtvtn.html

K. JSON 与序列化
来源：http://hz.zdqjudy.top/gtzhgyoeru.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtzzjsdejl.html

[K01] 对象转 JSON 字符串
来源：http://hz.cheryme.top/gtgnmhepsq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shzxlz.cn/gtnyvytvdl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.fzhhl.top/gtjshbscgm.html

JS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gtiiyfuvbh.html

TS:   JSON.stringify(obj)
来源：http://hz.yuanzhike.top/gtdkoihles.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.9152youxi.cn/gtsnewqkbr.html

Go:   json.Marshal(obj)
来源：http://hz.zhoulong.xyz/gtarzqfhsi.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hammf.cn/gthjudouwy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigfzy.top/gtgtvumfbi.html

[K02] JSON 字符串转对象
来源：http://hz.cqqwz.cn/gtgahehhaw.html

Py:   json.loads(s)
来源：http://hz.chenzaomai.com/gtygusuacl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.52xcode.cn/gtscwcdfde.html

JS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtyxfyfila.html

TS:   JSON.parse(s)
来源：http://hz.wangdashe.top/gteimfkbqp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhaomingkeji.xyz/gtmbmlqcis.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtrkudqyzw.html

Ruby: JSON.parse(s)
来源：http://hz.gogol.net.cn/gtrxskddad.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigufen.top/gttpflmukn.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yj20258.top/gtpytzteys.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj20258888.top/gttdbikank.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.pycfn.com/gtgpzwvkge.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.smart0.xyz/gtmbltcrno.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxuanxn.top/gtypjhpimi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jianghu66.top/gtrbesjkkm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.feifeiyinyue.top/gtbqyksbep.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnxiangtu.top/gtwfnidcle.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhoulong.xyz/gtummqngsc.html

[K04] 读取 JSON 文件
来源：http://hz.guowangkeji.top/gtlcqyrehl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ehwqpu.com/gtlyrrtgfj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ywan-chungtsiang.top/gtgimlmrhe.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gtcxfxcofa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.9152youxi.cn/gtyyhkgtkj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.daxiang520.top/gtpzkboxpu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.mhx1999.top/gtofmlnxol.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.9152youxi.cn/gttmaawwvu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cucudq.cn/gtzeefezuf.html

[K05] 深拷贝对象
来源：http://hz.zdqjudy.top/gtbpofvogh.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhiwuduotai.top/gtiwrpiwle.html

PHP:  unserialize(serialize($obj));
来源：http://hz.52xcode.cn/gtqxxplvfx.html

JS:   structuredClone(obj)
来源：http://hz.sufxvd.cn/gtuclrfpyc.html

TS:   structuredClone(obj)
来源：http://hz.yonumen.top/gtizjtpfxr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yueranfly.top/gtihijryuh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.daxiang520.top/gtumjgodec.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fengsongda.top/gtfqszvwwl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nanxuanxn.top/gtyjqwhyjx.html

[K06] 解析 URL 查询串
来源：http://hz.zycfv.cn/gtyvchymtp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tanke756.top/gttroaskdc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.9152youxi.cn/gthmmreuia.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yonumen.top/gtanatakce.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258.top/gtbbfygaal.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhoulong.xyz/gtyskutydy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sufxvd.cn/gtfuwqdqtr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.0kj1m.cn/gtdrvhsxwu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.52xcode.cn/gtmrmdefjm.html

[K07] 进制转换
来源：http://hz.daria6918.cn/gtagfbfhgk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gzhubu.top/gtwgbyuuge.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hywenlv.cn/gtjvzxkusy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtxhrvnwim.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtztndigmb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tian-w.cn/gterkktbkq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.chenlongwang.top/gtjqqndwjh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.quarkkingdee.top/gtstuyukoo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.daria6918.cn/gtfnxzngki.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xuanzx.com/gthzuuhvgb.html

Py:   pickle.dumps(obj)
来源：http://hz.hongshengwenyu.top/gtryerzctj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hnqzz.top/gtxftpoyfz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.snrcjt.cn/gtuxwvmcex.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gaohongyu789.top/gtufiopgst.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gtzbqrcmrc.html

Go:   encoding/gob
来源：http://hz.ywan-chungtsiang.top/gtzzrbowpe.html

Ruby: Marshal.dump(obj)
来源：http://hz.andypj.xyz/gtjqrphrca.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gotoacloud.top/gtjuspkyux.html

================================================================================
来源：http://hz.xuanzx.com/gtmhcmyspi.html

L. 网络请求
来源：http://hz.gogol.net.cn/gtzckzetdt.html

================================================================================
来源：http://hz.havefunace.top/gtslsbsree.html

[L01] 发送 GET 请求
来源：http://hz.wangdashe.top/gtyozhwwny.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.haohaochexian.top/gtwzylskyk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.andypj.xyz/gtysginpxb.html

JS:   await fetch(url)
来源：http://hz.feifeiyinyue.top/gtsmtuebca.html

TS:   await fetch(url)
来源：http://hz.yj20258888.top/gtfdelqyzh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ybcxt.top/gtxrobitfw.html

Go:   resp, err := http.Get(url)
来源：http://hz.hfpthk.cn/gtkthbbsuu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zdqjudy.top/gtqofihsbi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jiagoushi.top/gtwwmmbgdb.html

[L02] 发送 POST JSON
来源：http://hz.jianghu66.top/gtntgorgnr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jiagoushi.top/gtowmkysmo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yvedp.cn/gtfoubtouz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.316326.xyz/gtnpgxgzzq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hysaishi.cn/gtbkjnudud.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.wangshuangyany.cn/gteliubref.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.bjfxy.top/gteevurehw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shangyingyoupin.top/gtsmvfszoq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.52xcode.cn/gtvqvazdkb.html

[L03] 设置自定义请求头
来源：http://hz.mhx1999.top/gtosarnsuu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhixingplan.top/gtsglbjffs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.vqdsnc.cn/gtojdiqllm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtaloonijf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hongshengwenyu.top/gtdanyegqg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yonumen.top/gtwnxlzajb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gaohongyu789.top/gtcewnxflg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yuxming.cn/gtchjaptfd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tianlin.xyz/gtentauqfv.html

[L04] 设置超时
来源：http://hz.yuxming.cn/gtnaxdriah.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gaohongyu789.top/gtzhwmanel.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.fengsongda.top/gtleazjncd.html


<!-- 参考信息 -->