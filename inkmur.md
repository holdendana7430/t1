代发 wailian999

JS:   e.message;  e.stack
来源：http://hz.chenzaomai.com/gtvokcgjxu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ydzc1.top/gtachrxdom.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zdqjudy.top/gtwhimkxdk.html

Go:   err.Error()
来源：http://hz.haohaochexian.top/gtxpdhclag.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinyuanbaomall.cn/gtkygtzyjc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xylfe.cn/gtyegdxeba.html

[H09] 带错误码的异常
来源：http://hz.redwolf501.top/gtsopsalxq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nwbrower.top/gtnifpsejq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sysykeji.top/gtdimxkxgm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.c1oappe.top/gtfxcpzzft.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj202588.top/gtfutfocqc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yongpay.top/gthpxzmniw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nanxinkj.top/gtrkidkpsq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yangfankeji.com/gtbtrlbedx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.snrcjt.cn/gtulhwruap.html

[H10] 资源自动释放
来源：http://hz.nanxuanxn.top/gtsjaflqxp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.mhx1999.top/gtingigvyt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xingfuxueyuan.xyz/gtscaisung.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuanzx.com/gtzdeorqfy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cdnleiting.top/gtwoshabej.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhoulong.xyz/gtdcjuoznb.html

Go:   defer f.Close()
来源：http://hz.yj202588.top/gtszeityxl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.redwolf501.top/gtamtngwkv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hongshengwenyu.top/gtcaksphmo.html

================================================================================
来源：http://hz.zhengqikj.top/gtzyayzhrt.html

I. 正则表达式
来源：http://hz.jinyuanbaomall.cn/gttfbjuesc.html

================================================================================
来源：http://hz.andypj.xyz/gtggpuobrx.html

[I01] 判断是否匹配
来源：http://hz.fengsongda.top/gtygvtwcng.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenjidiqi.icu/gtvvdkxvfz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sufxvd.cn/gtlafvaljp.html

JS:   /\d+/.test(s)
来源：http://hz.chenzaomai.com/gtycvrgrbl.html

TS:   /\d+/.test(s)
来源：http://hz.guannengcc.top/gtwxvlihin.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yuxming.cn/gtuegljlap.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jlsjyb.cn/gtvqxexrni.html

Ruby: s.match?(/\d+/)
来源：http://hz.zycfv.cn/gtodsmkaol.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangdashe.top/gtsrlmooxg.html

[I02] 提取所有匹配
来源：http://hz.tianlin.xyz/gtkffhrbbb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yangfankeji.com/gtnkaiyogo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xziqi.cn/gtcvyzlzha.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.vqdsnc.cn/gtnbtoncxz.html

TS:   s.match(/\d+/g)
来源：http://hz.chenlongwang.top/gtvnpjnjlx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhengqikj.top/gtotgsijqz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xuanzx.com/gtdeohpzku.html

Ruby: s.scan(/\d+/)
来源：http://hz.xziqi.cn/gtwvqjmxmj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.quarkkingdee.top/gtxrwdurig.html

[I03] 提取捕获分组
来源：http://hz.tianlin.xyz/gtqcquzuys.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jqgufenzy.top/gtteidxyyf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.havefunace.top/gtescrbxlv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.kuanghao11.cn/gtbaejcelp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cucudq.cn/gtyfiyinsr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.wangshuangyany.cn/gtbzgqbaxs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.daria6918.cn/gtjtvxnpjj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zycfv.cn/gtblaubeeo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cashguo.top/gtvmbrlgrf.html

[I04] 正则替换
来源：http://hz.sufxvd.cn/gtrgcxkuvx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xylfe.cn/gtaywqhvwg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.snrcjt.cn/gtiwcemmob.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.guannengcc.top/gtzrpurqjm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.vqdsnc.cn/gtbhymrxea.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shanyushiyangkeji.top/gtcrovdrbq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhiwuduotai.top/gtiqwjzhdq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.52xcode.cn/gtsoajqyoh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.guowangkeji.top/gtugnwlaph.html

[I05] 按正则拆分
来源：http://hz.snrcjt.cn/gtpbjavswh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.vqdsnc.cn/gtbnhdivlx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yj202588.top/gtutcakbie.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtooltaleo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtvogojpce.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gaohongyu789.top/gtmzfxghqc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tian-w.cn/gtlodnftlt.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yanxiufei.cn/gthuumavjv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinqigufen.top/gtykbouztu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhiwuduotai.top/gtcbluynvt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinghuilouyu.cn/gttoljvexm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.andypj.xyz/gtopardxwt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenjidiqi.icu/gtiojgvtcw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jlsjyb.cn/gtvaknxrdd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.haohaochexian.top/gtnlhwagwj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinyuanbaomall.cn/gtkucmdypd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sysykeji.top/gtqliuysce.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gtrklmptko.html

[I07] 忽略大小写与多行模式
来源：http://hz.tian-w.cn/gtkzjbnpno.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.chenlongwang.top/gtejpwasak.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hysaishi.cn/gtrwviyxea.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ivvv.top/gtkbyohabs.html

TS:   /error/gim
来源：http://hz.haohaochexian.top/gtevldrvsz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.guowangkeji.top/gtjfgdmuve.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shuidangran.top/gtnucdpgix.html

Ruby: s.scan(/error/i)
来源：http://hz.yanxiufei.cn/gtwcezbotl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zycfv.cn/gtmyendtph.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.havefunace.top/gtrskjfjin.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cqqwz.cn/gteyqqawfv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hammf.cn/gtidomwtdw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj202588.top/gtzsweycpq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgfzy.top/gtqxwwjwpy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtwhqmegff.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xinyue.icu/gtwhliysix.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yongpay.top/gtexlcobuq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yongpay.top/gtffxjnarv.html

================================================================================
来源：http://hz.gaohongyu789.top/gtxdxuhgld.html

J. 日期与时间
来源：http://hz.jianghu66.top/gtqgyryync.html

================================================================================
来源：http://hz.tanke756.top/gtolicxxww.html

[J01] 获取当前时间
来源：http://hz.vqdsnc.cn/gtudxedldb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yuxming.cn/gtlqeokfjr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hammf.cn/gtkqhyuors.html

JS:   new Date();  Date.now()
来源：http://hz.jqgufenzy.top/gtqnwfhlqs.html

TS:   new Date();  Date.now()
来源：http://hz.52xcode.cn/gtikbkgfvk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cashguo.top/gtegaetzqk.html

Go:   time.Now()
来源：http://hz.bjfxy.top/gtmbabliwb.html

Ruby: Time.now
来源：http://hz.bjfxy.top/gtdtueunks.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jianghu66.top/gtubxaklrb.html

[J02] 格式化输出
来源：http://hz.shzxlz.cn/gtnhxfvhhe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gtzkrjnldf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xziqi.cn/gtiekwifnp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ydzc1.top/gtnbohwcir.html

TS:   d.toISOString()
来源：http://hz.hammf.cn/gtdfsumink.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhixingplan.top/gtrxfssbip.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yj202588.top/gtgrhgjgzo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtqthcepap.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sysykeji.top/gtmhmuneko.html

[J03] 字符串解析为日期
来源：http://hz.hywenlv.cn/gtneshincy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.meibo888.top/gtmvknmbth.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xylfe.cn/gtserlgusc.html

JS:   new Date("2024-01-02")
来源：http://hz.sxryk.cn/gtjgpcokxp.html

TS:   new Date("2024-01-02")
来源：http://hz.hongshengwenyu.top/gteulccspm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.pycfn.com/gthqlzsxsf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.meibo888.top/gtwftjjdbm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gaohongyu789.top/gtdgxqhzid.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.9152youxi.cn/gtdarywvnm.html

[J04] 时间戳与日期互转
来源：http://hz.sufxvd.cn/gtxnupxraw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xingfuxueyuan.xyz/gtqqagqsug.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nanxinkj.top/gtntnuntzp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xuanzx.com/gtuxikxujq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.quarkkingdee.top/gttsmzahfg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.feifeiyinyue.top/gtywyihseu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.chenjidiqi.icu/gtubeckxkb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.redwolf501.top/gtpfcsnabx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hywenlv.cn/gtcalihouc.html

[J05] 时间加减（加 7 天）
来源：http://hz.andypj.xyz/gttrkivmpa.html

Py:   now + timedelta(days=7)
来源：http://hz.havefunace.top/gtbwgiblwj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.vqdsnc.cn/gtsizotxda.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.redwolf501.top/gtzcswhxxm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.316326.xyz/gtywfslylh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gotoacloud.top/gtggqyjcoi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yangfankeji.com/gtdwgunqpr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.snrcjt.cn/gtksnymfdq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ybcxt.top/gttzmivlqb.html

[J06] 计算两时间之差
来源：http://hz.hnxiangtu.top/gtgmnmdgng.html

Py:   (end - start).total_seconds()
来源：http://hz.xuanzx.com/gtbunbnaon.html

PHP:  $end->diff($start)->days;
来源：http://hz.ywan-chungtsiang.top/gtisksebrd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hnqzz.top/gtumnxrngw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhijiandao.cn/gtgkzugtyd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cheryme.top/gteeoemerd.html

Go:   end.Sub(start).Hours()
来源：http://hz.c1oappe.top/gtzlfssasy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gaohongyu789.top/gtlldmmpvm.html

C#:   (end - start).TotalSeconds
来源：http://hz.sufxvd.cn/gtrdzttevh.html

[J07] 比较两个日期
来源：http://hz.nanxinkj.top/gtqzvseflx.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtouotujii.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.quarkkingdee.top/gtrhrydfll.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tianlin.xyz/gthxqunmvn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gtzlmnhwbn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxuanxn.top/gtpyihkbwy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yuxming.cn/gtojlhkjvr.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtqfsoofvd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gtjdgogkyg.html

[J08] 提取年月日与星期
来源：http://hz.wangshuangyany.cn/gtotbydfcm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.birdmap.top/gtxbjyxwqx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.c1oappe.top/gtyvqmdgmh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jlsjyb.cn/gtldwgpcrl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yuanzhike.top/gtcdigfwxj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.dashuyun.cn/gtlgbimedh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhixingplan.top/gtttsnnvvp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yuanzhike.top/gtgskfqema.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daxiang520.top/gtzafkszdu.html

[J09] 时区处理
来源：http://hz.cqqwz.cn/gtxtxhoucm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jiagoushi.top/gtwxuhuzju.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.fengsongda.top/gtypmwntrr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.feifeiyinyue.top/gtuqtbdilh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pycfn.com/gtkermmebb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhijiandao.cn/gtwslkfssr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hfpthk.cn/gtntqwikih.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sysykeji.top/gtulqojxop.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jlsjyb.cn/gtjnsaoosm.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinyuanbaomall.cn/gtavhhpedw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinghuilouyu.cn/gtpagwdlis.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yuanzhike.top/gtejthyunh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.9152youxi.cn/gttbaadjjy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhaomingkeji.xyz/gttfnbojoh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cheryme.top/gthhanvhws.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhongyouzk.top/gtsuyxncgn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.dianchejie.cn/gtiuxglveb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xylfe.cn/gthphonczq.html

================================================================================
来源：http://hz.cucudq.cn/gtgucctztv.html

K. JSON 与序列化
来源：http://hz.gotoacloud.top/gtblbxascv.html

================================================================================
来源：http://hz.quarkkingdee.top/gtzmvvqybr.html

[K01] 对象转 JSON 字符串
来源：http://hz.ywan-chungtsiang.top/gtcbzrqidj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenzaomai.com/gtpjilognm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sysykeji.top/gtbqdqzdxa.html

JS:   JSON.stringify(obj)
来源：http://hz.gzhubu.top/gtokwwgntj.html

TS:   JSON.stringify(obj)
来源：http://hz.zhiwuduotai.top/gtskrdlcni.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj202588.top/gtmmniytqt.html

Go:   json.Marshal(obj)
来源：http://hz.quarkkingdee.top/gtvynafcdd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.smart0.xyz/gtmpmwhcbx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nanxuanxn.top/gtuyzouuir.html

[K02] JSON 字符串转对象
来源：http://hz.bjfxy.top/gtkrsnxhps.html

Py:   json.loads(s)
来源：http://hz.zdqjudy.top/gttpylwgdx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.andypj.xyz/gtrjsvdtlb.html

JS:   JSON.parse(s)
来源：http://hz.yvedp.cn/gthphnbplz.html

TS:   JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtkpolbqif.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.quarkkingdee.top/gthohwsnyu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hammf.cn/gtaxcjxmpk.html

Ruby: JSON.parse(s)
来源：http://hz.yj20258888.top/gtstxhndqg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.quarkkingdee.top/gtntsxebdk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.iojbl.cn/gtkpaqaumy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xuetiantiany.cn/gtpubqbldq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtkbghqrbu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jianghu66.top/gtchfvsnsq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydzc1.top/gtzkajnmnl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.vqdsnc.cn/gtexlskgva.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nanxuanxn.top/gtljfmuziz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydzc1.top/gtazpyfsyq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhengqikj.top/gtctolmdwl.html

[K04] 读取 JSON 文件
来源：http://hz.sufxvd.cn/gtalkpnbxw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sxryk.cn/gtqytgumxc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenjidiqi.icu/gtxvkavkvv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gaohongyu789.top/gthswegngm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yonumen.top/gtktqrbfkx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangdashe.top/gtpcpkypkf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.daria6918.cn/gtmidbwqbw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.0kj1m.cn/gtltgilqok.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yongpay.top/gtjuimhlel.html

[K05] 深拷贝对象
来源：http://hz.xingfuxueyuan.xyz/gtjqosukhd.html

Py:   copy.deepcopy(obj)
来源：http://hz.shuidangran.top/gtaapnjtgs.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jqgufenzy.top/gtxxgnzhfz.html

JS:   structuredClone(obj)
来源：http://hz.gotoacloud.top/gtdjtisloa.html

TS:   structuredClone(obj)
来源：http://hz.tian-w.cn/gtogkkpezx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jqgufenzy.top/gtvinrgeor.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gaohongyu789.top/gtxsdjdshd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sweek.top/gtgfymtfmj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj20258888.top/gtveqocqxd.html

[K06] 解析 URL 查询串
来源：http://hz.yj20258888.top/gtvquomtdu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ppjwa.cn/gtkhiojzzi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.daxiang520.top/gtjtplqkij.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.316326.xyz/gtbzxmbcun.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuanzhike.top/gtyjebvehw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.havefunace.top/gtstvfmcor.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtampzuzwx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xingfuxueyuan.xyz/gtdtzsjird.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.wangdashe.top/gtnqyuwdey.html

[K07] 进制转换
来源：http://hz.zhijiandao.cn/gtkbmrpdio.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.birdmap.top/gtwftepbot.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ppjwa.cn/gtuqzgcxig.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.52xcode.cn/gtogntlfuu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtuevmjsfn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtmecjdhyi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinyuanbaomall.cn/gtzqmgdrgb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jyoumei.cn/gthwormqvd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xinyue.icu/gtrezlddsj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.c1oappe.top/gtgtniytvv.html

Py:   pickle.dumps(obj)
来源：http://hz.smart0.xyz/gtjavadmma.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xingfuxueyuan.xyz/gtfglvxozq.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtdznjmcrt.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cucudq.cn/gtjsnjbibn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.daria6918.cn/gtkksbzpow.html

Go:   encoding/gob
来源：http://hz.fengsongda.top/gtheyjddnr.html

Ruby: Marshal.dump(obj)
来源：http://hz.sufxvd.cn/gtzksnudvi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.aibaodan.cn/gtyvovrxtu.html

================================================================================
来源：http://hz.gotoacloud.top/gttcsrxwbl.html

L. 网络请求
来源：http://hz.jlsjyb.cn/gtjimzpnhs.html

================================================================================
来源：http://hz.shzxlz.cn/gtellbkeqg.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangtech.top/gtafoozltp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhongyouzk.top/gtnlrytpzz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yonumen.top/gtsttbmehn.html

JS:   await fetch(url)
来源：http://hz.gotoacloud.top/gtxngqksnn.html

TS:   await fetch(url)
来源：http://hz.shzxlz.cn/gtktstapse.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gogol.net.cn/gtqrjckamu.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhengqikj.top/gtsyezuhjh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ydjk.org.cn/gtizbzuzyr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.daria6918.cn/gtwkwgubsx.html

[L02] 发送 POST JSON
来源：http://hz.gogol.net.cn/gtceumuabh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hfpthk.cn/gtpuuxdaex.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhaomingkeji.xyz/gttuevppvw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guannengcc.top/gtxjqftfau.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daxiang520.top/gtcvgeklya.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hywenlv.cn/gtktmuidcv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.bjfxy.top/gtghwuhspd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.redwolf501.top/gtprhykmxc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hywenlv.cn/gtknetsclp.html

[L03] 设置自定义请求头
来源：http://hz.hammf.cn/gtdoxakobd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigfzy.top/gtzcoxycns.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xziqi.cn/gtrifegaqo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jianghu66.top/gtvbqukcox.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cucudq.cn/gtactphkwn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.c1oappe.top/gtbjnnosvj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenjidiqi.icu/gtpxgewqwq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhiwuduotai.top/gtjdmqkhee.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yanxiufei.cn/gtwtqgxpud.html

[L04] 设置超时
来源：http://hz.aizwys.cn/gtsezhhdlx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhoulong.xyz/gtwqudonhm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pycfn.com/gttzsnwyon.html


<!-- 参考信息 -->