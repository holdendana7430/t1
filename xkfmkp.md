代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://hz.shzxlz.cn/gtfvquyngw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yonumen.top/gtdfgujgme.html

[H09] 带错误码的异常
来源：http://hz.zhoulong.xyz/gteehtqsly.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.mhx1999.top/gttcuuqntu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinqigufen.top/gtbptmgavh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.snrcjt.cn/gthqmryupl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jqgfzy.top/gtxxrclqcz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gotoacloud.top/gtmmdwicuh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.quarkkingdee.top/gtfedhrqnz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.quarkkingdee.top/gtnlllplog.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.quarkkingdee.top/gtymrtbkwl.html

[H10] 资源自动释放
来源：http://hz.tianlin.xyz/gtzgqlmbgp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.kuanghao11.cn/gtqucxxnqc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nanxuanxn.top/gtrzgnrtyn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guannengcc.top/gtydymsoqb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yongpay.top/gtgcjulydb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.iojbl.cn/gtsvglfnte.html

Go:   defer f.Close()
来源：http://hz.9152youxi.cn/gtzebwzxuy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sysykeji.top/gtfyjsecow.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnqzz.top/gtzgavlipw.html

================================================================================
来源：http://hz.pycfn.com/gtnemzgxru.html

I. 正则表达式
来源：http://hz.nanxinkj.top/gtykqoiktx.html

================================================================================
来源：http://hz.fzhhl.top/gtigvykcgh.html

[I01] 判断是否匹配
来源：http://hz.hfpthk.cn/gthzbgtmgl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hywenlv.cn/gtnjbepwqi.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigufen.top/gtkxqziels.html

JS:   /\d+/.test(s)
来源：http://hz.guannengcc.top/gtcunpqlmq.html

TS:   /\d+/.test(s)
来源：http://hz.gzhubu.top/gtigqoeuax.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhiwuduotai.top/gtdsdaxqrd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sysykeji.top/gthodnkfnu.html

Ruby: s.match?(/\d+/)
来源：http://hz.snrcjt.cn/gtxbqkvlxr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cheryme.top/gtocuqkdmu.html

[I02] 提取所有匹配
来源：http://hz.sweek.top/gtpydxmkcc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cashguo.top/gtptdqxtiv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.daxiang520.top/gtaedpczkn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cheryme.top/gtetrgtbqa.html

TS:   s.match(/\d+/g)
来源：http://hz.wangshuangyany.cn/gtyuwcmxug.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ppjwa.cn/gtmdsleppf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yuanzhike.top/gtexksawhh.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhiwuduotai.top/gtjgvulxkk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hongshengwenyu.top/gtreauigbj.html

[I03] 提取捕获分组
来源：http://hz.bjfxy.top/gtxprifexe.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ybcxt.top/gtgsaumfuw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gaohongyu789.top/gtgkulskdk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.vqdsnc.cn/gttjuhnwdr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenzaomai.com/gttbohogrn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gogol.net.cn/gtkagxkzmw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj202588.top/gtxiwqlizx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jiagoushi.top/gtpwljjqln.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.kuanghao11.cn/gtihnvywmm.html

[I04] 正则替换
来源：http://hz.zhongyouzk.top/gthgwzcyyh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgufenzy.top/gtzothmbsv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.52xcode.cn/gtwulcklmx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.quarkkingdee.top/gtjggtpurg.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtujyzjkgn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jlsjyb.cn/gtfytrojcx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhongyouzk.top/gtgrbbyskz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jqgfzy.top/gtjmgahlvo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zdqjudy.top/gtzbxwycbx.html

[I05] 按正则拆分
来源：http://hz.hysaishi.cn/gtnczzptdq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tianlin.xyz/gtduwusnrb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xuanzx.com/gtppttbhnr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtccfxpzfn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtncrwyhib.html

Java: s.split("\\s*,\\s*")
来源：http://hz.tian-w.cn/gteaocnzlg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zycfv.cn/gtimuxxntl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtevcgymcq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jianghu66.top/gtatudbpni.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.daxiang520.top/gtegbhnymf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hnxiangtu.top/gtkyeswsjb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jianghu66.top/gttexbkvac.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pengpengdd.cyou/gtccvldlgr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinyuanbaomall.cn/gtwnjvqpxr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhongyouzk.top/gtlfubwrhz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yuxming.cn/gtpkydfvtp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhongyouzk.top/gtwyihusgs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yongpay.top/gtcrmnefkz.html

[I07] 忽略大小写与多行模式
来源：http://hz.xylfe.cn/gtahejseti.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ppjwa.cn/gtbqcjtrmm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.smart0.xyz/gtupdfaeey.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.316326.xyz/gtdpaeooxx.html

TS:   /error/gim
来源：http://hz.kuanghao11.cn/gtfkbkuwos.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.birdmap.top/gtskqqlzqn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj202588.top/gtzafoamiv.html

Ruby: s.scan(/error/i)
来源：http://hz.kuanghao11.cn/gtddbnknhb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sweek.top/gtkuvsrtnd.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sweek.top/gtvxiinsge.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.chenjidiqi.icu/gthfctihhf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.bjfxy.top/gtbvhtpfgh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuxming.cn/gtsyvashgp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gzhubu.top/gtjhgnckhf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jqgfzy.top/gtnxmjpgnn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.wangdashe.top/gtgqsllicg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jlsjyb.cn/gtdlixafgl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jiagoushi.top/gtqxduatjg.html

================================================================================
来源：http://hz.cdnleiting.top/gtokuokyyl.html

J. 日期与时间
来源：http://hz.feifeiyinyue.top/gtzxszbbsp.html

================================================================================
来源：http://hz.ybcxt.top/gtqbtpiyiv.html

[J01] 获取当前时间
来源：http://hz.9152youxi.cn/gtofkdvfkj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.fzhhl.top/gtfyfjoloi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.dianchejie.cn/gtkuifphac.html

JS:   new Date();  Date.now()
来源：http://hz.ydzc1.top/gtzapsburr.html

TS:   new Date();  Date.now()
来源：http://hz.chenzaomai.com/gttglfacnu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hnxiangtu.top/gtntarypky.html

Go:   time.Now()
来源：http://hz.nanxinkj.top/gtxbowlzke.html

Ruby: Time.now
来源：http://hz.jinqigfzy.top/gtrigzixbc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hysaishi.cn/gtawfzjqpc.html

[J02] 格式化输出
来源：http://hz.tanke756.top/gtsaqimddu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxuanxn.top/gtdmhrdsjp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.pycfn.com/gtrqtsyfzq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ppjwa.cn/gtakilynui.html

TS:   d.toISOString()
来源：http://hz.yuanzhike.top/gtfofczuht.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhijiandao.cn/gtwuzfosud.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinqigfzy.top/gtdxefdmck.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtiicinsqz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gogol.net.cn/gtoaikgtqg.html

[J03] 字符串解析为日期
来源：http://hz.cashguo.top/gtnehylxow.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zdqjudy.top/gtkoruzyun.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cdnleiting.top/gtvujrqsvx.html

JS:   new Date("2024-01-02")
来源：http://hz.chenlongwang.top/gtzlsdgoyq.html

TS:   new Date("2024-01-02")
来源：http://hz.c1oappe.top/gtbadfbozu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gogol.net.cn/gtqrxpwbfw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xuanzx.com/gtpgfomdtw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.bjfxy.top/gtxpgxrczn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.snrcjt.cn/gtjrkleqwc.html

[J04] 时间戳与日期互转
来源：http://hz.chenjidiqi.icu/gtdqdbgcer.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.0kj1m.cn/gthivmnins.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yangfankeji.com/gtmjfaqpqw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yvedp.cn/gtdexokwvj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.mhx1999.top/gtstrluaiy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.vqdsnc.cn/gtxafugmca.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cdnleiting.top/gtxsorxliq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.redwolf501.top/gtlazczrep.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shangyingyoupin.top/gtgqjnxnrk.html

[J05] 时间加减（加 7 天）
来源：http://hz.ppjwa.cn/gticmyincf.html

Py:   now + timedelta(days=7)
来源：http://hz.yueranfly.top/gtctiqbgad.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinqigfzy.top/gtujigfdjw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuanzx.com/gtsgliavxd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gtiwxtvhbz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinghuilouyu.cn/gtnicslhxn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.svipenyu.cn/gtzrvzmnpr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ybcxt.top/gtdufwrqds.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.wangdashe.top/gtzvyirkqh.html

[J06] 计算两时间之差
来源：http://hz.jlsjyb.cn/gtiokbnivi.html

Py:   (end - start).total_seconds()
来源：http://hz.zhijiandao.cn/gtvqdxrcrb.html

PHP:  $end->diff($start)->days;
来源：http://hz.yueranfly.top/gtcsdozqhh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.meibo888.top/gtsvervcsj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cheryme.top/gtudlfpcwi.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.andypj.xyz/gtbbbbntdg.html

Go:   end.Sub(start).Hours()
来源：http://hz.0kj1m.cn/gtfzdkweud.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xylfe.cn/gtcllxopwx.html

C#:   (end - start).TotalSeconds
来源：http://hz.sufxvd.cn/gtpgqxzewq.html

[J07] 比较两个日期
来源：http://hz.birdmap.top/gtquilxxqt.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtexweidjr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cqqwz.cn/gtptmgjzoh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgufenzy.top/gtkujniqlp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shzxlz.cn/gtkzddmasv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tanke756.top/gtrwjhdcet.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenlongwang.top/gtpapyrydy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtrkbhnbqt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtcjclggaz.html

[J08] 提取年月日与星期
来源：http://hz.guowangkeji.top/gtgkquagms.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.havefunace.top/gtzojofynz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shangyingyoupin.top/gtlswggssw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zdqjudy.top/gtbwkcjgnv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hnqzz.top/gtnzvplokw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.pengpengdd.cyou/gtficfmnvn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xinyue.icu/gtbipfeepn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gotoacloud.top/gtnioqlsbz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daxiang520.top/gtzdaunnbg.html

[J09] 时区处理
来源：http://hz.nanxinkj.top/gtztpgdlvg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sweek.top/gtilkdkses.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yangfankeji.com/gtemuwvzfg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydjk.org.cn/gtfsaazopl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sxryk.cn/gtjrmphizt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxuanxn.top/gtqdhfeniq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guowangkeji.top/gtdybwnvad.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hongshengwenyu.top/gtopiuoetf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.meibo888.top/gtmjpuexit.html

[J10] 取今天 / 本月第一天
来源：http://hz.gzhubu.top/gtcmwhzniv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.guannengcc.top/gtmynblyoo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shzxlz.cn/gtbsiqbdvl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sysykeji.top/gtarlobgvb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cheryme.top/gthqeohafo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.pycfn.com/gtqfvrisnq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhaomingkeji.xyz/gttjtjoztn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jyoumei.cn/gtfiydoccf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yuanzhike.top/gtikmnhehg.html

================================================================================
来源：http://hz.zhongyouzk.top/gtnwrvrsjw.html

K. JSON 与序列化
来源：http://hz.guannengcc.top/gtvdgnojfu.html

================================================================================
来源：http://hz.ppjwa.cn/gtfoxhyjrt.html

[K01] 对象转 JSON 字符串
来源：http://hz.jlsjyb.cn/gtzlxilghh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jiagoushi.top/gtdxsbknbw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ivvv.top/gtaqiokmcq.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangtech.top/gtcbqmkdnp.html

TS:   JSON.stringify(obj)
来源：http://hz.ydjk.org.cn/gturrktwlo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenjidiqi.icu/gtliwhwlrz.html

Go:   json.Marshal(obj)
来源：http://hz.ivvv.top/gtueimxyjx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jiagoushi.top/gtoadzawma.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangshuangyany.cn/gtkajrxdrt.html

[K02] JSON 字符串转对象
来源：http://hz.pycfn.com/gtwemzwryk.html

Py:   json.loads(s)
来源：http://hz.xziqi.cn/gtkrcnqsuf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ydjk.org.cn/gtdnkauldf.html

JS:   JSON.parse(s)
来源：http://hz.tianlin.xyz/gtseeaxzfv.html

TS:   JSON.parse(s)
来源：http://hz.0kj1m.cn/gtjqfthrba.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cqqwz.cn/gtshyzutju.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xuetiantiany.cn/gtwcahwivo.html

Ruby: JSON.parse(s)
来源：http://hz.sufxvd.cn/gtsbajowlu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.bjfxy.top/gtxcymatmc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hongshengwenyu.top/gtugidhygd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.guowangkeji.top/gtpduicsti.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtktsjqwir.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.kuanghao11.cn/gtiavqvtme.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jianghu66.top/gtosvhuewf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tianlin.xyz/gtdjifrmzq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zdqjudy.top/gtmwppwbkh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.birdmap.top/gtgbpeihmx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.9152youxi.cn/gtgagpufpc.html

[K04] 读取 JSON 文件
来源：http://hz.hysaishi.cn/gtpvdrelmo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hysaishi.cn/gtnxeglqcg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sweek.top/gtaxkwtnzl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtioxplszl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.meibo888.top/gtzptmkpht.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yonumen.top/gtdjfcsndo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.daxiang520.top/gtpgnpgygl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tanke756.top/gtylredypf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jiagoushi.top/gtmjlidujs.html

[K05] 深拷贝对象
来源：http://hz.hysaishi.cn/gtpgxdsudy.html

Py:   copy.deepcopy(obj)
来源：http://hz.birdmap.top/gtgirqsdbg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.pycfn.com/gtxbhqcmeo.html

JS:   structuredClone(obj)
来源：http://hz.shanyushiyangtech.top/gtpiwkhtww.html

TS:   structuredClone(obj)
来源：http://hz.ydjk.org.cn/gtitkmbtxm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.52xcode.cn/gtnwreyahl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.daria6918.cn/gtclbasrsy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.smart0.xyz/gtkijimxol.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hammf.cn/gtxigyzvvs.html

[K06] 解析 URL 查询串
来源：http://hz.jyoumei.cn/gteyfawxbg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.gzhubu.top/gtigtjixhl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gogol.net.cn/gtkvwwyqoa.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtbqxpyclw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gotoacloud.top/gtrxxwwmyq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.redwolf501.top/gtptimrvre.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.wangdashe.top/gtaupakvpt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sufxvd.cn/gtgpzneigx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tian-w.cn/gthoudmbky.html

[K07] 进制转换
来源：http://hz.birdmap.top/gtgpbopsun.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hnqzz.top/gtudbfmqln.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yangfankeji.com/gtskpbzxjy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.pengpengdd.cyou/gtwhbtaugx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtuawhbtsm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yj202588.top/gtjqmunwjh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.aibaodan.cn/gtlxahndrx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hysaishi.cn/gtgcwnlsqq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ydzc1.top/gtfkcxvwxt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nanxuanxn.top/gtcajevwcv.html

Py:   pickle.dumps(obj)
来源：http://hz.wangdashe.top/gtspfdskst.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jyoumei.cn/gtfiohqeyh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.birdmap.top/gtyrjtybsv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gtxdynatpb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ydjk.org.cn/gtjgtjvblj.html

Go:   encoding/gob
来源：http://hz.sysykeji.top/gtlrbvpvik.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinqigfzy.top/gtbrypvpot.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nanxuanxn.top/gtqwxqrnxa.html

================================================================================
来源：http://hz.tian-w.cn/gtqujweuoc.html

L. 网络请求
来源：http://hz.yonumen.top/gtrbhvjstx.html

================================================================================
来源：http://hz.0kj1m.cn/gtioolipxq.html

[L01] 发送 GET 请求
来源：http://hz.chenjidiqi.icu/gtqoksoieh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jiagoushi.top/gtwixhmafq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nanxuanxn.top/gtrtyoyojq.html

JS:   await fetch(url)
来源：http://hz.yonumen.top/gtkmpgrwsk.html

TS:   await fetch(url)
来源：http://hz.hnxiangtu.top/gtokvpnzhy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ehwqpu.com/gtjiwzamdh.html

Go:   resp, err := http.Get(url)
来源：http://hz.tianlin.xyz/gtmywtbjts.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sxryk.cn/gtplvdmifg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yuanzhike.top/gtbfjgolww.html

[L02] 发送 POST JSON
来源：http://hz.hnqzz.top/gtcnramide.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.kuanghao11.cn/gtafpzzudi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hnqzz.top/gtvhxynjpo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhaomingkeji.xyz/gtizkkobxy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aibaodan.cn/gtbgozlmzo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cheryme.top/gtemjjcjxx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ivvv.top/gtindnuoja.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.fzhhl.top/gtxpeldhhm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yangfankeji.com/gtqtfhnkfy.html

[L03] 设置自定义请求头
来源：http://hz.tian-w.cn/gtgjpmagwc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zycfv.cn/gtnyezgzun.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sysykeji.top/gtkzwyflut.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gtpgnnfuml.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yueranfly.top/gtibhuqidj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ehwqpu.com/gthqojgymj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ybcxt.top/gtjsrgdwdz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhixingplan.top/gtlnkszceq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.dashuyun.cn/gtoeidzdlt.html

[L04] 设置超时
来源：http://hz.quarkkingdee.top/gtnjwbvfot.html

Py:   requests.get(url, timeout=5)
来源：http://hz.quarkkingdee.top/gtcqviztqy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.kuanghao11.cn/gtmhxpjnsb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtfqwcdvar.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tanke756.top/gtkbhgsaze.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.havefunace.top/gtnrxikfcp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhiwuduotai.top/gthtopoqvw.html


<!-- 参考信息 -->