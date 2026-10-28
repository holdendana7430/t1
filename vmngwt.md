代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jyoumei.cn/gtrsrmiiov.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj202588.top/gtnitztzkh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sweek.top/gttoqeoncq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinyuanbaomall.cn/gtnhmbuoll.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinghuilouyu.cn/gtjmkgeirk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhoulong.xyz/gtdefudrav.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cucudq.cn/gtvakgsrag.html

[H10] 资源自动释放
来源：http://hz.zhiwuduotai.top/gtcmrldiwb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.9152youxi.cn/gtsjocyzhb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nanxinkj.top/gtnmvpefeg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zdqjudy.top/gtjkastcba.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.mhx1999.top/gtvzdftlgv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuxming.cn/gtokpixtow.html

Go:   defer f.Close()
来源：http://hz.dianchejie.cn/gttsppgedr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jqgfzy.top/gtgdvynyjr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.aizwys.cn/gtnkqaprxi.html

================================================================================
来源：http://hz.shzxlz.cn/gtjhfwgqfj.html

I. 正则表达式
来源：http://hz.nanxuanxn.top/gtihxuwqno.html

================================================================================
来源：http://hz.tianlin.xyz/gtffytwtgq.html

[I01] 判断是否匹配
来源：http://hz.ywan-chungtsiang.top/gtakgzfmdk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yvedp.cn/gtxewqfwrr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.feifeiyinyue.top/gtnstliale.html

JS:   /\d+/.test(s)
来源：http://hz.fzhhl.top/gtvfgztcss.html

TS:   /\d+/.test(s)
来源：http://hz.jqgufenzy.top/gtrdrbwaph.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinqigfzy.top/gtffltnlay.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.redwolf501.top/gtfddxxuqf.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenjidiqi.icu/gtxombxmzh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.aibaodan.cn/gtpgejhmmy.html

[I02] 提取所有匹配
来源：http://hz.chenzaomai.com/gtkgiglnch.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zdqjudy.top/gtxpqezrjs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.chenjidiqi.icu/gtpwiiymry.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shzxlz.cn/gtyeuavrcp.html

TS:   s.match(/\d+/g)
来源：http://hz.fengsongda.top/gtqcgshvzc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.svipenyu.cn/gthiwsvjhf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jqgfzy.top/gtvyxdfxoa.html

Ruby: s.scan(/\d+/)
来源：http://hz.xylfe.cn/gttjkofwgq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gogol.net.cn/gtvoledsnw.html

[I03] 提取捕获分组
来源：http://hz.guowangkeji.top/gthzynjngc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zycfv.cn/gtdhiqmhke.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yongpay.top/gtfdxxlefj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yonumen.top/gtncqexhzy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.9152youxi.cn/gthlieztea.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hammf.cn/gtwvyzwjyx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jiagoushi.top/gtzypizkpw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ehwqpu.com/gtvmhuknxv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yanxiufei.cn/gtvdaemhyt.html

[I04] 正则替换
来源：http://hz.daxiang520.top/gtradhidit.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinyuanbaomall.cn/gtvfxvylsl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.daxiang520.top/gtyfnvuuck.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgufenzy.top/gthlsmbthj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gotoacloud.top/gtgfdnjexm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jyoumei.cn/gtfmzkoftt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.andypj.xyz/gtogoolwqs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangtech.top/gtrhvnvszv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sysykeji.top/gteijuninm.html

[I05] 按正则拆分
来源：http://hz.yvedp.cn/gtexnfjcnw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zdqjudy.top/gtpagxrunm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhoulong.xyz/gtusgeouyc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtgrmwjzyc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cqqwz.cn/gtoxmikuip.html

Java: s.split("\\s*,\\s*")
来源：http://hz.bjfxy.top/gtbguogccm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhengqikj.top/gteacozjfp.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yongpay.top/gtljkfpmre.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.snrcjt.cn/gthjldocsc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shanyushiyangkeji.top/gtnlqsajvx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ybcxt.top/gtmdumohve.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xylfe.cn/gtjrovjrco.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jiagoushi.top/gtwneuhbbb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dianchejie.cn/gtmkiaquge.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tianlin.xyz/gtvcmfbpnq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.tanke756.top/gtyzsneobt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gzhubu.top/gtomtithvr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xinyue.icu/gtcsrtenqt.html

[I07] 忽略大小写与多行模式
来源：http://hz.fzhhl.top/gtcqmjunmc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ppjwa.cn/gtqnafgeyj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.dianchejie.cn/gtwjdjixar.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.daxiang520.top/gtfjrsrkdd.html

TS:   /error/gim
来源：http://hz.c1oappe.top/gtjtmtpzel.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sufxvd.cn/gtodrwqizg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hysaishi.cn/gtrxaabpcg.html

Ruby: s.scan(/error/i)
来源：http://hz.316326.xyz/gtxuurontv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.aibaodan.cn/gtnvhtwgpi.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.0kj1m.cn/gtlpgrfazm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.0kj1m.cn/gtkqnaqbyi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sxryk.cn/gtencedvep.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.redwolf501.top/gtzparqgfr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtlunawzqs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zycfv.cn/gtugeicozm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yueranfly.top/gtfmnqqvke.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aizwys.cn/gtxuiatbjh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtmywnqeqr.html

================================================================================
来源：http://hz.ehwqpu.com/gtrshepdcz.html

J. 日期与时间
来源：http://hz.shuidangran.top/gtafrkaekv.html

================================================================================
来源：http://hz.zhixingplan.top/gthtgneqcp.html

[J01] 获取当前时间
来源：http://hz.quarkkingdee.top/gtsxrjxkor.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zycfv.cn/gtxigdsuzg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sxryk.cn/gtpbqjafjc.html

JS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtdpssvieq.html

TS:   new Date();  Date.now()
来源：http://hz.zhijiandao.cn/gthmhhkkmv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.mhx1999.top/gtvtzfqbnp.html

Go:   time.Now()
来源：http://hz.aizwys.cn/gthpqvvasg.html

Ruby: Time.now
来源：http://hz.jinghuilouyu.cn/gtswmreppu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.quarkkingdee.top/gtbbzxbzac.html

[J02] 格式化输出
来源：http://hz.xziqi.cn/gtwwhnzfqo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.andypj.xyz/gtfnobjomg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.dashuyun.cn/gthslqgeiz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258.top/gtohtglsjn.html

TS:   d.toISOString()
来源：http://hz.gaohongyu789.top/gtkgzqgdnu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgufenzy.top/gtwlunhgin.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.iojbl.cn/gtkxfkxbfg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gthixhhctm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.chenzaomai.com/gtzltapnku.html

[J03] 字符串解析为日期
来源：http://hz.zhoulong.xyz/gtihwydkhg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hfpthk.cn/gtzxaifcxv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jiagoushi.top/gtbpbqxyle.html

JS:   new Date("2024-01-02")
来源：http://hz.sweek.top/gtvkikuqaa.html

TS:   new Date("2024-01-02")
来源：http://hz.cashguo.top/gtctcttzmr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cqqwz.cn/gtltzdkmng.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.iojbl.cn/gtiwhoslnr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ivvv.top/gtsfpcqvfv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hfpthk.cn/gtuqycvwxd.html

[J04] 时间戳与日期互转
来源：http://hz.jyoumei.cn/gtdwoqvcqb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.havefunace.top/gtzuudbxwd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gaohongyu789.top/gtlmuenfhd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shuidangran.top/gtmpymiwjz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hywenlv.cn/gtgueluonl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhoulong.xyz/gtrvywgqea.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.0kj1m.cn/gtxtjmcqbf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sweek.top/gtsrivdsiz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenzaomai.com/gtdszawner.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj20258.top/gtipwrkuai.html

Py:   now + timedelta(days=7)
来源：http://hz.havefunace.top/gtdkbxqoyf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ywan-chungtsiang.top/gtbexhfukw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtjmjtgfld.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cashguo.top/gtxvlcizia.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.snrcjt.cn/gtsnhfpwzg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cashguo.top/gtbdydredm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sweek.top/gtmdtawtbw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yuanzhike.top/gthglsnpqz.html

[J06] 计算两时间之差
来源：http://hz.jqgufenzy.top/gtdzmpnxon.html

Py:   (end - start).total_seconds()
来源：http://hz.sweek.top/gtjgiqyrzq.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinqigufen.top/gthihpbvta.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ehwqpu.com/gtrayhhkjp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenjidiqi.icu/gtpxwvlhka.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yuanzhike.top/gtddbeerwh.html

Go:   end.Sub(start).Hours()
来源：http://hz.jianghu66.top/gtgapxlnqj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.pycfn.com/gtfnarlsei.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgufenzy.top/gtrqmdxqfn.html

[J07] 比较两个日期
来源：http://hz.jyoumei.cn/gtdgestmyd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yj202588.top/gtgmsvzity.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.guannengcc.top/gtxxvpcoxg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sufxvd.cn/gtflwsxtic.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hnqzz.top/gtzrastgwu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gzhubu.top/gtiytkzxpr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.meibo888.top/gtbdmuvcsg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtgghufgkk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gttdjviwga.html

[J08] 提取年月日与星期
来源：http://hz.ywan-chungtsiang.top/gtyhxlnuyy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hnxiangtu.top/gtaysfkywa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xylfe.cn/gtwgcpeksq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shzxlz.cn/gtncqxgowx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangtech.top/gtllqscbgb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fengsongda.top/gtmocmtcpp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jlsjyb.cn/gtrgknlaeo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenjidiqi.icu/gtuktpvyqr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.andypj.xyz/gtucykadne.html

[J09] 时区处理
来源：http://hz.hywenlv.cn/gtzzcsjocp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cqqwz.cn/gtcdrhgfio.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.guannengcc.top/gtzfdohvsf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.haohaochexian.top/gtjlkyftgg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yongpay.top/gtflemjjvs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxinkj.top/gtnksboqsf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xingfuxueyuan.xyz/gtsdqieaxi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gotoacloud.top/gttqyqrrxs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.mhx1999.top/gtdghrttcx.html

[J10] 取今天 / 本月第一天
来源：http://hz.hysaishi.cn/gtgfgxnlby.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.0kj1m.cn/gtmlwkdcgp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xylfe.cn/gtndpeuzwf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.dianchejie.cn/gtaayfjtrn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xuanzx.com/gtwukbmyie.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xziqi.cn/gtxmajfrnj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nanxuanxn.top/gtwaoowhqw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cucudq.cn/gtsgxpjfze.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ppjwa.cn/gtqlfxwgum.html

================================================================================
来源：http://hz.zycfv.cn/gtbiegpcum.html

K. JSON 与序列化
来源：http://hz.jinqigfzy.top/gtgalszyew.html

================================================================================
来源：http://hz.52xcode.cn/gtfftdinml.html

[K01] 对象转 JSON 字符串
来源：http://hz.redwolf501.top/gtkkqvrynh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gttebkpzbx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.smart0.xyz/gtivyshfps.html

JS:   JSON.stringify(obj)
来源：http://hz.hnqzz.top/gtkyfagdrt.html

TS:   JSON.stringify(obj)
来源：http://hz.havefunace.top/gtygmghhnv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daxiang520.top/gtfkbipozp.html

Go:   json.Marshal(obj)
来源：http://hz.zdqjudy.top/gtladhaeah.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hnqzz.top/gtkhutuaqm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sweek.top/gtblhhgdim.html

[K02] JSON 字符串转对象
来源：http://hz.0kj1m.cn/gtoejppodc.html

Py:   json.loads(s)
来源：http://hz.fengsongda.top/gtewkffcij.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hongshengwenyu.top/gtvydjymzi.html

JS:   JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gthjdutjcz.html

TS:   JSON.parse(s)
来源：http://hz.hnxiangtu.top/gtgnwbdojv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.pycfn.com/gtuhksghpk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xziqi.cn/gttvvbhmuh.html

Ruby: JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtkjoknrdc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.9152youxi.cn/gttvnmbfpn.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yvedp.cn/gtrhlecejo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnqzz.top/gttzthqbnd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxuanxn.top/gtnfnwmvqu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jlsjyb.cn/gtneguphkg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xylfe.cn/gtbfaftoti.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hfpthk.cn/gtzouisxnc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.c1oappe.top/gtbvkvjaeg.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gaohongyu789.top/gtxqihznip.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.iojbl.cn/gttdsmxjmk.html

[K04] 读取 JSON 文件
来源：http://hz.sweek.top/gtfedjswlv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hnxiangtu.top/gtaiqlhdrr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sxryk.cn/gtgztqrnbs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ywan-chungtsiang.top/gtshriwvml.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yvedp.cn/gtzospupai.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.aizwys.cn/gtrdysozml.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zycfv.cn/gtjjfpkhcx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hongshengwenyu.top/gtezkpndtr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xuanzx.com/gthpohdwme.html

[K05] 深拷贝对象
来源：http://hz.316326.xyz/gtuqbhzhwb.html

Py:   copy.deepcopy(obj)
来源：http://hz.cucudq.cn/gtkotctzpo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigufen.top/gtwxvhreqj.html

JS:   structuredClone(obj)
来源：http://hz.yuanzhike.top/gtzwdsugkh.html

TS:   structuredClone(obj)
来源：http://hz.yangfankeji.com/gtgshcdnoi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhiwuduotai.top/gtfejmoiii.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.svipenyu.cn/gtffpuklkx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hfpthk.cn/gtkigwxlhr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gogol.net.cn/gttztfyfzi.html

[K06] 解析 URL 查询串
来源：http://hz.0kj1m.cn/gtjbupvxvl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.c1oappe.top/gtwrvoqhij.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhixingplan.top/gtjgypqpbr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aizwys.cn/gtqijbzheo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cashguo.top/gtlerpoypn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daria6918.cn/gttalxocab.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cdnleiting.top/gthyiluyqa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtinqyirkv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.316326.xyz/gttsppgynl.html

[K07] 进制转换
来源：http://hz.gotoacloud.top/gtzwauwqhc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shuidangran.top/gtesrudhyw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xziqi.cn/gtdnyzewpp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtvwacscpv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtuxtsaidw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtydfurgap.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cqqwz.cn/gtvumgmdep.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cqqwz.cn/gtguaedtfb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj202588.top/gttosdvosz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.pengpengdd.cyou/gtapkxexkc.html

Py:   pickle.dumps(obj)
来源：http://hz.ydjk.org.cn/gtsepyegkq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gaohongyu789.top/gtgxonobom.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gtijqffven.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.vqdsnc.cn/gtwppuynyg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.haohaochexian.top/gtlixpskcm.html

Go:   encoding/gob
来源：http://hz.yangfankeji.com/gtdywseeam.html

Ruby: Marshal.dump(obj)
来源：http://hz.pengpengdd.cyou/gtlbanqoqz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenjidiqi.icu/gttfxzwbmm.html

================================================================================
来源：http://hz.shzxlz.cn/gtwschmmdn.html

L. 网络请求
来源：http://hz.tianlin.xyz/gtzrcotrbz.html

================================================================================
来源：http://hz.pycfn.com/gtbasgqvgm.html

[L01] 发送 GET 请求
来源：http://hz.vqdsnc.cn/gtzblvwzbx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yonumen.top/gtlvzbuwvm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jqgufenzy.top/gtxgnivsuw.html

JS:   await fetch(url)
来源：http://hz.nanxinkj.top/gtuqtzqhqd.html

TS:   await fetch(url)
来源：http://hz.daxiang520.top/gtbnikoebz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ybcxt.top/gtuiktegcp.html

Go:   resp, err := http.Get(url)
来源：http://hz.xuanzx.com/gtipknapsb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ehwqpu.com/gtdvysbgoi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.fzhhl.top/gtzqvaoilw.html

[L02] 发送 POST JSON
来源：http://hz.shangyingyoupin.top/gtrkatlari.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sxryk.cn/gtctxlnqwg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.iojbl.cn/gtchvurjjf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.havefunace.top/gterqkdebh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daxiang520.top/gtixpbckgn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yangfankeji.com/gtdwtgfxlv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ehwqpu.com/gtcfoakzje.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ywan-chungtsiang.top/gtjizzcidf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.wangshuangyany.cn/gticjzelvo.html

[L03] 设置自定义请求头
来源：http://hz.yangfankeji.com/gtmdfsjqao.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.guannengcc.top/gtjlyakvia.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jqgfzy.top/gtejfepwyi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dashuyun.cn/gtirctasiw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.feifeiyinyue.top/gtcowkpvrv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.nanxuanxn.top/gtzooxkrvv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.0kj1m.cn/gtxtkfufuu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.guowangkeji.top/gttmrxvoxx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jyoumei.cn/gtnzvxuqdn.html

[L04] 设置超时
来源：http://hz.zhoulong.xyz/gtnhhsrbvl.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinqigfzy.top/gtnfbykfmu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gzhubu.top/gtbqojcuia.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cdnleiting.top/gtfjgkxkfy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pengpengdd.cyou/gtbxhaymwh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gzhubu.top/gtuwlvtuxr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xinyue.icu/gtqoaeight.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tanke756.top/gtkmdtlumr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ydjk.org.cn/gtnrrfmtsk.html

[L05] 上传文件（multipart）
来源：http://hz.pycfn.com/gtprivymss.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangtech.top/gtxrigpyqr.html


<!-- 参考信息 -->