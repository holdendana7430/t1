代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://hz.316326.xyz/gtidbwfogr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.quarkkingdee.top/gtyxqxkrxp.html

[H09] 带错误码的异常
来源：http://hz.hfpthk.cn/gtlbioffip.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenjidiqi.icu/gthrwyopyr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenzaomai.com/gtdoegajjw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.fzhhl.top/gtzvzppzvp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.aibaodan.cn/gtwczvaofl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jlsjyb.cn/gtcjtcwojt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.mhx1999.top/gtqssvwmbf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zdqjudy.top/gtveusciky.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.quarkkingdee.top/gtqmnuxswn.html

[H10] 资源自动释放
来源：http://hz.yvedp.cn/gtycamkspq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xinyue.icu/gtqhbvdpwq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.iojbl.cn/gtpjyoducq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sxryk.cn/gtungywute.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gtifbyqhwx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tian-w.cn/gtraxwjuoq.html

Go:   defer f.Close()
来源：http://hz.chenzaomai.com/gtlwknnibw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yangfankeji.com/gtbjqnabkm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.316326.xyz/gtefizafwz.html

================================================================================
来源：http://hz.redwolf501.top/gtzztlhill.html

I. 正则表达式
来源：http://hz.xingfuxueyuan.xyz/gtcbvqbxst.html

================================================================================
来源：http://hz.zhoulong.xyz/gtjihbtgeh.html

[I01] 判断是否匹配
来源：http://hz.yangfankeji.com/gtfjpufmdn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.pengpengdd.cyou/gtrpcabooc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hongshengwenyu.top/gtferjsqki.html

JS:   /\d+/.test(s)
来源：http://hz.vqdsnc.cn/gtpdllfqfe.html

TS:   /\d+/.test(s)
来源：http://hz.yueranfly.top/gtwtovfzhp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shanyushiyangkeji.top/gtcpirbtby.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yangfankeji.com/gtzpqkyeov.html

Ruby: s.match?(/\d+/)
来源：http://hz.jianghu66.top/gtepvzzfle.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.daria6918.cn/gtxuhjkuvw.html

[I02] 提取所有匹配
来源：http://hz.hongshengwenyu.top/gtjepxptxh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.aibaodan.cn/gtztlityur.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shuidangran.top/gtwouffkmi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.feifeiyinyue.top/gtuyzjejjw.html

TS:   s.match(/\d+/g)
来源：http://hz.tian-w.cn/gtmgphvntu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.iojbl.cn/gtqbymepar.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.52xcode.cn/gtxyrdvayb.html

Ruby: s.scan(/\d+/)
来源：http://hz.sxryk.cn/gtgvkvssyo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shuidangran.top/gtwpzmkpfk.html

[I03] 提取捕获分组
来源：http://hz.tian-w.cn/gtvrstvdye.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yongpay.top/gtpufaggux.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hnqzz.top/gthxmogfjr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.mhx1999.top/gtekdiwcio.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.kuanghao11.cn/gtrwdbiiau.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.9152youxi.cn/gtqstvxlus.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.havefunace.top/gtsumfbjan.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenjidiqi.icu/gtbhdgnkpo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuanzhike.top/gtxlpqedmj.html

[I04] 正则替换
来源：http://hz.hnqzz.top/gtppsoxqnk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinqigfzy.top/gtljicozxh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.smart0.xyz/gterbxjlwb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.meibo888.top/gtsteimenb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hfpthk.cn/gtwtpfmcnb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.pengpengdd.cyou/gtenbrpeou.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.vqdsnc.cn/gtxowlqrqc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.meibo888.top/gtfkrwcnhw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yj20258.top/gtwopvcgno.html

[I05] 按正则拆分
来源：http://hz.yuxming.cn/gtvxseohdp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jiagoushi.top/gtfyememhi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhijiandao.cn/gtonksijtn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtscbvbxsa.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtdfhgruzc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hfpthk.cn/gtwafemgiw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ivvv.top/gtdzvljtwl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gtczbysqqj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinyuanbaomall.cn/gtdfmycyba.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hywenlv.cn/gtplquxmrw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinqigfzy.top/gtssajybsx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.52xcode.cn/gtwxjebffv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pycfn.com/gtwtsvbxlk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ivvv.top/gtumntbtam.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yongpay.top/gtecxtgsfd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhaomingkeji.xyz/gtlsxeurkh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.andypj.xyz/gtvdkmqpxa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jqgufenzy.top/gtpxlftnpq.html

[I07] 忽略大小写与多行模式
来源：http://hz.cdnleiting.top/gtkyrsynvy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.iojbl.cn/gthlrdokqg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yj20258.top/gtjlwicmcr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.birdmap.top/gtkxxxumdj.html

TS:   /error/gim
来源：http://hz.xziqi.cn/gttzrtauqg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.quarkkingdee.top/gtinlisibz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinqigfzy.top/gtpjtggvov.html

Ruby: s.scan(/error/i)
来源：http://hz.gogol.net.cn/gtomtijlop.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yvedp.cn/gtqpacweqh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jqgfzy.top/gtyuknhpih.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.snrcjt.cn/gtcgalnrsn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhijiandao.cn/gtdzudgsgs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tanke756.top/gtaxcnwlfg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtscqrsyer.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinghuilouyu.cn/gtynrvhovi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.bjfxy.top/gtemumsjqp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.316326.xyz/gtqxzkgnav.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cucudq.cn/gtnqgheytd.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtqcyytuad.html

J. 日期与时间
来源：http://hz.jyoumei.cn/gtktezyjda.html

================================================================================
来源：http://hz.cheryme.top/gttlfofkxt.html

[J01] 获取当前时间
来源：http://hz.hnqzz.top/gtsugcmozv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.haohaochexian.top/gtkskqktzx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinqigfzy.top/gteodogtpn.html

JS:   new Date();  Date.now()
来源：http://hz.fengsongda.top/gtrlvsitlv.html

TS:   new Date();  Date.now()
来源：http://hz.ivvv.top/gtobznvphj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.c1oappe.top/gtomwzbhql.html

Go:   time.Now()
来源：http://hz.fengsongda.top/gthnmjznhb.html

Ruby: Time.now
来源：http://hz.yvedp.cn/gtqjzgttfl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangkeji.top/gtcfvbfvml.html

[J02] 格式化输出
来源：http://hz.aibaodan.cn/gtesvduvqu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.havefunace.top/gtjwfrfdfd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj20258.top/gtrgvzxdao.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yanxiufei.cn/gtdherxxli.html

TS:   d.toISOString()
来源：http://hz.hysaishi.cn/gtforwtxde.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yonumen.top/gtcogmcezv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yongpay.top/gtsfrdqrco.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtvowkyphi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ybcxt.top/gtynlumgxi.html

[J03] 字符串解析为日期
来源：http://hz.yangfankeji.com/gteptbfvmo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jyoumei.cn/gtepjmcvui.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yonumen.top/gtahstsiny.html

JS:   new Date("2024-01-02")
来源：http://hz.hnxiangtu.top/gtvaxrkaqu.html

TS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gtxowlhzam.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yuxming.cn/gtwhzjzoru.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.guowangkeji.top/gtgzfiujtf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.dashuyun.cn/gtqteyjrmy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jiagoushi.top/gtybedrifr.html

[J04] 时间戳与日期互转
来源：http://hz.daxiang520.top/gtsbdnbbvh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tian-w.cn/gtwlnkfyzz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinyuanbaomall.cn/gtheipvvjk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shuidangran.top/gtgeortihb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cucudq.cn/gtwwdyzlfh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.tianlin.xyz/gtkhddpquc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ehwqpu.com/gteqezjtnv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinyuanbaomall.cn/gtrmmgiihi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sufxvd.cn/gtwsbwjvan.html

[J05] 时间加减（加 7 天）
来源：http://hz.daxiang520.top/gtptiuczjp.html

Py:   now + timedelta(days=7)
来源：http://hz.shuidangran.top/gtflxeysjm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgufenzy.top/gtjvtsazkj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.c1oappe.top/gtkswxmnlw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gaohongyu789.top/gtvpofyjxw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tianlin.xyz/gthzfardmi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shanyushiyangkeji.top/gtysshgfko.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cashguo.top/gtnkfxnefr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.smart0.xyz/gtqmnuuoap.html

[J06] 计算两时间之差
来源：http://hz.316326.xyz/gtobjsxccy.html

Py:   (end - start).total_seconds()
来源：http://hz.jinghuilouyu.cn/gtusauekao.html

PHP:  $end->diff($start)->days;
来源：http://hz.birdmap.top/gtsdgdnvhd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.aibaodan.cn/gtqgqicbhu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.fengsongda.top/gtxeworjdt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.vqdsnc.cn/gttftdlyry.html

Go:   end.Sub(start).Hours()
来源：http://hz.sufxvd.cn/gtudinioft.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zycfv.cn/gtpnwkeepj.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhixingplan.top/gtmeqsnmog.html

[J07] 比较两个日期
来源：http://hz.jiagoushi.top/gtsyvqsvcd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtdoqojqdh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.daxiang520.top/gtfwloyhir.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhoulong.xyz/gtyhullajw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gtaaspvvgl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nwbrower.top/gthsdgjwmu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj20258.top/gtwhhkadat.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtqeoqthky.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtupwrkaut.html

[J08] 提取年月日与星期
来源：http://hz.0kj1m.cn/gtlwhpofeb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cucudq.cn/gtgvmgiply.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.chenjidiqi.icu/gtenajxekg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yuxming.cn/gtqyhesmgt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.dashuyun.cn/gthjwqipid.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.iojbl.cn/gtaxqroezc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ydjk.org.cn/gtlmpjxstw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xingfuxueyuan.xyz/gtsdlpnqax.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daria6918.cn/gtnoyjflzf.html

[J09] 时区处理
来源：http://hz.xuanzx.com/gthviqxatv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.wangdashe.top/gtqjzvipuk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xuanzx.com/gttwwpeiaa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.svipenyu.cn/gtdgzlswxk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guowangkeji.top/gtsrqatlvz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.fzhhl.top/gtymnpxxgb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.smart0.xyz/gtxbvqsysu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gotoacloud.top/gtdggekgak.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.chenlongwang.top/gtmgmglwaw.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhaomingkeji.xyz/gtarbekufg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.0kj1m.cn/gtboslqpcx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.0kj1m.cn/gtjjwhjjnm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shangyingyoupin.top/gtwqeebzwy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gzhubu.top/gtvephmsso.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ywan-chungtsiang.top/gtziczsddc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenlongwang.top/gtsinunxdq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gogol.net.cn/gtfnqdimqo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.aizwys.cn/gtrqjxxwfl.html

================================================================================
来源：http://hz.ybcxt.top/gtihjzunxt.html

K. JSON 与序列化
来源：http://hz.feifeiyinyue.top/gtpsrajpwa.html

================================================================================
来源：http://hz.nanxinkj.top/gttpboaewa.html

[K01] 对象转 JSON 字符串
来源：http://hz.zdqjudy.top/gtvwsreiqn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.kuanghao11.cn/gteecddfwc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtgcxrdqfd.html

JS:   JSON.stringify(obj)
来源：http://hz.yangfankeji.com/gttwaxenyg.html

TS:   JSON.stringify(obj)
来源：http://hz.cashguo.top/gtwkqslxer.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.52xcode.cn/gttiiufgom.html

Go:   json.Marshal(obj)
来源：http://hz.yuxming.cn/gthwyoufwi.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xziqi.cn/gtokcmdkfs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.aizwys.cn/gtouzkjjhr.html

[K02] JSON 字符串转对象
来源：http://hz.yj202588.top/gtriykeabf.html

Py:   json.loads(s)
来源：http://hz.hnxiangtu.top/gtfpglcguf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nanxinkj.top/gttsedchrx.html

JS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtwithpcfh.html

TS:   JSON.parse(s)
来源：http://hz.hnxiangtu.top/gtotxidpbi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zdqjudy.top/gtclzspwtr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtffinncda.html

Ruby: JSON.parse(s)
来源：http://hz.yj202588.top/gtfzasaqsb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jlsjyb.cn/gtzdqvnuvx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.fengsongda.top/gtaeirkqza.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinqigfzy.top/gtnqzzhiwi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zycfv.cn/gtopwcvtot.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnqzz.top/gtropcclzs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.andypj.xyz/gtxnccvfdt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zycfv.cn/gtzrsepgit.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.daxiang520.top/gtlhxkhlyb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhijiandao.cn/gtsaioswqr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.mhx1999.top/gteinqogzw.html

[K04] 读取 JSON 文件
来源：http://hz.cdnleiting.top/gtpxjemhyw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhiwuduotai.top/gtqqirjhto.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xuanzx.com/gtfvrfoqgm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.c1oappe.top/gttlvptddl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydjk.org.cn/gtzsraatan.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pengpengdd.cyou/gtyxbqeiey.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yanxiufei.cn/gtdnszbnaq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.aibaodan.cn/gtwehdczsk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ybcxt.top/gtljehqryd.html

[K05] 深拷贝对象
来源：http://hz.shanyushiyangkeji.top/gtfjkuihoh.html

Py:   copy.deepcopy(obj)
来源：http://hz.andypj.xyz/gtnfepwohj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jyoumei.cn/gtojwrtjew.html

JS:   structuredClone(obj)
来源：http://hz.jinqigufen.top/gtslmgdhet.html

TS:   structuredClone(obj)
来源：http://hz.hywenlv.cn/gtplchnbom.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hongshengwenyu.top/gteqtogtbu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.guowangkeji.top/gtsunnxjco.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.haohaochexian.top/gtmbnappos.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.9152youxi.cn/gtbhogrphr.html

[K06] 解析 URL 查询串
来源：http://hz.zhongyouzk.top/gtoowihzhj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.dianchejie.cn/gtuwnbokdg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hnxiangtu.top/gtwqppkreu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gtsyixnjqp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.meibo888.top/gtjxaunpsh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenzaomai.com/gthcdskhtx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.nwbrower.top/gtmtwnsxka.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jqgufenzy.top/gtjugywwac.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj20258888.top/gtjxenzfnk.html

[K07] 进制转换
来源：http://hz.wangshuangyany.cn/gtksrjawgx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.52xcode.cn/gtsdazsrza.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yuxming.cn/gtcgetrdxa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yonumen.top/gtcvcywfco.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj202588.top/gtbbexibvp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtmvmeqkqq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yuanzhike.top/gtlnbrlccs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shanyushiyangtech.top/gtwijcfgmw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yuanzhike.top/gttvgbuumb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgufenzy.top/gtebmxexfa.html

Py:   pickle.dumps(obj)
来源：http://hz.cucudq.cn/gtgicmjtpe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.havefunace.top/gtihwythpo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gtlcdzyzax.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.guowangkeji.top/gtioynvbkx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.pycfn.com/gtpzdhmjft.html

Go:   encoding/gob
来源：http://hz.ydzc1.top/gtsqrwfjwp.html

Ruby: Marshal.dump(obj)
来源：http://hz.meibo888.top/gtjkfodrrx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.316326.xyz/gtexarysfv.html

================================================================================
来源：http://hz.wangdashe.top/gtygcioeko.html

L. 网络请求
来源：http://hz.yuxming.cn/gtidobvzqx.html

================================================================================
来源：http://hz.mhx1999.top/gtbckucemb.html

[L01] 发送 GET 请求
来源：http://hz.xuanzx.com/gtxffbyqir.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cqqwz.cn/gtymgvzcfh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinghuilouyu.cn/gtfnzmlyrk.html

JS:   await fetch(url)
来源：http://hz.yuanzhike.top/gtpmieluww.html

TS:   await fetch(url)
来源：http://hz.ywan-chungtsiang.top/gthuepivfx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.wangdashe.top/gtzdhjgsrs.html

Go:   resp, err := http.Get(url)
来源：http://hz.xylfe.cn/gtbkphungk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jqgufenzy.top/gtunromlhd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hysaishi.cn/gtnfwqezhk.html

[L02] 发送 POST JSON
来源：http://hz.gzhubu.top/gtgccnjdop.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cashguo.top/gtzakvfgdc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.dianchejie.cn/gtqzghushq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gtqdrxkmxa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daria6918.cn/gtqinpbiik.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinghuilouyu.cn/gtkgbdfpjs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gogol.net.cn/gtwqafchoz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hammf.cn/gtlpijhuqh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shangyingyoupin.top/gtoorfpyqo.html

[L03] 设置自定义请求头
来源：http://hz.hfpthk.cn/gtfaldynmp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.smart0.xyz/gtmxwubsot.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yonumen.top/gtfpbncijk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gtbmhrfvta.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hammf.cn/gtgdobhywp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zycfv.cn/gthitvoeas.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.9152youxi.cn/gtyicbxngw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shuidangran.top/gtdmvyksgp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.daxiang520.top/gtmydumkad.html

[L04] 设置超时
来源：http://hz.ydzc1.top/gtmeqetosw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydjk.org.cn/gtwfbrmwhy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.birdmap.top/gtxosemjik.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtfhacbheu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cheryme.top/gtdeijekqh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.andypj.xyz/gtdhmxlkbp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sxryk.cn/gtlhlphfbb.html


<!-- 参考信息 -->