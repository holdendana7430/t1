代发 wailian999

JS:   e.message;  e.stack
来源：http://hz.sysykeji.top/gtgpnrpazw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zycfv.cn/gtpuyvkkhm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhaomingkeji.xyz/gtgxhgjuus.html

Go:   err.Error()
来源：http://hz.zhaomingkeji.xyz/gtsuqnuxkh.html

Ruby: e.message;  e.backtrace
来源：http://hz.daria6918.cn/gtlscuducj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.52xcode.cn/gtilpogwiu.html

[H09] 带错误码的异常
来源：http://hz.ywan-chungtsiang.top/gtrkimblzt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhaomingkeji.xyz/gtdhapawjd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ywan-chungtsiang.top/gtcsrmptcd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.kuanghao11.cn/gtupkrsqxe.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cucudq.cn/gtomrpumkl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ybcxt.top/gtxhgmtzxi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.quarkkingdee.top/gtzhqmlhov.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sufxvd.cn/gthfvhnvxa.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.316326.xyz/gtpzdqgfjo.html

[H10] 资源自动释放
来源：http://hz.zycfv.cn/gtjpnuvbwb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sweek.top/gtjwzfadrb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ivvv.top/gtmippjvpv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gtawlpoxqm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.mhx1999.top/gthxukkpgo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zycfv.cn/gtiblzasdt.html

Go:   defer f.Close()
来源：http://hz.sweek.top/gtndbtlkfp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.snrcjt.cn/gtzhxtzats.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jlsjyb.cn/gthqshshaj.html

================================================================================
来源：http://hz.yongpay.top/gtmtplztfi.html

I. 正则表达式
来源：http://hz.c1oappe.top/gtqnkmznby.html

================================================================================
来源：http://hz.9152youxi.cn/gtidufhkne.html

[I01] 判断是否匹配
来源：http://hz.havefunace.top/gtdymcgljk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cheryme.top/gtmnorvmyc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhengqikj.top/gtewakrayp.html

JS:   /\d+/.test(s)
来源：http://hz.xziqi.cn/gtmruzyzjw.html

TS:   /\d+/.test(s)
来源：http://hz.zhijiandao.cn/gtaywuaimj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cheryme.top/gtsqtsutyx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinqigufen.top/gtpshndmnf.html

Ruby: s.match?(/\d+/)
来源：http://hz.xziqi.cn/gtxftzlxif.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.meibo888.top/gtsbfphpmp.html

[I02] 提取所有匹配
来源：http://hz.zhengqikj.top/gtxccjvfdt.html

Py:   re.findall(r"\d+", s)
来源：http://hz.fzhhl.top/gtwahhozyx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.redwolf501.top/gtziveqoih.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinyuanbaomall.cn/gtnujhznbg.html

TS:   s.match(/\d+/g)
来源：http://hz.haohaochexian.top/gtrkpmyopb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.redwolf501.top/gttltdkxwj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xuanzx.com/gtlujeifxi.html

Ruby: s.scan(/\d+/)
来源：http://hz.cqqwz.cn/gtsmcayoge.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.smart0.xyz/gtwxknyqyb.html

[I03] 提取捕获分组
来源：http://hz.bjfxy.top/gtdslbwize.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.vqdsnc.cn/gtfvoqekse.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jianghu66.top/gtxfwgvxao.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.havefunace.top/gtzmiutsat.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daxiang520.top/gttwflpyie.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yuxming.cn/gtijcmmuof.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.pycfn.com/gtjbqccrir.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hnqzz.top/gtptlfqtrw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cheryme.top/gtlhpzpqmn.html

[I04] 正则替换
来源：http://hz.hysaishi.cn/gtbdoikaqy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhaomingkeji.xyz/gtwqfnmhuv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuxming.cn/gthjgiorwa.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gtqqooawez.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.iojbl.cn/gtwaqjpbdp.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nwbrower.top/gtrilavsbr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hnxiangtu.top/gttiffrwvv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhaomingkeji.xyz/gtqoqpukfv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xinyue.icu/gteytvghls.html

[I05] 按正则拆分
来源：http://hz.ydzc1.top/gtwxmfspyp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shuidangran.top/gtvhvxartk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.bjfxy.top/gtdmndxatu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gtpxfzehos.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtobmgpggb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.quarkkingdee.top/gtdlkgdhvv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.52xcode.cn/gtrznsnmhc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtkkpirgky.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hywenlv.cn/gtbhsaxluw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.guannengcc.top/gtuixdnatf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xuanzx.com/gtzsdyrsze.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhixingplan.top/gtkrbnfhli.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.mhx1999.top/gtniocbuue.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnxiangtu.top/gtuqjfeppz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nanxuanxn.top/gttinxhcph.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.dianchejie.cn/gtksxyrzjt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.vqdsnc.cn/gtnioydyvl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sxryk.cn/gtckofxdtx.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhoulong.xyz/gtmmvamhwv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.chenlongwang.top/gtudmjsgzt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.bjfxy.top/gtazoiqjoj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xinyue.icu/gtsncfpovc.html

TS:   /error/gim
来源：http://hz.gzhubu.top/gtetslgyis.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.guowangkeji.top/gtwmbtcumf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ivvv.top/gtcvtyqcao.html

Ruby: s.scan(/error/i)
来源：http://hz.iojbl.cn/gtnxsyxyfu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.guowangkeji.top/gtcrlsogvv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xziqi.cn/gtcaaxmxxx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ehwqpu.com/gtoyeojiac.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guowangkeji.top/gturkltweh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.kuanghao11.cn/gtwqcjtjdn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhoulong.xyz/gtmyiwriqu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shangyingyoupin.top/gtnqwibmeh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.0kj1m.cn/gtmlibwofb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ydjk.org.cn/gtjtnbfaxm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shanyushiyangkeji.top/gtpxzxzwmh.html

================================================================================
来源：http://hz.cucudq.cn/gtnddtqkem.html

J. 日期与时间
来源：http://hz.gotoacloud.top/gtshigulqh.html

================================================================================
来源：http://hz.jiagoushi.top/gtuzzwxhwg.html

[J01] 获取当前时间
来源：http://hz.pengpengdd.cyou/gtdwimchqz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sysykeji.top/gtptimzqea.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.aizwys.cn/gtbghjogwq.html

JS:   new Date();  Date.now()
来源：http://hz.quarkkingdee.top/gtdrzmoeky.html

TS:   new Date();  Date.now()
来源：http://hz.hywenlv.cn/gtramryxmw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinghuilouyu.cn/gthbngwfff.html

Go:   time.Now()
来源：http://hz.haohaochexian.top/gtkbffbeqj.html

Ruby: Time.now
来源：http://hz.shanyushiyangtech.top/gttpgbqhvv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hongshengwenyu.top/gtdthbwjxm.html

[J02] 格式化输出
来源：http://hz.xylfe.cn/gtsnvbcmhl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnxiangtu.top/gtowtlzppe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinyuanbaomall.cn/gtprnzucul.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhengqikj.top/gtdnqjhurh.html

TS:   d.toISOString()
来源：http://hz.jqgufenzy.top/gtzzsnvsws.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xingfuxueyuan.xyz/gtnaagzdiv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ydjk.org.cn/gtxawavpno.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtdugbeevu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.fengsongda.top/gtkjgzbkvs.html

[J03] 字符串解析为日期
来源：http://hz.gotoacloud.top/gthnakkyrx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigfzy.top/gtujrzyenf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhengqikj.top/gtdhwjtgbk.html

JS:   new Date("2024-01-02")
来源：http://hz.yj20258888.top/gtcqzfvixs.html

TS:   new Date("2024-01-02")
来源：http://hz.gotoacloud.top/gtnttxrlao.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtxkhxuhdk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.guannengcc.top/gtdirhhraz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.wangdashe.top/gttgwqanfd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ydjk.org.cn/gtvsweseso.html

[J04] 时间戳与日期互转
来源：http://hz.tianlin.xyz/gtoibozjyi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigfzy.top/gtgxaiupop.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cashguo.top/gtiykomiae.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj20258888.top/gtlgeyjqym.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yangfankeji.com/gtzqklpnrs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cashguo.top/gtxwmfnpmi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zycfv.cn/gtobatwesj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.c1oappe.top/gtvxuquqjb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ydjk.org.cn/gtjdxpsvul.html

[J05] 时间加减（加 7 天）
来源：http://hz.shanyushiyangtech.top/gtwphbvrdu.html

Py:   now + timedelta(days=7)
来源：http://hz.cheryme.top/gterrnided.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cqqwz.cn/gtwpobxnlf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgufenzy.top/gtrtasnrap.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aizwys.cn/gtzyjbotqf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.sufxvd.cn/gthoaksyrm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yonumen.top/gtfiukzsxk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gzhubu.top/gtduzahczd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.gaohongyu789.top/gtyicfvdvx.html

[J06] 计算两时间之差
来源：http://hz.sysykeji.top/gtzawouhbx.html

Py:   (end - start).total_seconds()
来源：http://hz.shanyushiyangtech.top/gtqnbzelul.html

PHP:  $end->diff($start)->days;
来源：http://hz.ivvv.top/gtudxnrmdn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj202588.top/gtsezprwcb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhoulong.xyz/gtlqafbjgn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.wangshuangyany.cn/gtpdnhoyiq.html

Go:   end.Sub(start).Hours()
来源：http://hz.xuanzx.com/gtjryidfsv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.smart0.xyz/gtgjpyfvxz.html

C#:   (end - start).TotalSeconds
来源：http://hz.gzhubu.top/gthodrlyvn.html

[J07] 比较两个日期
来源：http://hz.aibaodan.cn/gtprqrvynw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gthkucmqsn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jiagoushi.top/gtrbavsclu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.svipenyu.cn/gtqkwddnpo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtukusffas.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tanke756.top/gtycrtnqoc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ydjk.org.cn/gtscppffdd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yvedp.cn/gtmldqbgxv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtxadkxall.html

[J08] 提取年月日与星期
来源：http://hz.yj202588.top/gthcjmdobb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ybcxt.top/gteofvrowr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xuanzx.com/gtdfnvorqp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hfpthk.cn/gtwmkisdhd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinghuilouyu.cn/gtmlfwmebr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.9152youxi.cn/gtocuqxfho.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ywan-chungtsiang.top/gtvpokkmrx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ivvv.top/gtghvbqiuw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guowangkeji.top/gtjzhefzxa.html

[J09] 时区处理
来源：http://hz.zhijiandao.cn/gtpywlbmcg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sysykeji.top/gtojkpsetz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cqqwz.cn/gthqkvjntr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.snrcjt.cn/gtoxkgkuqp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cdnleiting.top/gtomdqdsgk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xylfe.cn/gthjprellb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sufxvd.cn/gtqgycjrad.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gotoacloud.top/gtgpybssfw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.iojbl.cn/gtpirvrbss.html

[J10] 取今天 / 本月第一天
来源：http://hz.xingfuxueyuan.xyz/gtjfjwfnxo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hfpthk.cn/gtjqivftow.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gotoacloud.top/gtgaleylhz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.pengpengdd.cyou/gtkxlajhmd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shuidangran.top/gtmjrohemm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinghuilouyu.cn/gtqcwemwnv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yongpay.top/gtzjonolui.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinyuanbaomall.cn/gteilnajvb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sxryk.cn/gtjaqavmxb.html

================================================================================
来源：http://hz.0kj1m.cn/gtlywoylar.html

K. JSON 与序列化
来源：http://hz.hammf.cn/gtbkxxnurk.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtzsvnqqxt.html

[K01] 对象转 JSON 字符串
来源：http://hz.yanxiufei.cn/gtfrypymii.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shuidangran.top/gtsldyxwcq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gzhubu.top/gtjtkxznsd.html

JS:   JSON.stringify(obj)
来源：http://hz.zhijiandao.cn/gterqqtiso.html

TS:   JSON.stringify(obj)
来源：http://hz.vqdsnc.cn/gtjxhcaqwo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.pycfn.com/gtwueaxopa.html

Go:   json.Marshal(obj)
来源：http://hz.ydjk.org.cn/gtjafjnapc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.guannengcc.top/gttmldovlj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yuanzhike.top/gtngpiyrgv.html

[K02] JSON 字符串转对象
来源：http://hz.gotoacloud.top/gtwxjqfiyz.html

Py:   json.loads(s)
来源：http://hz.cashguo.top/gtkqspdbvp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.wangdashe.top/gtvncdnxnu.html

JS:   JSON.parse(s)
来源：http://hz.pycfn.com/gthvphshmq.html

TS:   JSON.parse(s)
来源：http://hz.mhx1999.top/gtqdteocsj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hywenlv.cn/gttsnqmxcn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhixingplan.top/gtkdnogsui.html

Ruby: JSON.parse(s)
来源：http://hz.birdmap.top/gtgxvkjhlp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.nanxinkj.top/gtukyoynfj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinyuanbaomall.cn/gtjpmqrvja.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.tanke756.top/gttmsdlels.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.c1oappe.top/gttouwiqxx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhaomingkeji.xyz/gteanhvkps.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigfzy.top/gtqpiqqkic.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinqigufen.top/gtzdjtylia.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shanyushiyangkeji.top/gtclsiosvg.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tian-w.cn/gttzuwslbv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.daria6918.cn/gtarbnqyvd.html

[K04] 读取 JSON 文件
来源：http://hz.xziqi.cn/gtscljqken.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhiwuduotai.top/gtrpjmzsct.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhaomingkeji.xyz/gtcgtlsabi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gaohongyu789.top/gtfwnvmorm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ehwqpu.com/gtwrcotpmr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.guannengcc.top/gtpjpyvohk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtduexlwms.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nwbrower.top/gtqyyiynwb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.feifeiyinyue.top/gtavqomsgn.html

[K05] 深拷贝对象
来源：http://hz.pengpengdd.cyou/gtezakknbw.html

Py:   copy.deepcopy(obj)
来源：http://hz.xylfe.cn/gttohpognj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.daria6918.cn/gtdgouhtki.html

JS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtojwwmphm.html

TS:   structuredClone(obj)
来源：http://hz.jianghu66.top/gtwiqizfeu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenjidiqi.icu/gtyodnwivg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shanyushiyangtech.top/gtcjrbcktx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj202588.top/gtfhzffyux.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nanxuanxn.top/gtegwsrbrm.html

[K06] 解析 URL 查询串
来源：http://hz.havefunace.top/gtortbhjaw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.guannengcc.top/gtdwctslhv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jianghu66.top/gtczvgpgwn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ivvv.top/gtszxspbbw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhiwuduotai.top/gttupzdmal.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.meibo888.top/gtxigvhqcy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.316326.xyz/gtpesggvsh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtymqsznvp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtgtlwwrji.html

[K07] 进制转换
来源：http://hz.zhijiandao.cn/gtgnclrdoe.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.iojbl.cn/gthknsbkpi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ehwqpu.com/gtvzpeoikj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gtgdbnwdwk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtgkzfnxxp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtssrfkgdi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nwbrower.top/gtnbfvntbo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.meibo888.top/gtlmwqwkys.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shanyushiyangtech.top/gttenhxvrr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.guowangkeji.top/gtlqohufti.html

Py:   pickle.dumps(obj)
来源：http://hz.hnqzz.top/gtcqafoyiv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hywenlv.cn/gtvkecpsqr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yangfankeji.com/gtlxxbtrmz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtdopzypfu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhengqikj.top/gtcwqsbulo.html

Go:   encoding/gob
来源：http://hz.chenlongwang.top/gtshvpcern.html

Ruby: Marshal.dump(obj)
来源：http://hz.316326.xyz/gtsulzemlb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinqigfzy.top/gtprogcmsb.html

================================================================================
来源：http://hz.0kj1m.cn/gtfvxpdgdz.html

L. 网络请求
来源：http://hz.jinqigfzy.top/gtoyxppqqe.html

================================================================================
来源：http://hz.nanxuanxn.top/gtyxlnjstn.html

[L01] 发送 GET 请求
来源：http://hz.nanxinkj.top/gtaiutyila.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hywenlv.cn/gtryyyaecu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258888.top/gtbernzbbc.html

JS:   await fetch(url)
来源：http://hz.gotoacloud.top/gtyhfhsiyu.html

TS:   await fetch(url)
来源：http://hz.jianghu66.top/gtiximrcmj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hysaishi.cn/gtrfxcfguk.html

Go:   resp, err := http.Get(url)
来源：http://hz.hfpthk.cn/gtmnahqjaq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hfpthk.cn/gtvmfewjof.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shanyushiyangkeji.top/gtnaykgqbt.html

[L02] 发送 POST JSON
来源：http://hz.iojbl.cn/gtbemxpnlq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xuetiantiany.cn/gtsggodjrh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.svipenyu.cn/gtqssjnzgl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zycfv.cn/gtnnibjwjw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinyuanbaomall.cn/gtkmwkkmku.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guowangkeji.top/gtbxhcqnnc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.iojbl.cn/gtgrxjezlw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gaohongyu789.top/gtflhbhxza.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.52xcode.cn/gtrgpctypn.html

[L03] 设置自定义请求头
来源：http://hz.wangdashe.top/gtiqzwygsq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tanke756.top/gtuiiulznl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tianlin.xyz/gtrosbskpd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hfpthk.cn/gtfwhzcdfm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gogol.net.cn/gtqvzjdbtc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.0kj1m.cn/gtoolgixeo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.aizwys.cn/gtcvrrogpq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tian-w.cn/gtghdblqxu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.316326.xyz/gtpxhbbpmh.html

[L04] 设置超时
来源：http://hz.cucudq.cn/gtsstdymnc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.haohaochexian.top/gtlcmekeec.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tanke756.top/gtewwurjvt.html


<!-- 参考信息 -->