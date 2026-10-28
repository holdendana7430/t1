代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://hz.yj20258888.top/gtvklajvay.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jyoumei.cn/gttooifukz.html

[H09] 带错误码的异常
来源：http://hz.yuanzhike.top/gtnxgvxhbq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zycfv.cn/gtlnxymkfz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.daria6918.cn/gtlewlvjcf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.dashuyun.cn/gtzacjdfdp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.svipenyu.cn/gtovpfigvg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jyoumei.cn/gtiovfyrxu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xziqi.cn/gtnobbpuhi.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xuetiantiany.cn/gtlhtyfpgu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cashguo.top/gthjuuhhfk.html

[H10] 资源自动释放
来源：http://hz.daria6918.cn/gtlbjjpolg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cdnleiting.top/gtctbkvipg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shangyingyoupin.top/gtihrvwcjl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tian-w.cn/gthihpavus.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydjk.org.cn/gtfadoutaj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dianchejie.cn/gtfnrwmqfh.html

Go:   defer f.Close()
来源：http://hz.nanxinkj.top/gteraxcszd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yanxiufei.cn/gtkgmxpqqq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gzhubu.top/gtelamdxzv.html

================================================================================
来源：http://hz.zhongyouzk.top/gtnxsskcyp.html

I. 正则表达式
来源：http://hz.0kj1m.cn/gtqwgckohe.html

================================================================================
来源：http://hz.svipenyu.cn/gtvevaqbif.html

[I01] 判断是否匹配
来源：http://hz.pycfn.com/gtcajuqfqs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.pengpengdd.cyou/gtyvnhiqri.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhiwuduotai.top/gtnldsrqvy.html

JS:   /\d+/.test(s)
来源：http://hz.pengpengdd.cyou/gtbrpfesue.html

TS:   /\d+/.test(s)
来源：http://hz.jinghuilouyu.cn/gtdojjrjtf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhaomingkeji.xyz/gtgdcxtgkk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ivvv.top/gtkqdkxqqr.html

Ruby: s.match?(/\d+/)
来源：http://hz.jqgufenzy.top/gtmcyoiozg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.nwbrower.top/gtrxjjtltg.html

[I02] 提取所有匹配
来源：http://hz.yanxiufei.cn/gtpraomscv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tianlin.xyz/gthdfwxfwu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zdqjudy.top/gtqunmdbon.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ydjk.org.cn/gtqzuyebuh.html

TS:   s.match(/\d+/g)
来源：http://hz.nwbrower.top/gtplsvyowl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.feifeiyinyue.top/gtgkbdltbj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhongyouzk.top/gtnhugjxlp.html

Ruby: s.scan(/\d+/)
来源：http://hz.ydzc1.top/gtpadmzves.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jqgufenzy.top/gtntkkzhun.html

[I03] 提取捕获分组
来源：http://hz.gaohongyu789.top/gtymmnmdbu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuxming.cn/gtyuolqigp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gaohongyu789.top/gtwbmgbncn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.mhx1999.top/gtukzqtfek.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hongshengwenyu.top/gtrbtwziki.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jlsjyb.cn/gtyanhmrne.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.daxiang520.top/gtfmvbudem.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhongyouzk.top/gtvdcppqqt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.tanke756.top/gtbdpaffex.html

[I04] 正则替换
来源：http://hz.yueranfly.top/gtojzawipp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgfzy.top/gthbritujl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinyuanbaomall.cn/gtptwjoyvf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shzxlz.cn/gtpbftvkiy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhoulong.xyz/gtchlglals.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ivvv.top/gtdfmohcfe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shanyushiyangtech.top/gteiebwpuz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.316326.xyz/gtoauexclo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sweek.top/gtbewxcuzz.html

[I05] 按正则拆分
来源：http://hz.jqgfzy.top/gtelhrxqty.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhijiandao.cn/gthzkfubei.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jianghu66.top/gtbhqopzhv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gttcqrspfp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gtxzhalenv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hnxiangtu.top/gtokxiavrx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.redwolf501.top/gtudphdvrn.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gtorzlgjed.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yj202588.top/gtjnmcnhsx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tianlin.xyz/gtzokcctwt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.wangdashe.top/gtjagptwfu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.aibaodan.cn/gtjwgrsmxu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gotoacloud.top/gtucmxblis.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydjk.org.cn/gtartflfxj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.daxiang520.top/gtwnxpnzof.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jianghu66.top/gtspzumtzu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cucudq.cn/gtugodkhzf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhengqikj.top/gtpauglugz.html

[I07] 忽略大小写与多行模式
来源：http://hz.yangfankeji.com/gtgvkrzjmf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.wangdashe.top/gtfqrtjvhj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yj202588.top/gtojbxsycm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.bjfxy.top/gtstgtxxja.html

TS:   /error/gim
来源：http://hz.shuidangran.top/gtpqjcxndi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yongpay.top/gtaavtubpu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xylfe.cn/gtvvckhenl.html

Ruby: s.scan(/error/i)
来源：http://hz.xingfuxueyuan.xyz/gtolqcscwi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jlsjyb.cn/gtsqpvefiv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hfpthk.cn/gtjqbuyvve.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jianghu66.top/gtlpqladjg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guannengcc.top/gtbddfsneo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sxryk.cn/gtltdqiila.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.birdmap.top/gtuoqcvwwx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.andypj.xyz/gtvpfclwfp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.aizwys.cn/gtuexxrcgs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenjidiqi.icu/gtosbuwvsa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gotoacloud.top/gtksiclrci.html

================================================================================
来源：http://hz.cqqwz.cn/gttjvscpzq.html

J. 日期与时间
来源：http://hz.jiagoushi.top/gtkevwmksi.html

================================================================================
来源：http://hz.0kj1m.cn/gtjmkkkduu.html

[J01] 获取当前时间
来源：http://hz.hnqzz.top/gtzzfuxmcc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xinyue.icu/gtrihqccag.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jianghu66.top/gtbkdqhyoc.html

JS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtkyiilnwe.html

TS:   new Date();  Date.now()
来源：http://hz.bjfxy.top/gtrntsasxw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhijiandao.cn/gtetraxnoo.html

Go:   time.Now()
来源：http://hz.sufxvd.cn/gtiaizjpjl.html

Ruby: Time.now
来源：http://hz.gzhubu.top/gtonmdxszf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj20258.top/gtseuumshw.html

[J02] 格式化输出
来源：http://hz.sweek.top/gtakvgeqsc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aibaodan.cn/gtsmyhahaa.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.aibaodan.cn/gtufapqyiz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cheryme.top/gtpyzvbubi.html

TS:   d.toISOString()
来源：http://hz.cqqwz.cn/gtkiogmlqt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yuanzhike.top/gtfmjgdyeo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.aibaodan.cn/gttzrhjhmk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gthksmqaox.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hfpthk.cn/gtdudyyeqk.html

[J03] 字符串解析为日期
来源：http://hz.xingfuxueyuan.xyz/gtjgpopbbg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.redwolf501.top/gtgenfxlod.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.quarkkingdee.top/gtrtgnjshe.html

JS:   new Date("2024-01-02")
来源：http://hz.birdmap.top/gtmyiszdcz.html

TS:   new Date("2024-01-02")
来源：http://hz.316326.xyz/gtcwbkxnwn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhoulong.xyz/gtwlvsvahd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtribggvvz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.andypj.xyz/gtvheomgrm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ydzc1.top/gttcmgaxim.html

[J04] 时间戳与日期互转
来源：http://hz.52xcode.cn/gtkeueowew.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenzaomai.com/gtfglgpcye.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenjidiqi.icu/gtswtiovbc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xingfuxueyuan.xyz/gtlzolsgrr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dianchejie.cn/gtynzfcrzu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gotoacloud.top/gtxujgyfpn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.c1oappe.top/gtgfombymr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hnxiangtu.top/gtaygljyem.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jqgufenzy.top/gtasnfbpet.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhoulong.xyz/gtxhrvfehu.html

Py:   now + timedelta(days=7)
来源：http://hz.yueranfly.top/gtlvaanlqs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.iojbl.cn/gtzmfdmvcc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ivvv.top/gtubixeday.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangtech.top/gtlrxuozgp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yongpay.top/gtrukevlnn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.havefunace.top/gtslyyrrbu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zycfv.cn/gtpnotvfkx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.c1oappe.top/gtschzlaky.html

[J06] 计算两时间之差
来源：http://hz.sweek.top/gtknlfthqf.html

Py:   (end - start).total_seconds()
来源：http://hz.zhoulong.xyz/gtesvflnfu.html

PHP:  $end->diff($start)->days;
来源：http://hz.tianlin.xyz/gtrqajykxp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhixingplan.top/gthtzmcqgo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.fengsongda.top/gtnbesynrp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj20258888.top/gtsqtuioed.html

Go:   end.Sub(start).Hours()
来源：http://hz.ybcxt.top/gtmhwzbigy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenzaomai.com/gtyujsjcyw.html

C#:   (end - start).TotalSeconds
来源：http://hz.hongshengwenyu.top/gtdrbivgge.html

[J07] 比较两个日期
来源：http://hz.fengsongda.top/gtagulludk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gttilquomz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj20258.top/gtbfpupfkc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.andypj.xyz/gttidlbcal.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtwuazjboz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gotoacloud.top/gtvihzncor.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sufxvd.cn/gteffzsaly.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtsdumszkp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtpaousypo.html

[J08] 提取年月日与星期
来源：http://hz.nanxuanxn.top/gtypxgklzm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xuetiantiany.cn/gtkdgwpzys.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhijiandao.cn/gtopqzaize.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xylfe.cn/gtqlkpzgvf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yonumen.top/gtdreofzul.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yueranfly.top/gtxvpdxrko.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xuanzx.com/gtkqzmnyia.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinghuilouyu.cn/gthpdnqoiy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.andypj.xyz/gtjchldyac.html

[J09] 时区处理
来源：http://hz.jianghu66.top/gtlwhqvbyz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.meibo888.top/gtonynhyxu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.mhx1999.top/gtlrcwmoeg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.haohaochexian.top/gtpbawxhbc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenjidiqi.icu/gtflwboxjc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.haohaochexian.top/gtchltfdil.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.kuanghao11.cn/gtoxvmlpsm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cqqwz.cn/gtuuduqytt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj202588.top/gtqjdbyrum.html

[J10] 取今天 / 本月第一天
来源：http://hz.snrcjt.cn/gtzmvppwwu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.birdmap.top/gtpzuldshk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinqigufen.top/gtorpeglev.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.iojbl.cn/gtbkqfhrer.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhijiandao.cn/gtarfdqajc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xinyue.icu/gtxcisczwq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jianghu66.top/gtkfghucol.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.aizwys.cn/gtdzheebcf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gotoacloud.top/gtbozbogar.html

================================================================================
来源：http://hz.ydzc1.top/gtihullxyh.html

K. JSON 与序列化
来源：http://hz.sysykeji.top/gtzsoikhaf.html

================================================================================
来源：http://hz.cdnleiting.top/gtkeuaskhn.html

[K01] 对象转 JSON 字符串
来源：http://hz.316326.xyz/gtkwqjivsv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gtgkhrydtf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtqcvebydi.html

JS:   JSON.stringify(obj)
来源：http://hz.havefunace.top/gtaxvacqty.html

TS:   JSON.stringify(obj)
来源：http://hz.yj20258888.top/gtierbxdji.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xylfe.cn/gtocybcmpj.html

Go:   json.Marshal(obj)
来源：http://hz.xylfe.cn/gtffnfoozk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj202588.top/gtspmcqsgz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hnqzz.top/gtsdowhbzz.html

[K02] JSON 字符串转对象
来源：http://hz.feifeiyinyue.top/gtbnejmrcx.html

Py:   json.loads(s)
来源：http://hz.c1oappe.top/gtfmvyorvb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.iojbl.cn/gtkmgepuit.html

JS:   JSON.parse(s)
来源：http://hz.shuidangran.top/gtjaagttan.html

TS:   JSON.parse(s)
来源：http://hz.xuanzx.com/gtstelulhd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj202588.top/gtbsutonga.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xziqi.cn/gtamuxjhgq.html

Ruby: JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtvwolugwe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tian-w.cn/gtomrsswez.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.andypj.xyz/gtyvhbocpv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hfpthk.cn/gtufldtubk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuanzhike.top/gtpwdzxzyi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xylfe.cn/gtebhvzayd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuanzhike.top/gtupjfoebm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.haohaochexian.top/gtcdrxuttm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shuidangran.top/gtzjbfznhz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.iojbl.cn/gttlxoppao.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.52xcode.cn/gtyttbeyze.html

[K04] 读取 JSON 文件
来源：http://hz.hammf.cn/gtysiytsov.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.tanke756.top/gtidbqgtax.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zycfv.cn/gtjyccwgcs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zycfv.cn/gtjnfxpirq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shzxlz.cn/gtnbklgyul.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenzaomai.com/gtitldqwaq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.havefunace.top/gtkhgplyjh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenjidiqi.icu/gtjjzoganp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhengqikj.top/gtcrhqvsxa.html

[K05] 深拷贝对象
来源：http://hz.ivvv.top/gtedzqhzgl.html

Py:   copy.deepcopy(obj)
来源：http://hz.pycfn.com/gtmqszbixc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shzxlz.cn/gtebhxccpm.html

JS:   structuredClone(obj)
来源：http://hz.meibo888.top/gtvcrgiguu.html

TS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gtlbrknphr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.guannengcc.top/gtzjeyeuxx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.0kj1m.cn/gtfmpwhgmr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.pycfn.com/gtyqrmijjs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cdnleiting.top/gtxnaxojuk.html

[K06] 解析 URL 查询串
来源：http://hz.jinyuanbaomall.cn/gthkupzxtn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zdqjudy.top/gtaalmvlwd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cucudq.cn/gtkusajgwj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gtxwjbwyfe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.snrcjt.cn/gteooxczut.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.c1oappe.top/gtnirvseec.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.52xcode.cn/gtwnimheeq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtdfhrdajh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtosvzftjw.html

[K07] 进制转换
来源：http://hz.hywenlv.cn/gtacvyruxv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tianlin.xyz/gtpwtfzvey.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gzhubu.top/gtxkrnhglc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gttzmyakvs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtmzkipvzj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtayuabsvc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hnxiangtu.top/gtydfrkghx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ydzc1.top/gthsskmwfz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hnxiangtu.top/gtsouetfbf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yuanzhike.top/gtwvjbayli.html

Py:   pickle.dumps(obj)
来源：http://hz.dianchejie.cn/gtebjqddxh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xziqi.cn/gtuzlvfnpk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtcatbolcl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hammf.cn/gtroebfoqv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.dashuyun.cn/gtzstngwdk.html

Go:   encoding/gob
来源：http://hz.bjfxy.top/gtshzcspwr.html

Ruby: Marshal.dump(obj)
来源：http://hz.c1oappe.top/gtfhpcmztf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xinyue.icu/gtnilfjxxc.html

================================================================================
来源：http://hz.daxiang520.top/gttbqwjgmp.html

L. 网络请求
来源：http://hz.bjfxy.top/gtwixcbjom.html

================================================================================
来源：http://hz.c1oappe.top/gtfoslsjhh.html

[L01] 发送 GET 请求
来源：http://hz.jyoumei.cn/gtngxweuqo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xinyue.icu/gtbgiumbcj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.kuanghao11.cn/gtheycasjl.html

JS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gtnthwkwsi.html

TS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtzyweuaed.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.tian-w.cn/gtjozgqdfa.html

Go:   resp, err := http.Get(url)
来源：http://hz.sxryk.cn/gtroyevihx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yanxiufei.cn/gtbharyggv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.feifeiyinyue.top/gtjqfdmail.html

[L02] 发送 POST JSON
来源：http://hz.jlsjyb.cn/gtjmhahvjj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgufenzy.top/gtdqygvyqj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ydzc1.top/gtaanotmwh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jiagoushi.top/gtvkvcrlai.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sweek.top/gtdaylmhbs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jlsjyb.cn/gtmlptkkqf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.mhx1999.top/gtiwywccpx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj20258888.top/gtfliprmro.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cucudq.cn/gtvglqvreo.html

[L03] 设置自定义请求头
来源：http://hz.gzhubu.top/gtkycvboqb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.9152youxi.cn/gtlbldrqmo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cqqwz.cn/gtlaqwakng.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daxiang520.top/gttncvkqon.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gtsqjzrloa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tian-w.cn/gtisxcedaz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.feifeiyinyue.top/gtoyjuvbmz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cheryme.top/gtfpjzochp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hysaishi.cn/gtasunhdnf.html

[L04] 设置超时
来源：http://hz.zhixingplan.top/gtxcadphit.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nwbrower.top/gtnurdywhp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yanxiufei.cn/gtafsxnndn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgufenzy.top/gtzamcdqfh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.9152youxi.cn/gtopbqpmce.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gzhubu.top/gtxqcyakpj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhijiandao.cn/gtfplhgwej.html


<!-- 参考信息 -->