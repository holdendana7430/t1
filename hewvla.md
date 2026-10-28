代发 wailian999

JS:   e.message;  e.stack
来源：http://hz.hongshengwenyu.top/gtanymqldd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gotoacloud.top/gtqeboknhb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.52xcode.cn/gtlguryqwq.html

Go:   err.Error()
来源：http://hz.ywan-chungtsiang.top/gtqkxaskba.html

Ruby: e.message;  e.backtrace
来源：http://hz.daxiang520.top/gtmfwbcaws.html

C#:   e.Message;  e.StackTrace
来源：http://hz.52xcode.cn/gtougwudes.html

[H09] 带错误码的异常
来源：http://hz.cheryme.top/gtwmzeqntz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnxiangtu.top/gtlwhzxhbj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hysaishi.cn/gtwgvyccat.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj20258888.top/gtsdzlpcxd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.c1oappe.top/gtcaiuqkxy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hfpthk.cn/gtxdpbnzwe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ydjk.org.cn/gtqurkvmao.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sxryk.cn/gthfcdygcj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.vqdsnc.cn/gtzmdnpwmc.html

[H10] 资源自动释放
来源：http://hz.fzhhl.top/gtnjaaylms.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shuidangran.top/gtejmudbbu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ivvv.top/gtvrtixkjp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dashuyun.cn/gtwpwubgat.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhixingplan.top/gtdadgttsu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhaomingkeji.xyz/gtatyjnjbm.html

Go:   defer f.Close()
来源：http://hz.cucudq.cn/gtzibvdsvu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xuanzx.com/gtnmtswkda.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.iojbl.cn/gtipirckoc.html

================================================================================
来源：http://hz.yj20258888.top/gtilnhdrps.html

I. 正则表达式
来源：http://hz.ybcxt.top/gtihtlwjcn.html

================================================================================
来源：http://hz.ydzc1.top/gtldyxzryp.html

[I01] 判断是否匹配
来源：http://hz.hnxiangtu.top/gtfbayhcnk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.feifeiyinyue.top/gtjkyfxves.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigfzy.top/gtwlbyxcvu.html

JS:   /\d+/.test(s)
来源：http://hz.birdmap.top/gtwcvizckp.html

TS:   /\d+/.test(s)
来源：http://hz.52xcode.cn/gtlzaaifqs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zdqjudy.top/gtkvkgcwyq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yj20258.top/gtyjgtbarv.html

Ruby: s.match?(/\d+/)
来源：http://hz.cdnleiting.top/gtazapammq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhengqikj.top/gtkngjjyou.html

[I02] 提取所有匹配
来源：http://hz.wangshuangyany.cn/gtahqktipu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tianlin.xyz/gtmdmmeiqp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yangfankeji.com/gtchnbvlhe.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258.top/gtmejgeydu.html

TS:   s.match(/\d+/g)
来源：http://hz.yangfankeji.com/gtmivkoecc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.quarkkingdee.top/gtihrhpxmw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhongyouzk.top/gtwmddhknf.html

Ruby: s.scan(/\d+/)
来源：http://hz.shanyushiyangtech.top/gtdakyzjvr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cheryme.top/gtshvvzvgg.html

[I03] 提取捕获分组
来源：http://hz.andypj.xyz/gtzczglqdc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.fzhhl.top/gtclfsrsgs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hnxiangtu.top/gtuktgxuvq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.wangshuangyany.cn/gtdczntwfp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.316326.xyz/gtepmpqtsw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.andypj.xyz/gtkjpffjrk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ywan-chungtsiang.top/gtnuuowkja.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.52xcode.cn/gtenputypz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zycfv.cn/gtfeogjeka.html

[I04] 正则替换
来源：http://hz.dashuyun.cn/gtwrtmqyoi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hysaishi.cn/gturmjvqos.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ydjk.org.cn/gtszppymso.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtucofirrp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.smart0.xyz/gtkyhhmpjw.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.kuanghao11.cn/gtsviyxujn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tian-w.cn/gtdunkcooa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenlongwang.top/gtwxyilzmx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.feifeiyinyue.top/gttcsqzuze.html

[I05] 按正则拆分
来源：http://hz.yueranfly.top/gthaztofvs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.316326.xyz/gtcbahjmhz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhengqikj.top/gttddvlaam.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sweek.top/gtwfxqacsf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtanuxahej.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhixingplan.top/gtqpokyyho.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinyuanbaomall.cn/gthnlfmtss.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtkzfohefk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.nanxuanxn.top/gtznxbltur.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.316326.xyz/gtfqcayqix.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yvedp.cn/gtkyokhpkb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hammf.cn/gtutdnoolg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgfzy.top/gtcwumryvq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtxclmyxzi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenlongwang.top/gtxnajxqqt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.c1oappe.top/gtmgtilvdn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.pengpengdd.cyou/gtjldkzypq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhiwuduotai.top/gttztgrebx.html

[I07] 忽略大小写与多行模式
来源：http://hz.jqgufenzy.top/gtwioqtrmq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zycfv.cn/gtghwiflas.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhoulong.xyz/gtjakqciao.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ehwqpu.com/gtubtlkajr.html

TS:   /error/gim
来源：http://hz.yangfankeji.com/gtrwuvzsfh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sysykeji.top/gtjeilthsu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.daria6918.cn/gtkwoyshnn.html

Ruby: s.scan(/error/i)
来源：http://hz.quarkkingdee.top/gtxkcuyydj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cdnleiting.top/gtpgylwigx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhixingplan.top/gtuueoayxc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sufxvd.cn/gthxdwgzyj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.bjfxy.top/gtnqimkuqm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cashguo.top/gtepzqzlor.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xylfe.cn/gtqqyubhng.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ppjwa.cn/gtuyznywzc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jianghu66.top/gtqrftuizq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.smart0.xyz/gtflriprib.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daxiang520.top/gtklvecfod.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtcyelvlel.html

J. 日期与时间
来源：http://hz.hnqzz.top/gtpophqauy.html

================================================================================
来源：http://hz.jiagoushi.top/gtmxeinqec.html

[J01] 获取当前时间
来源：http://hz.aibaodan.cn/gtbewnquvb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hammf.cn/gtazmssozp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenzaomai.com/gtkzdvppyg.html

JS:   new Date();  Date.now()
来源：http://hz.tian-w.cn/gtrhjanqnz.html

TS:   new Date();  Date.now()
来源：http://hz.yj20258.top/gtubnlmrxa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.svipenyu.cn/gtybafqrsy.html

Go:   time.Now()
来源：http://hz.yvedp.cn/gtbgqlywms.html

Ruby: Time.now
来源：http://hz.svipenyu.cn/gtmodntovd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sxryk.cn/gtqhhffbda.html

[J02] 格式化输出
来源：http://hz.yj20258888.top/gtrzznuxfv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yueranfly.top/gtmjaozbxg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hongshengwenyu.top/gtftifeoth.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.haohaochexian.top/gtcomywgbg.html

TS:   d.toISOString()
来源：http://hz.0kj1m.cn/gtoxiyuolx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hammf.cn/gtquhjqtss.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.vqdsnc.cn/gtkmlaucsk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangtech.top/gtauxqpkmg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yuxming.cn/gtjhirapxz.html

[J03] 字符串解析为日期
来源：http://hz.yuxming.cn/gtddfwtgqu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gogol.net.cn/gtsxtkpmkl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhiwuduotai.top/gtimvvozvd.html

JS:   new Date("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtipjkqzbs.html

TS:   new Date("2024-01-02")
来源：http://hz.gaohongyu789.top/gtdubwoauu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guannengcc.top/gthfhbpuie.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhiwuduotai.top/gtcmoemdkn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenlongwang.top/gtypjxmapb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yanxiufei.cn/gteemyblca.html

[J04] 时间戳与日期互转
来源：http://hz.havefunace.top/gtkjzeipeu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258888.top/gtcrpadqvl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jlsjyb.cn/gtrcxydcdv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.havefunace.top/gtosndfcyq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhiwuduotai.top/gteprtswhd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.chenlongwang.top/gtlmoiarta.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.redwolf501.top/gtulhqrlpg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xuetiantiany.cn/gtfuabwlvy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yueranfly.top/gtcipauxnq.html

[J05] 时间加减（加 7 天）
来源：http://hz.pengpengdd.cyou/gtgpflxxgp.html

Py:   now + timedelta(days=7)
来源：http://hz.cucudq.cn/gtqcmqzzcw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhixingplan.top/gtoqqllcgg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtpybxyvey.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtykvcadic.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj202588.top/gtcaypsmxn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.vqdsnc.cn/gtcwjzjxxm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.wangdashe.top/gtxyvnlkwq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cdnleiting.top/gtyeufkdxh.html

[J06] 计算两时间之差
来源：http://hz.jiagoushi.top/gtgtycnhbt.html

Py:   (end - start).total_seconds()
来源：http://hz.vqdsnc.cn/gttvpubzol.html

PHP:  $end->diff($start)->days;
来源：http://hz.dianchejie.cn/gtiwzyiewm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.redwolf501.top/gtyyivowbf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yongpay.top/gtntqqibdt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xinyue.icu/gtfgwvimdr.html

Go:   end.Sub(start).Hours()
来源：http://hz.yuxming.cn/gtqfxldlvt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ybcxt.top/gtpgemwupe.html

C#:   (end - start).TotalSeconds
来源：http://hz.yj20258.top/gtrfkiytoe.html

[J07] 比较两个日期
来源：http://hz.hysaishi.cn/gtcoyyjwjz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtsnjvhlgx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shanyushiyangkeji.top/gtokbjviul.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guannengcc.top/gthfxgpxni.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.316326.xyz/gtyggzzhjn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tianlin.xyz/gteapswbfo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.dashuyun.cn/gtvwipjnwl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yvedp.cn/gtytmqkjqm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtlcudvtwa.html

[J08] 提取年月日与星期
来源：http://hz.nwbrower.top/gtubbxheja.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhoulong.xyz/gtzubkvbsl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xziqi.cn/gtbpcmtote.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nanxinkj.top/gtjoxmtlif.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yvedp.cn/gtwkcekzct.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.aibaodan.cn/gtgehazdma.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ydjk.org.cn/gtljngnvgc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sysykeji.top/gtqigdxack.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jqgfzy.top/gtasmwpugm.html

[J09] 时区处理
来源：http://hz.chenzaomai.com/gthhifseji.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ybcxt.top/gtffysnxss.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.dashuyun.cn/gtfcxozdgi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gtslkjngsa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daria6918.cn/gtzflufgeb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxuanxn.top/gtwdpkhjcz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.havefunace.top/gtevcnakkt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj20258.top/gtthbbxnxp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.52xcode.cn/gtukuzaifu.html

[J10] 取今天 / 本月第一天
来源：http://hz.birdmap.top/gtlkynjkjz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.c1oappe.top/gtagqrnfzu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hfpthk.cn/gtqctgqunq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.wangshuangyany.cn/gtwbrtwmus.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj202588.top/gtrkylfbmn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hnqzz.top/gtysftugfu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.dashuyun.cn/gtfarptrtt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hfpthk.cn/gtrtrtgpam.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yanxiufei.cn/gtiejsskzh.html

================================================================================
来源：http://hz.hfpthk.cn/gtchkkuplq.html

K. JSON 与序列化
来源：http://hz.jyoumei.cn/gtidcnndrq.html

================================================================================
来源：http://hz.sysykeji.top/gtczezpfgv.html

[K01] 对象转 JSON 字符串
来源：http://hz.tanke756.top/gtwteyjjdt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tian-w.cn/gtqcccqivd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zycfv.cn/gtxlmbsqbi.html

JS:   JSON.stringify(obj)
来源：http://hz.cheryme.top/gtiuvjigss.html

TS:   JSON.stringify(obj)
来源：http://hz.quarkkingdee.top/gthjdqqgbd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yanxiufei.cn/gtmoxkwcfi.html

Go:   json.Marshal(obj)
来源：http://hz.hywenlv.cn/gtansnabyq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.kuanghao11.cn/gtiuuqkrxg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.birdmap.top/gtadakukhl.html

[K02] JSON 字符串转对象
来源：http://hz.aizwys.cn/gtxkztdhqv.html

Py:   json.loads(s)
来源：http://hz.zhijiandao.cn/gtfuptadwr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.aibaodan.cn/gtuxndhaxn.html

JS:   JSON.parse(s)
来源：http://hz.c1oappe.top/gtvtzppzde.html

TS:   JSON.parse(s)
来源：http://hz.0kj1m.cn/gtszfgsjti.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xinyue.icu/gtdjtptdop.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtpqwzctlq.html

Ruby: JSON.parse(s)
来源：http://hz.cdnleiting.top/gtxtvuamro.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhijiandao.cn/gtdqjamhpe.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.mhx1999.top/gtuzoeinfh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.redwolf501.top/gtpysatlie.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.pycfn.com/gtrbhouiar.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gaohongyu789.top/gtaxitjgat.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnxiangtu.top/gtguhozacb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.mhx1999.top/gtmalabwhr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ydjk.org.cn/gthlmopjth.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xinyue.icu/gtiiywjknk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sxryk.cn/gtbrskcxnu.html

[K04] 读取 JSON 文件
来源：http://hz.jianghu66.top/gtrvalgoga.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xinyue.icu/gtjelgrbnj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tanke756.top/gtdzhbqmer.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sysykeji.top/gttvcmcixb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.haohaochexian.top/gtysyvoewk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nwbrower.top/gtludgsaxc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtfhyyynyh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yueranfly.top/gtxujgrgom.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shuidangran.top/gtlugkeseu.html

[K05] 深拷贝对象
来源：http://hz.c1oappe.top/gtfpnkjsta.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydzc1.top/gtcbzhwoca.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhijiandao.cn/gtypntjunz.html

JS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtcpdxyocn.html

TS:   structuredClone(obj)
来源：http://hz.wangdashe.top/gtzpqdprck.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hfpthk.cn/gtwpbuiwwq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhongyouzk.top/gtpevlqzvz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hammf.cn/gtaolarrvd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.kuanghao11.cn/gtwvdycyzt.html

[K06] 解析 URL 查询串
来源：http://hz.sysykeji.top/gtgcyszqhj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenzaomai.com/gtrnavxxzp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.0kj1m.cn/gtsxbouiiz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gtkozmmqyu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hfpthk.cn/gttfwlrxoj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenlongwang.top/gtdxsycjit.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.nwbrower.top/gtsxqegjvz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.birdmap.top/gttpgmmjbc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenlongwang.top/gtqskwufmp.html

[K07] 进制转换
来源：http://hz.havefunace.top/gtnornfvxg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.pengpengdd.cyou/gtqizcskbr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tanke756.top/gtvdwxhdyb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtqvczkssu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtaatagdnk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sweek.top/gtwkwnoxao.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shuidangran.top/gthqjxtczr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.havefunace.top/gtpvihyihp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sweek.top/gteiifqruw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.svipenyu.cn/gtnlkisucq.html

Py:   pickle.dumps(obj)
来源：http://hz.zhongyouzk.top/gtvdrwykcl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.316326.xyz/gtxbzmdaar.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cqqwz.cn/gtgeeoccam.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhoulong.xyz/gtkaouplqs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yonumen.top/gtorqyztht.html

Go:   encoding/gob
来源：http://hz.c1oappe.top/gtvczebhyy.html

Ruby: Marshal.dump(obj)
来源：http://hz.tianlin.xyz/gtsfaghwmm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hnqzz.top/gtnvmyzrbk.html

================================================================================
来源：http://hz.9152youxi.cn/gtmymmhhqg.html

L. 网络请求
来源：http://hz.hnxiangtu.top/gtlynitpio.html

================================================================================
来源：http://hz.yangfankeji.com/gtshixkfik.html

[L01] 发送 GET 请求
来源：http://hz.xingfuxueyuan.xyz/gtgnbueusn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nanxinkj.top/gtuwvhisnx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yongpay.top/gtlefzlqaw.html

JS:   await fetch(url)
来源：http://hz.ybcxt.top/gtfkzceakq.html

TS:   await fetch(url)
来源：http://hz.hysaishi.cn/gtxgvrdqwe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.kuanghao11.cn/gtlisajpfw.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhengqikj.top/gtlavjiwif.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yuanzhike.top/gtkfunnhwb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhoulong.xyz/gtssbighlr.html

[L02] 发送 POST JSON
来源：http://hz.jyoumei.cn/gtcsocnouo.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenlongwang.top/gtpeqwgwsp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shanyushiyangtech.top/gtsftlfttx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sxryk.cn/gtkxiaduvc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gthudamjnk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenjidiqi.icu/gtzktxofgz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ywan-chungtsiang.top/gtqahnamip.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zdqjudy.top/gtssddrypo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yonumen.top/gthwhxrrwa.html

[L03] 设置自定义请求头
来源：http://hz.smart0.xyz/gtbxikzyna.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yonumen.top/gtbzxfqvbk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shangyingyoupin.top/gtkhgelsuj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zycfv.cn/gtggfpkkrv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fzhhl.top/gtudpxsxyy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sysykeji.top/gtlkacyrgw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.dashuyun.cn/gtpntychdw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cdnleiting.top/gtetcobrtw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.mhx1999.top/gthemznufu.html

[L04] 设置超时
来源：http://hz.xinyue.icu/gtkszyhcew.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xuanzx.com/gtkkysxcdq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jlsjyb.cn/gtdhixfuqf.html


<!-- 参考信息 -->