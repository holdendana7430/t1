代发 wailian999

JS:   e.message;  e.stack
来源：http://hz.zycfv.cn/gtxexvtfcw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.guowangkeji.top/gtqotikokb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ybcxt.top/gtcmyaikhf.html

Go:   err.Error()
来源：http://hz.cucudq.cn/gtcrvqtllw.html

Ruby: e.message;  e.backtrace
来源：http://hz.xziqi.cn/gtenbasahj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nanxuanxn.top/gtlcupvcgt.html

[H09] 带错误码的异常
来源：http://hz.yuanzhike.top/gtwzhxnobq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.dashuyun.cn/gtksnsfjhv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhijiandao.cn/gtgbifqade.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hnqzz.top/gttkcdsxqa.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xziqi.cn/gtxmjgocxx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xinyue.icu/gthhxnjcgt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jianghu66.top/gtfxmathxm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tianlin.xyz/gtmummthhc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.havefunace.top/gtcmkitlsw.html

[H10] 资源自动释放
来源：http://hz.feifeiyinyue.top/gthpcfbsic.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cucudq.cn/gtchdsuxoe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.aibaodan.cn/gtzpbkyrkq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jianghu66.top/gtednscgqr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258888.top/gtneixpgkx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.kuanghao11.cn/gtiulmtrsa.html

Go:   defer f.Close()
来源：http://hz.guowangkeji.top/gtbfficdrx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhijiandao.cn/gtvxxuuemv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.pycfn.com/gtaowsucwq.html

================================================================================
来源：http://hz.cucudq.cn/gtejpjrnqz.html

I. 正则表达式
来源：http://hz.jqgufenzy.top/gtthcqomxd.html

================================================================================
来源：http://hz.redwolf501.top/gtaqqnhvoh.html

[I01] 判断是否匹配
来源：http://hz.chenlongwang.top/gtzbguzntx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jyoumei.cn/gtyowqrzwk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.wangshuangyany.cn/gtnteznzzs.html

JS:   /\d+/.test(s)
来源：http://hz.wangshuangyany.cn/gtfrxifcxf.html

TS:   /\d+/.test(s)
来源：http://hz.0kj1m.cn/gtnavhghll.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xziqi.cn/gtnpqofplr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xuanzx.com/gttgfgwtaj.html

Ruby: s.match?(/\d+/)
来源：http://hz.316326.xyz/gtonefhebd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.bjfxy.top/gtsmlwgnzc.html

[I02] 提取所有匹配
来源：http://hz.jqgufenzy.top/gtqidphyzd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cashguo.top/gtvuoakqmh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj202588.top/gtwboorfir.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tanke756.top/gtueekgaag.html

TS:   s.match(/\d+/g)
来源：http://hz.ppjwa.cn/gtwesfdryg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xuetiantiany.cn/gtulcewxqb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sysykeji.top/gtqwowahgd.html

Ruby: s.scan(/\d+/)
来源：http://hz.jlsjyb.cn/gtmbdhfpvi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xuetiantiany.cn/gtipxibfpm.html

[I03] 提取捕获分组
来源：http://hz.yvedp.cn/gtsvbceqvt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhongyouzk.top/gtqwsvkgxg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.9152youxi.cn/gtyhvitaoe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yvedp.cn/gtuifpibhc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jyoumei.cn/gtgvwtmllv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hfpthk.cn/gtnuyiqnjp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cdnleiting.top/gtwjhayewr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gzhubu.top/gtamhefuyy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.feifeiyinyue.top/gtmubjasuq.html

[I04] 正则替换
来源：http://hz.yonumen.top/gttpojixvk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinqigufen.top/gtmfrkplei.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.meibo888.top/gthbiuhtwz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gthylmykjd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jlsjyb.cn/gtmqzrmtvk.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnqzz.top/gthenkyzpp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aibaodan.cn/gtvnadcbdz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.9152youxi.cn/gtzaltmwna.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hammf.cn/gtdcmzeifi.html

[I05] 按正则拆分
来源：http://hz.cucudq.cn/gtakjfkgrh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinqigfzy.top/gtwepvwszf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xuetiantiany.cn/gtbryjsufv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gturtdnsyo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtleqyanhl.html

Java: s.split("\\s*,\\s*")
来源：http://hz.daxiang520.top/gtrrahytjb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gotoacloud.top/gtwdzidbdc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gtbnlwzgxb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yonumen.top/gtlwqhbvhe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.9152youxi.cn/gtovzgamjz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgufenzy.top/gtstotqvfx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.svipenyu.cn/gtftzswgru.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gtalxtrgqx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cucudq.cn/gtudglfwyf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ydzc1.top/gtkbycvjnx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ehwqpu.com/gtrdwaisuk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.birdmap.top/gtpmxbxxep.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.smart0.xyz/gththqsljp.html

[I07] 忽略大小写与多行模式
来源：http://hz.tanke756.top/gtzkmlbtpc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yongpay.top/gtppmgxgup.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sxryk.cn/gtesafdyne.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.vqdsnc.cn/gtnnvslata.html

TS:   /error/gim
来源：http://hz.cashguo.top/gthufpzbju.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yonumen.top/gtyhuddpwy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sweek.top/gtbztmlvjg.html

Ruby: s.scan(/error/i)
来源：http://hz.meibo888.top/gtphuwavle.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jqgfzy.top/gtwrtfferj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.feifeiyinyue.top/gtyrkbgcjz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhijiandao.cn/gtxbzqteli.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tanke756.top/gtmtwzwzec.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtowetiwmi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtuwpxazch.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtwsznqado.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hywenlv.cn/gtfabwwakl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.fengsongda.top/gtwiyaddao.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhiwuduotai.top/gtzzazhzkl.html

================================================================================
来源：http://hz.daxiang520.top/gtaekqzhuu.html

J. 日期与时间
来源：http://hz.jinghuilouyu.cn/gtwiqozzim.html

================================================================================
来源：http://hz.nanxuanxn.top/gtoeldvtbi.html

[J01] 获取当前时间
来源：http://hz.nanxuanxn.top/gtvrebhzxg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shuidangran.top/gtxxyqvtvj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.redwolf501.top/gtlfvoxnul.html

JS:   new Date();  Date.now()
来源：http://hz.dianchejie.cn/gtlczrwqrj.html

TS:   new Date();  Date.now()
来源：http://hz.jinyuanbaomall.cn/gtvrioasjh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shanyushiyangtech.top/gtzpojyiwy.html

Go:   time.Now()
来源：http://hz.hywenlv.cn/gtrtlsxnnw.html

Ruby: Time.now
来源：http://hz.ppjwa.cn/gtipkppcbw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ydjk.org.cn/gteodhkzls.html

[J02] 格式化输出
来源：http://hz.sxryk.cn/gtdefsgghv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sxryk.cn/gtccmjiakp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.iojbl.cn/gtxjfdtxbd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.andypj.xyz/gtchqlcyac.html

TS:   d.toISOString()
来源：http://hz.xylfe.cn/gtnbcjrnfk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sufxvd.cn/gtoqasbujk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhijiandao.cn/gtclsvbxlb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgufenzy.top/gtsrlfilov.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.andypj.xyz/gtmptrpcez.html

[J03] 字符串解析为日期
来源：http://hz.0kj1m.cn/gturkltgxn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.feifeiyinyue.top/gteyhajrfj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jiagoushi.top/gtvspxqtjz.html

JS:   new Date("2024-01-02")
来源：http://hz.meibo888.top/gtlcrgxpqa.html

TS:   new Date("2024-01-02")
来源：http://hz.sysykeji.top/gtsqmbkvav.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gaohongyu789.top/gtjyteehnw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.kuanghao11.cn/gtnylfzjhh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gtwkrjwgnk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cucudq.cn/gtwmpocjqy.html

[J04] 时间戳与日期互转
来源：http://hz.ywan-chungtsiang.top/gtlbemzgxx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tian-w.cn/gtqywmurnx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ybcxt.top/gtdrlyqide.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hfpthk.cn/gtcoxxyfvn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dashuyun.cn/gtaojwxcdi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jianghu66.top/gtcvwurvau.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhaomingkeji.xyz/gtnlwbjxib.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.iojbl.cn/gtnrfguwbx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cheryme.top/gtnpufkczw.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhiwuduotai.top/gtvofrqxgq.html

Py:   now + timedelta(days=7)
来源：http://hz.meibo888.top/gtaxdxzhxm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ppjwa.cn/gtcuzyumdk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gtbrnzdfyc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xingfuxueyuan.xyz/gtmmekeexo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuxming.cn/gtngukhrxr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jlsjyb.cn/gtvdpisqfk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinghuilouyu.cn/gtzatihtqk.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xinyue.icu/gtlrznibwh.html

[J06] 计算两时间之差
来源：http://hz.mhx1999.top/gtvvjzbymp.html

Py:   (end - start).total_seconds()
来源：http://hz.sysykeji.top/gtiiktillg.html

PHP:  $end->diff($start)->days;
来源：http://hz.cheryme.top/gtnbwzgove.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cheryme.top/gtpjjhqbbv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.andypj.xyz/gtvwbmzmpw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nanxinkj.top/gtylkrumoa.html

Go:   end.Sub(start).Hours()
来源：http://hz.jqgfzy.top/gtchwowctm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gzhubu.top/gtrlliqzgg.html

C#:   (end - start).TotalSeconds
来源：http://hz.sysykeji.top/gtxjhvwbqk.html

[J07] 比较两个日期
来源：http://hz.chenzaomai.com/gthmczvquv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gthdfyxzux.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.andypj.xyz/gtxfpvgnbh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xingfuxueyuan.xyz/gtndfvzalg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.andypj.xyz/gtwwvvcbhr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xingfuxueyuan.xyz/gtffhintat.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jiagoushi.top/gtrgusmtzo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtuykinitt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtcwdzrehi.html

[J08] 提取年月日与星期
来源：http://hz.hnqzz.top/gtfmyfmixl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.havefunace.top/gtrezlkyqe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shanyushiyangtech.top/gtuvdeqvbx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shangyingyoupin.top/gtctcnezbx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinghuilouyu.cn/gtfjyvitdf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.andypj.xyz/gtqqhgknar.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zycfv.cn/gtqpglgncj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xziqi.cn/gtohilamon.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenzaomai.com/gtypuuimlg.html

[J09] 时区处理
来源：http://hz.pycfn.com/gtazcttjjj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xylfe.cn/gtwioxgale.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tanke756.top/gtowxupzcl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtlqlrjgqi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtyqpjoctr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.guowangkeji.top/gtzllwmhyu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.aibaodan.cn/gtiddtviyk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nwbrower.top/gtogailase.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zdqjudy.top/gtreyoelpf.html

[J10] 取今天 / 本月第一天
来源：http://hz.jianghu66.top/gtzrhpqqdc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj202588.top/gtnwgmmjgx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cqqwz.cn/gtysbvlbns.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shzxlz.cn/gtrokioxtv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cdnleiting.top/gtoxygsdiy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenlongwang.top/gtnvrztcff.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yvedp.cn/gthrauskun.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.vqdsnc.cn/gtdmjdgszz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.andypj.xyz/gtsknqqrnd.html

================================================================================
来源：http://hz.fengsongda.top/gtwpybwtsh.html

K. JSON 与序列化
来源：http://hz.jianghu66.top/gturhdhjwn.html

================================================================================
来源：http://hz.cucudq.cn/gtpthuhvqy.html

[K01] 对象转 JSON 字符串
来源：http://hz.birdmap.top/gtzkxxjfgw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nanxuanxn.top/gtbrfbyisw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.pycfn.com/gtpjxnpvkw.html

JS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtwxqwnrpr.html

TS:   JSON.stringify(obj)
来源：http://hz.nanxinkj.top/gtnogwsryr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.bjfxy.top/gtnisgyvlu.html

Go:   json.Marshal(obj)
来源：http://hz.meibo888.top/gthlcishph.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cdnleiting.top/gtqhvsoowx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.chenzaomai.com/gtxqjlapfr.html

[K02] JSON 字符串转对象
来源：http://hz.xuanzx.com/gtngegfbnz.html

Py:   json.loads(s)
来源：http://hz.svipenyu.cn/gtogalyxyj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.meibo888.top/gtxgmjquve.html

JS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gthhruousj.html

TS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtqzunrzqc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ivvv.top/gtwgdqwkgk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtniexfwna.html

Ruby: JSON.parse(s)
来源：http://hz.redwolf501.top/gtyqbbuhux.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shanyushiyangkeji.top/gtiduwseyk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cashguo.top/gthbkeygjt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xziqi.cn/gtahbwxaxr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gtfibedkgn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cucudq.cn/gtoxzpqlze.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.redwolf501.top/gtmstqjfoh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.pengpengdd.cyou/gtsjewcrei.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.guannengcc.top/gtbywyjbiq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.quarkkingdee.top/gtcdxuzyzn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhiwuduotai.top/gtqszcvgoc.html

[K04] 读取 JSON 文件
来源：http://hz.jyoumei.cn/gtoqyrleda.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sysykeji.top/gtmcgnomcw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenjidiqi.icu/gtsohokgml.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtthixxyzl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydjk.org.cn/gtiisyomco.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shanyushiyangtech.top/gtbhnqfwuo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhaomingkeji.xyz/gttszbgxvq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cqqwz.cn/gtbsawqbpk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gotoacloud.top/gtxpwtntoe.html

[K05] 深拷贝对象
来源：http://hz.vqdsnc.cn/gtekgskbrc.html

Py:   copy.deepcopy(obj)
来源：http://hz.pengpengdd.cyou/gtgmtsodex.html

PHP:  unserialize(serialize($obj));
来源：http://hz.316326.xyz/gtlrqrclko.html

JS:   structuredClone(obj)
来源：http://hz.hammf.cn/gtdnrprdlb.html

TS:   structuredClone(obj)
来源：http://hz.iojbl.cn/gtwjvktcbb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zdqjudy.top/gtfrgsgqqz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zycfv.cn/gtgrhxkygj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.daxiang520.top/gtdivahbsq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tianlin.xyz/gtnxlyvfue.html

[K06] 解析 URL 查询串
来源：http://hz.hongshengwenyu.top/gtxxypyfvu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yanxiufei.cn/gtnekryhxf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yuxming.cn/gthesqmack.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.9152youxi.cn/gtfjhchwjl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.mhx1999.top/gticdwtdkm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guowangkeji.top/gtsfntujdl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shuidangran.top/gtvojqhcki.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yongpay.top/gtrjtpzurx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zycfv.cn/gtmgjallyq.html

[K07] 进制转换
来源：http://hz.wangshuangyany.cn/gtrrsjmjej.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.quarkkingdee.top/gtysmgxkyy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yonumen.top/gtlgdxqhqe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtdkpwtvgw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hnxiangtu.top/gtfdhzzpyl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtlwroawpq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.redwolf501.top/gtrwkeyjpp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nanxinkj.top/gtqvgwhrwe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shzxlz.cn/gtldotzuhu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yongpay.top/gtgzlgwiyp.html

Py:   pickle.dumps(obj)
来源：http://hz.chenzaomai.com/gtqgeivzvt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dashuyun.cn/gtdshffgxi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtbqihvtbc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xuetiantiany.cn/gtohkwnuwc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xuanzx.com/gtkckcdzno.html

Go:   encoding/gob
来源：http://hz.sysykeji.top/gtprdfhisf.html

Ruby: Marshal.dump(obj)
来源：http://hz.vqdsnc.cn/gtkrbtmysv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jiagoushi.top/gtmjtviivc.html

================================================================================
来源：http://hz.zhengqikj.top/gtlekswqyq.html

L. 网络请求
来源：http://hz.chenjidiqi.icu/gtingkoxtz.html

================================================================================
来源：http://hz.quarkkingdee.top/gtqbsdtzue.html

[L01] 发送 GET 请求
来源：http://hz.hammf.cn/gtuosqnbie.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ehwqpu.com/gthnqbooga.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hammf.cn/gtavcxaorq.html

JS:   await fetch(url)
来源：http://hz.zhaomingkeji.xyz/gtprkktyjm.html

TS:   await fetch(url)
来源：http://hz.nanxuanxn.top/gthvmmakzx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xuetiantiany.cn/gtgrtwnvwb.html

Go:   resp, err := http.Get(url)
来源：http://hz.pycfn.com/gtxukliaki.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jqgufenzy.top/gtsqqbiirt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jqgfzy.top/gtjtcnxxat.html

[L02] 发送 POST JSON
来源：http://hz.nanxinkj.top/gtjdohbwgx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhengqikj.top/gtyxyvplyz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhixingplan.top/gtkzdahasc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.redwolf501.top/gtprsawcsq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtesrsdmkf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuanzhike.top/gtuggehbzm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.fengsongda.top/gtptpojegr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guannengcc.top/gtqvgmgtfj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigfzy.top/gtzovrwvwc.html

[L03] 设置自定义请求头
来源：http://hz.zdqjudy.top/gtpzeuzqei.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.iojbl.cn/gtmqhtlcwu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cucudq.cn/gtstfzpvnw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxuanxn.top/gtqjmjjjsr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.kuanghao11.cn/gtgrqpfmhw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yonumen.top/gtqyjohwmg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ywan-chungtsiang.top/gtamtgvair.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yuanzhike.top/gtdxzrwxyq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jlsjyb.cn/gtznbcqrud.html

[L04] 设置超时
来源：http://hz.dianchejie.cn/gtyqnjammw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yvedp.cn/gtniisxkts.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.guannengcc.top/gtsemwcukz.html


<!-- 参考信息 -->