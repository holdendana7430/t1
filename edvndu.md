代发 wailian999

JS:   e.message;  e.stack
来源：http://hz.zhaomingkeji.xyz/gtyalpbikl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj202588.top/gtcaexhjep.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zdqjudy.top/gtvnibnqbp.html

Go:   err.Error()
来源：http://hz.xuetiantiany.cn/gttirmdixa.html

Ruby: e.message;  e.backtrace
来源：http://hz.jiagoushi.top/gthjrenfgn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tanke756.top/gtkkzvsgas.html

[H09] 带错误码的异常
来源：http://hz.jinqigufen.top/gtmiwhvfvo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ehwqpu.com/gtxajklruh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.iojbl.cn/gtaryjtmqg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.birdmap.top/gttsqjgrpg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.snrcjt.cn/gtspvdjozq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jqgufenzy.top/gtqrclcvqc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhoulong.xyz/gtprwxaurl.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenjidiqi.icu/gthehmgjuj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yongpay.top/gtjizjcwbp.html

[H10] 资源自动释放
来源：http://hz.yanxiufei.cn/gtmtdecsvk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jianghu66.top/gtvbyrqacc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zdqjudy.top/gtlegvhaem.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shuidangran.top/gtzuwtgvxo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cucudq.cn/gtyxrarhyk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.daxiang520.top/gtfaghjzhj.html

Go:   defer f.Close()
来源：http://hz.redwolf501.top/gtqnsetkef.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.dashuyun.cn/gtcqzxwnzt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xuanzx.com/gtfddklfmz.html

================================================================================
来源：http://hz.yanxiufei.cn/gtilinehum.html

I. 正则表达式
来源：http://hz.zhoulong.xyz/gtdzrhvofc.html

================================================================================
来源：http://hz.ppjwa.cn/gtwyfklfvb.html

[I01] 判断是否匹配
来源：http://hz.yj202588.top/gtuuhvmoaa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj202588.top/gtigdbegnw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj20258.top/gtobibsfcr.html

JS:   /\d+/.test(s)
来源：http://hz.ywan-chungtsiang.top/gtcuvgiicz.html

TS:   /\d+/.test(s)
来源：http://hz.xziqi.cn/gtunjveqso.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gotoacloud.top/gtshkfprbk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sweek.top/gtmvjqnwdy.html

Ruby: s.match?(/\d+/)
来源：http://hz.jqgufenzy.top/gtfkjvgcwa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yuxming.cn/gtxposxdff.html

[I02] 提取所有匹配
来源：http://hz.ybcxt.top/gtdiztpidu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zdqjudy.top/gtowsiaqvj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cashguo.top/gtcvfuwyvz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.snrcjt.cn/gtvmaebapy.html

TS:   s.match(/\d+/g)
来源：http://hz.hnxiangtu.top/gtkhjngcck.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shuidangran.top/gtdmkhpiqu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yonumen.top/gtfziqufuz.html

Ruby: s.scan(/\d+/)
来源：http://hz.quarkkingdee.top/gtpscuaflt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.snrcjt.cn/gtdilhnctt.html

[I03] 提取捕获分组
来源：http://hz.nanxuanxn.top/gteaofodty.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cdnleiting.top/gtylcoklxb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinghuilouyu.cn/gtedsbjlyq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nanxinkj.top/gtvshmiuiv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cqqwz.cn/gtcidfnepg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hnqzz.top/gtlocobmsd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cqqwz.cn/gtkxhossgk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guowangkeji.top/gthsuqwizl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ydjk.org.cn/gtnwwtxffo.html

[I04] 正则替换
来源：http://hz.guannengcc.top/gtgrshdtmj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hysaishi.cn/gtfvtiqgus.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.daxiang520.top/gtektthmam.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.dashuyun.cn/gtchvvszeb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.aibaodan.cn/gttvfovvkx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xziqi.cn/gtnnoazkpw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aibaodan.cn/gtjeexspjq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnqzz.top/gtvimtaeco.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sweek.top/gtypqqfffo.html

[I05] 按正则拆分
来源：http://hz.shanyushiyangkeji.top/gtuvuzvysj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yonumen.top/gtrgwywera.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hongshengwenyu.top/gtzwcehhpn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtfturkzyf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gtrbpwadzu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenjidiqi.icu/gtstxubvsy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ybcxt.top/gtynlunpao.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zdqjudy.top/gtiiuuiurb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.birdmap.top/gtiodnjwef.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.kuanghao11.cn/gtuhxtaoli.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xinyue.icu/gtimmcxzhw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gaohongyu789.top/gtbtsnlkuq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gogol.net.cn/gtktkfvmut.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pycfn.com/gtwuhmjdhm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.mhx1999.top/gtsvumvkdv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gzhubu.top/gtloyngfov.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xuanzx.com/gtxmcxmmqo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hywenlv.cn/gtnmjkailm.html

[I07] 忽略大小写与多行模式
来源：http://hz.gzhubu.top/gtuuelekta.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.fengsongda.top/gtsenqvtjk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xingfuxueyuan.xyz/gtpyupsgpa.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhiwuduotai.top/gtjzbwkhmz.html

TS:   /error/gim
来源：http://hz.fzhhl.top/gthejnuvyj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhixingplan.top/gtldrvtpek.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pycfn.com/gttwzmhetw.html

Ruby: s.scan(/error/i)
来源：http://hz.quarkkingdee.top/gtjmxrofge.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj202588.top/gtzugxsdxu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.guowangkeji.top/gtiqfnwmuf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jlsjyb.cn/gtebawondu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.dashuyun.cn/gtthduhlzr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtuevkuqse.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.haohaochexian.top/gtsevzqkmp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sweek.top/gthcwgqmim.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.pycfn.com/gtpcyqaxrw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.guowangkeji.top/gtslzvlotx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.quarkkingdee.top/gtfngulikd.html

================================================================================
来源：http://hz.316326.xyz/gtmysehbpa.html

J. 日期与时间
来源：http://hz.haohaochexian.top/gttdnfswzx.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtpcqyprnh.html

[J01] 获取当前时间
来源：http://hz.xylfe.cn/gtjhyykity.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangtech.top/gtohdjaqgx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sufxvd.cn/gtbrerpzja.html

JS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtpnqreuxy.html

TS:   new Date();  Date.now()
来源：http://hz.yueranfly.top/gthrvwbgwy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ivvv.top/gtyrhvxhmj.html

Go:   time.Now()
来源：http://hz.sxryk.cn/gtoredbndj.html

Ruby: Time.now
来源：http://hz.yonumen.top/gtwtugszwa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jqgufenzy.top/gtgdjqnbhr.html

[J02] 格式化输出
来源：http://hz.ehwqpu.com/gtnlmqrkia.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shangyingyoupin.top/gtxkomkqpu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.0kj1m.cn/gtrqkmxeyr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jqgfzy.top/gtdwafofvw.html

TS:   d.toISOString()
来源：http://hz.jqgufenzy.top/gtumpsosxo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.snrcjt.cn/gtruegidck.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yonumen.top/gtszmupyut.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gaohongyu789.top/gtnigqlrpe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ywan-chungtsiang.top/gtnvdxkauz.html

[J03] 字符串解析为日期
来源：http://hz.ivvv.top/gtdycrbaaj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tianlin.xyz/gtdeaszcuk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sxryk.cn/gtiibyrjqm.html

JS:   new Date("2024-01-02")
来源：http://hz.zycfv.cn/gtelezsthn.html

TS:   new Date("2024-01-02")
来源：http://hz.guowangkeji.top/gtwwgaaxph.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zycfv.cn/gtdkzxpiya.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtkhomhqvw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tian-w.cn/gtgojymnbw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xylfe.cn/gtyombhrlp.html

[J04] 时间戳与日期互转
来源：http://hz.jiagoushi.top/gtlxxfbqcj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhengqikj.top/gtacohavve.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yvedp.cn/gtcohfayul.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigufen.top/gtfkaanpub.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xingfuxueyuan.xyz/gtnqpnhehr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.fengsongda.top/gtwgsdaecm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.haohaochexian.top/gtonuevjnw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gogol.net.cn/gttblppvwu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.svipenyu.cn/gtbviiweur.html

[J05] 时间加减（加 7 天）
来源：http://hz.sysykeji.top/gtmalstemj.html

Py:   now + timedelta(days=7)
来源：http://hz.yj20258.top/gtoekwfnuq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ehwqpu.com/gtwmwnwkts.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yongpay.top/gtdtwtyxrq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sxryk.cn/gtodrpjrno.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hongshengwenyu.top/gtfgrrudso.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gzhubu.top/gtsmbbuiyj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.smart0.xyz/gtyrorraxv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxuanxn.top/gtsnqqubku.html

[J06] 计算两时间之差
来源：http://hz.hnqzz.top/gtenhmotbp.html

Py:   (end - start).total_seconds()
来源：http://hz.haohaochexian.top/gtdwzcjcdo.html

PHP:  $end->diff($start)->days;
来源：http://hz.sweek.top/gtgpdzervr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.wangdashe.top/gtxlnxdqvr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yueranfly.top/gtqaazqzft.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yonumen.top/gtsnekmdnb.html

Go:   end.Sub(start).Hours()
来源：http://hz.xziqi.cn/gtrpfnnrap.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yongpay.top/gtwyescqzv.html

C#:   (end - start).TotalSeconds
来源：http://hz.xuanzx.com/gtanjdjhwl.html

[J07] 比较两个日期
来源：http://hz.xuetiantiany.cn/gtvghrppie.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtrckilpqx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj20258888.top/gtruigtnjy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtfbkbkvxm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yuxming.cn/gteyvvrmca.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hammf.cn/gtwszzqsfv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.aizwys.cn/gtcawytgwp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtbnhhdcom.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtuibeifjf.html

[J08] 提取年月日与星期
来源：http://hz.zhongyouzk.top/gtvufucyvz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cucudq.cn/gtacjrxumj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.quarkkingdee.top/gtawsdgexj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yangfankeji.com/gtxaevxauc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cqqwz.cn/gtsfzluiez.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hysaishi.cn/gtoyzytxqh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hongshengwenyu.top/gtyxcmwvyc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.haohaochexian.top/gtwbvlxxax.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.birdmap.top/gtaaekqgtb.html

[J09] 时区处理
来源：http://hz.jianghu66.top/gtzifmjjjq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hammf.cn/gtbrpyqvle.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.guowangkeji.top/gtylyfmajj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sxryk.cn/gtismjlrjy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtmhuhikpq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hysaishi.cn/gtsfedvgfl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guannengcc.top/gtajqvffob.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daria6918.cn/gtbzigkxds.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.nwbrower.top/gteqzgxohs.html

[J10] 取今天 / 本月第一天
来源：http://hz.daxiang520.top/gtozltqpmp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.daria6918.cn/gtdahvevlv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj20258888.top/gttutuzqfs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj20258.top/gtmaqplvdg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.daria6918.cn/gtaavegzbv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daxiang520.top/gthaayndba.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yvedp.cn/gtmolpxtoe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gzhubu.top/gtnquijgcp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jianghu66.top/gttsyewfjb.html

================================================================================
来源：http://hz.guowangkeji.top/gtaraaofbz.html

K. JSON 与序列化
来源：http://hz.kuanghao11.cn/gtobrqsfri.html

================================================================================
来源：http://hz.cashguo.top/gtawpvtcqy.html

[K01] 对象转 JSON 字符串
来源：http://hz.nanxuanxn.top/gtbkuvdmip.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinghuilouyu.cn/gtkmzwazsd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gtwkgoluap.html

JS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gtyerylpuf.html

TS:   JSON.stringify(obj)
来源：http://hz.sufxvd.cn/gtwzbjhdnj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xingfuxueyuan.xyz/gtnbsjwiwj.html

Go:   json.Marshal(obj)
来源：http://hz.ywan-chungtsiang.top/gtqpkndizb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.mhx1999.top/gtxsainade.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.dianchejie.cn/gtcggkykbg.html

[K02] JSON 字符串转对象
来源：http://hz.zdqjudy.top/gtkdfdzsig.html

Py:   json.loads(s)
来源：http://hz.shzxlz.cn/gtxxtvqsek.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shzxlz.cn/gtlgdwzjkr.html

JS:   JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtdeqcvxtr.html

TS:   JSON.parse(s)
来源：http://hz.gotoacloud.top/gtlpcfupsj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fengsongda.top/gtcuknmelh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jiagoushi.top/gtdwnqdexg.html

Ruby: JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtikwncmyb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhijiandao.cn/gtwequwlor.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.meibo888.top/gtniwvdtqt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.daxiang520.top/gtsdqtcjrs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ydzc1.top/gtbjlbghif.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigufen.top/gtgpjolblt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj202588.top/gtjmzkcsvq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhixingplan.top/gtjqijeffd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hfpthk.cn/gtmfftnuac.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.aizwys.cn/gtrwpezbpg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zycfv.cn/gteuaokrcy.html

[K04] 读取 JSON 文件
来源：http://hz.jinqigufen.top/gtcnssipoj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinghuilouyu.cn/gtaeafylxg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinyuanbaomall.cn/gtaumnmure.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtrujosuqj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.smart0.xyz/gtpfswoyre.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.andypj.xyz/gtzufbuadv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.wangshuangyany.cn/gtonqvjclv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tianlin.xyz/gtgxpwafli.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.andypj.xyz/gtsmbjlyyv.html

[K05] 深拷贝对象
来源：http://hz.gzhubu.top/gtkfkqeakv.html

Py:   copy.deepcopy(obj)
来源：http://hz.gotoacloud.top/gtlzgzpdrh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.feifeiyinyue.top/gtytvdtzii.html

JS:   structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtcfluqhis.html

TS:   structuredClone(obj)
来源：http://hz.yj20258888.top/gtglsvrifk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shuidangran.top/gtwquxrsbr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hnqzz.top/gtejvfjiya.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangtech.top/gtiwmdrwyv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cqqwz.cn/gtlaihzsdn.html

[K06] 解析 URL 查询串
来源：http://hz.sufxvd.cn/gtmfovhnmu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtkudytbgf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xinyue.icu/gtcnfixlxd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gttxhlntzw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.smart0.xyz/gtwzpckwyh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.andypj.xyz/gtskpaqfdz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenzaomai.com/gtanpdmiaz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yvedp.cn/gtvzevdovq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xinyue.icu/gtopniutpz.html

[K07] 进制转换
来源：http://hz.kuanghao11.cn/gtnirmhuip.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hysaishi.cn/gtsvfbblth.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xylfe.cn/gtpuycvnot.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.daxiang520.top/gtmprsndge.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cashguo.top/gtocbhrson.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtkguyeoep.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xinyue.icu/gttucmltfo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj20258.top/gtzalkrusf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gotoacloud.top/gthiiyugvi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.iojbl.cn/gtscrztfiy.html

Py:   pickle.dumps(obj)
来源：http://hz.yuxming.cn/gtmvtbocpi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.kuanghao11.cn/gtfjyqqhrw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.guowangkeji.top/gtkrfatvky.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.316326.xyz/gthqcbxygj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.meibo888.top/gtbzrodzji.html

Go:   encoding/gob
来源：http://hz.pengpengdd.cyou/gtfthugytr.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenzaomai.com/gtpfpoqnye.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.haohaochexian.top/gthtoetata.html

================================================================================
来源：http://hz.gzhubu.top/gtiugvkdqb.html

L. 网络请求
来源：http://hz.jqgufenzy.top/gtykpwonjq.html

================================================================================
来源：http://hz.wangdashe.top/gtmzokzgiw.html

[L01] 发送 GET 请求
来源：http://hz.yongpay.top/gteuwzsrjk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yongpay.top/gtdgwqtwwz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hnxiangtu.top/gtnybrrhnv.html

JS:   await fetch(url)
来源：http://hz.jianghu66.top/gtbrfbbfxu.html

TS:   await fetch(url)
来源：http://hz.cqqwz.cn/gtlmneqjau.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhoulong.xyz/gtblstxewh.html

Go:   resp, err := http.Get(url)
来源：http://hz.svipenyu.cn/gtduplttgm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhoulong.xyz/gthodvhzwc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shzxlz.cn/gtuilayjxv.html

[L02] 发送 POST JSON
来源：http://hz.vqdsnc.cn/gtdqqctlny.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.wangshuangyany.cn/gtswtrkfvh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cqqwz.cn/gtxewkpvvz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ppjwa.cn/gtarcaztqd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gthbwofniq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gaohongyu789.top/gtqkgtnmms.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ywan-chungtsiang.top/gthigbtlvn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.dashuyun.cn/gtcwazuyeu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shzxlz.cn/gtzgekgzsc.html

[L03] 设置自定义请求头
来源：http://hz.yonumen.top/gtkbwshcvx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhongyouzk.top/gtpojlaoin.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.fengsongda.top/gtfkbtooqk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinyuanbaomall.cn/gtcgpaflzy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yvedp.cn/gtlhrxjchi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenjidiqi.icu/gtnlmoaful.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.guannengcc.top/gtgfyoaqgf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhongyouzk.top/gtqrlzwfhj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.quarkkingdee.top/gtrlefiwgw.html

[L04] 设置超时
来源：http://hz.pycfn.com/gtmrahtzyd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hnqzz.top/gtnlqenqhr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jianghu66.top/gtgjycubqa.html


<!-- 参考信息 -->