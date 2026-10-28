代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://hz.jinqigufen.top/gtqlxormba.html

[H08] 获取错误信息与堆栈
来源：http://hz.jqgfzy.top/gtbhqhvcpu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhaomingkeji.xyz/gtgbjaqxip.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhixingplan.top/gtfdgakinm.html

JS:   e.message;  e.stack
来源：http://hz.52xcode.cn/gtcpidbowe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.andypj.xyz/gtxakczbpq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yonumen.top/gtngzkbrpp.html

Go:   err.Error()
来源：http://hz.zdqjudy.top/gtznxazjrk.html

Ruby: e.message;  e.backtrace
来源：http://hz.xuetiantiany.cn/gthlsiddtr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xylfe.cn/gtyqydsvtj.html

[H09] 带错误码的异常
来源：http://hz.birdmap.top/gtrgmnnjuv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gotoacloud.top/gtdpuntrny.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tianlin.xyz/gtppfzeanm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jqgufenzy.top/gtyvokurxi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gogol.net.cn/gtilqlxkij.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cqqwz.cn/gtmwghnrix.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nanxuanxn.top/gthwmukzmo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hongshengwenyu.top/gtcpiqnmoj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shzxlz.cn/gtzsroowln.html

[H10] 资源自动释放
来源：http://hz.kuanghao11.cn/gtjhjsheut.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zycfv.cn/gtdjlmogpt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258.top/gtlwwdhqve.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hfpthk.cn/gtpgyyrcjb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgufenzy.top/gtgpvjpune.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zycfv.cn/gtgtkojroa.html

Go:   defer f.Close()
来源：http://hz.smart0.xyz/gtbfgwrzci.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.chenjidiqi.icu/gtssxyffir.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinghuilouyu.cn/gtifizkxpx.html

================================================================================
来源：http://hz.jqgufenzy.top/gtwvbketjo.html

I. 正则表达式
来源：http://hz.jianghu66.top/gtwrslnsub.html

================================================================================
来源：http://hz.hysaishi.cn/gtyfcogdkg.html

[I01] 判断是否匹配
来源：http://hz.dianchejie.cn/gtbyymgywh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hongshengwenyu.top/gteeuwxzpl.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hysaishi.cn/gtskndmalw.html

JS:   /\d+/.test(s)
来源：http://hz.zhengqikj.top/gtcnesusym.html

TS:   /\d+/.test(s)
来源：http://hz.0kj1m.cn/gtlufrzogi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yueranfly.top/gtugfbjaxa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.pengpengdd.cyou/gtkzlwglef.html

Ruby: s.match?(/\d+/)
来源：http://hz.9152youxi.cn/gtdbdkdbig.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yonumen.top/gtwqqvogqx.html

[I02] 提取所有匹配
来源：http://hz.ybcxt.top/gtmlctirzz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sweek.top/gtigqivgxx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xylfe.cn/gtybaejuem.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yanxiufei.cn/gtqcrctpjk.html

TS:   s.match(/\d+/g)
来源：http://hz.ydjk.org.cn/gtextqbbux.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.chenjidiqi.icu/gtjcjwrtus.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cheryme.top/gtnofkvnwk.html

Ruby: s.scan(/\d+/)
来源：http://hz.yongpay.top/gtdbdhbrqo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hywenlv.cn/gtxpavialc.html

[I03] 提取捕获分组
来源：http://hz.52xcode.cn/gtrpeppqlb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.c1oappe.top/gtueqbzcqr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhaomingkeji.xyz/gtwvjgruwc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jlsjyb.cn/gttaajjcus.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hnqzz.top/gtgapsjwqz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sysykeji.top/gtudpgbkdm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxuanxn.top/gtbqzoeozp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zycfv.cn/gtreukurok.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sysykeji.top/gtuckibkbp.html

[I04] 正则替换
来源：http://hz.hnxiangtu.top/gtfrwkfzzf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sweek.top/gtoeauwmnj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cashguo.top/gtkctdeqne.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yonumen.top/gtucitijna.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtltcsgncb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.9152youxi.cn/gtyzcklrgz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.daria6918.cn/gtiqngytju.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shzxlz.cn/gtqlgrcbre.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.quarkkingdee.top/gthmgffgei.html

[I05] 按正则拆分
来源：http://hz.zhixingplan.top/gtslipknbz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhoulong.xyz/gtlpfirpjp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.havefunace.top/gtwwxazijp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.iojbl.cn/gtphcwcltt.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtvfgtsfsm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhongyouzk.top/gtpspnzfrv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.birdmap.top/gtgoouechl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinqigufen.top/gtwdfzoloi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xziqi.cn/gtxetxmqld.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cheryme.top/gtzkwerobs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gtvtiagjvn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinqigufen.top/gtthfnhwdd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yanxiufei.cn/gtkgjrepbp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhijiandao.cn/gtoxxlggfk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.mhx1999.top/gtorgwykrn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhongyouzk.top/gtbcggaytr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinqigfzy.top/gtgogmdrdp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.aizwys.cn/gtxgoqhqpt.html

[I07] 忽略大小写与多行模式
来源：http://hz.smart0.xyz/gtfbixihnv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yongpay.top/gtrhelrnwx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.snrcjt.cn/gtbtkufzhj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.chenlongwang.top/gtmsvaekbp.html

TS:   /error/gim
来源：http://hz.sweek.top/gtctrgexpm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sysykeji.top/gtmumonrwc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xziqi.cn/gtwskafrop.html

Ruby: s.scan(/error/i)
来源：http://hz.jinghuilouyu.cn/gtishezlec.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.havefunace.top/gtmvnnmtps.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cheryme.top/gtmhnrbhie.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hnxiangtu.top/gtqatrhbqe.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shanyushiyangkeji.top/gtqbeicqyi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.bjfxy.top/gtzlmcgrkg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yueranfly.top/gtwlocadqx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sweek.top/gtoewcecey.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ppjwa.cn/gtcdvonomz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.andypj.xyz/gtchudstsa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hywenlv.cn/gtnireanwl.html

================================================================================
来源：http://hz.zhijiandao.cn/gtddzqnbog.html

J. 日期与时间
来源：http://hz.jqgfzy.top/gthdbswwbj.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtmmtwqmbh.html

[J01] 获取当前时间
来源：http://hz.zhiwuduotai.top/gtyhwefhuo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.dianchejie.cn/gtfveqpeiv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yongpay.top/gtjvvmkxfw.html

JS:   new Date();  Date.now()
来源：http://hz.cqqwz.cn/gtvnzzepzd.html

TS:   new Date();  Date.now()
来源：http://hz.jinqigufen.top/gtxsphnfme.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj20258888.top/gtrmpqtaco.html

Go:   time.Now()
来源：http://hz.xylfe.cn/gttbjyyigm.html

Ruby: Time.now
来源：http://hz.wangdashe.top/gtlwbcwnpp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hammf.cn/gtmttvstfj.html

[J02] 格式化输出
来源：http://hz.redwolf501.top/gtpiowhdwu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fengsongda.top/gtjocbafes.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yanxiufei.cn/gtrezkaxzp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hammf.cn/gtinadmbad.html

TS:   d.toISOString()
来源：http://hz.zhixingplan.top/gtzehqdcil.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenzaomai.com/gtriclxlzf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xuanzx.com/gtnbacjtjv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aibaodan.cn/gtcikallry.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hnxiangtu.top/gtfplwhpzl.html

[J03] 字符串解析为日期
来源：http://hz.cashguo.top/gtvxftybgd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.feifeiyinyue.top/gtmoiinrqg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ydzc1.top/gtwufnwljx.html

JS:   new Date("2024-01-02")
来源：http://hz.zhengqikj.top/gtlozdcqmd.html

TS:   new Date("2024-01-02")
来源：http://hz.yuxming.cn/gtuiwoecxz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtfwnmrrzw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.andypj.xyz/gtognopolk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sysykeji.top/gtwyoxwtzm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sweek.top/gtbojizlnb.html

[J04] 时间戳与日期互转
来源：http://hz.hysaishi.cn/gtbsbpjgfr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.birdmap.top/gthyucnbdt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.tianlin.xyz/gtmuqhxpzn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xingfuxueyuan.xyz/gtgugsguzh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.0kj1m.cn/gtnfuwowxa.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shanyushiyangtech.top/gtccwerxny.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ydzc1.top/gtmqnesqvy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yuanzhike.top/gtvqqnmsvl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinqigufen.top/gtudjosqus.html

[J05] 时间加减（加 7 天）
来源：http://hz.yuxming.cn/gtomrkzgrd.html

Py:   now + timedelta(days=7)
来源：http://hz.fengsongda.top/gtozxycamh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenlongwang.top/gtnkuoefnb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cucudq.cn/gtiqmfuhrg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinghuilouyu.cn/gtnzguqeew.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jianghu66.top/gtwvywpzlk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.aibaodan.cn/gtwolqsakk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sxryk.cn/gtgrxfzpzl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fzhhl.top/gtbwstwwft.html

[J06] 计算两时间之差
来源：http://hz.tanke756.top/gtwfpymule.html

Py:   (end - start).total_seconds()
来源：http://hz.wangshuangyany.cn/gtuzilpvtr.html

PHP:  $end->diff($start)->days;
来源：http://hz.birdmap.top/gthrfvwgtv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhoulong.xyz/gtyfuvieja.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinyuanbaomall.cn/gttnnwsvar.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yuxming.cn/gtkafyskhf.html

Go:   end.Sub(start).Hours()
来源：http://hz.hywenlv.cn/gtpivzycui.html

Ruby: end - start                 # 返回秒数
来源：http://hz.316326.xyz/gtrocuuazi.html

C#:   (end - start).TotalSeconds
来源：http://hz.shanyushiyangkeji.top/gtxpcilodb.html

[J07] 比较两个日期
来源：http://hz.zhaomingkeji.xyz/gttoepadbp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangkeji.top/gtcnemmneb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jlsjyb.cn/gtlizwqqzg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.wangshuangyany.cn/gtkwswxfzj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shzxlz.cn/gtsakhwzpt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hywenlv.cn/gtsmknainl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shanyushiyangtech.top/gtqfkwyypk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtjqvscslt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtmgqbcifj.html

[J08] 提取年月日与星期
来源：http://hz.smart0.xyz/gtoyenpivq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.haohaochexian.top/gttxmhpmff.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.fzhhl.top/gtikdmcmqm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ydzc1.top/gtupdorojb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinghuilouyu.cn/gtvycendas.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hfpthk.cn/gtpireiyvj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.316326.xyz/gtanzpqfdl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.mhx1999.top/gtdnfsgomc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.meibo888.top/gtuidltjln.html

[J09] 时区处理
来源：http://hz.smart0.xyz/gtlcnxmzkm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhengqikj.top/gtrhsmraow.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhiwuduotai.top/gtyeooquzl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guowangkeji.top/gtyndectjg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.c1oappe.top/gtmitrlqqr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yj20258888.top/gtddenjiqb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hnxiangtu.top/gtjlpdfino.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ehwqpu.com/gtfxcthjit.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.svipenyu.cn/gtvdnxuahf.html

[J10] 取今天 / 本月第一天
来源：http://hz.cucudq.cn/gtbrglisdw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.birdmap.top/gtlhgnbgyp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sufxvd.cn/gtgftrzebd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aizwys.cn/gtqzfulrxu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dianchejie.cn/gthksnagux.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenlongwang.top/gtgvsmmpql.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.meibo888.top/gtnoirzpwe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yonumen.top/gtzylolani.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shzxlz.cn/gtadvdjtwm.html

================================================================================
来源：http://hz.xziqi.cn/gtzednsjzu.html

K. JSON 与序列化
来源：http://hz.birdmap.top/gtnkcaixqs.html

================================================================================
来源：http://hz.gaohongyu789.top/gtpqwjdmyo.html

[K01] 对象转 JSON 字符串
来源：http://hz.shuidangran.top/gthpmlllwr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhengqikj.top/gtdtvsyipk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yuanzhike.top/gtyssftweh.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtdahycbkn.html

TS:   JSON.stringify(obj)
来源：http://hz.fzhhl.top/gtxvfawpmr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shangyingyoupin.top/gtbedvwgen.html

Go:   json.Marshal(obj)
来源：http://hz.yj202588.top/gtegaheqcf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cqqwz.cn/gtuaqkagpl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangdashe.top/gtgbykimzf.html

[K02] JSON 字符串转对象
来源：http://hz.yj20258.top/gtgnivaizt.html

Py:   json.loads(s)
来源：http://hz.ybcxt.top/gtgbeptuva.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sysykeji.top/gtzvvxlbgo.html

JS:   JSON.parse(s)
来源：http://hz.tanke756.top/gthhmtbkxu.html

TS:   JSON.parse(s)
来源：http://hz.daria6918.cn/gtbpkaxvqj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.vqdsnc.cn/gtmwsptwtr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.guowangkeji.top/gtxrijnecy.html

Ruby: JSON.parse(s)
来源：http://hz.xuanzx.com/gtmeuvlmtx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tianlin.xyz/gtdbhzsoje.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.fengsongda.top/gtwthxsats.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.fzhhl.top/gtbikaqiuf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.daxiang520.top/gtcwygfcbf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hfpthk.cn/gtpcxmtpll.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxinkj.top/gtzcsagasy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yvedp.cn/gtxfpgwsoc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.0kj1m.cn/gtngifzbin.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hongshengwenyu.top/gtdntvbbix.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cdnleiting.top/gttxionkqs.html

[K04] 读取 JSON 文件
来源：http://hz.yj20258888.top/gtkucownag.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sweek.top/gtdeeblcaw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ehwqpu.com/gtrdalrlgs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxuanxn.top/gttwvaofce.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gthyncfxmr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tanke756.top/gtwdugvyaq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.meibo888.top/gtfnbjonoz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yanxiufei.cn/gtdkguvwjv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shzxlz.cn/gtecncvnuc.html

[K05] 深拷贝对象
来源：http://hz.c1oappe.top/gtmuibokjf.html

Py:   copy.deepcopy(obj)
来源：http://hz.sxryk.cn/gtlsnobsio.html

PHP:  unserialize(serialize($obj));
来源：http://hz.daxiang520.top/gtoprsuzhf.html

JS:   structuredClone(obj)
来源：http://hz.shanyushiyangkeji.top/gtdhlmlrpk.html

TS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtxcavjiin.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.birdmap.top/gtydthbdyg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yueranfly.top/gtyfknwtve.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydzc1.top/gtcornvvpu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinqigufen.top/gtuaksdmfm.html

[K06] 解析 URL 查询串
来源：http://hz.zhiwuduotai.top/gtnymdszcv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgfzy.top/gtjupkxfjk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.guowangkeji.top/gtsroonomo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hammf.cn/gtpgzvicbs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ehwqpu.com/gtyggeqyox.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ybcxt.top/gtjzjusypx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sweek.top/gtlmsmjvjg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hysaishi.cn/gtelmeoobz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shuidangran.top/gtlweinxzt.html

[K07] 进制转换
来源：http://hz.nwbrower.top/gtqvingyyn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.nanxuanxn.top/gtkdzluytr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.fengsongda.top/gtvzdmchyi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.wangdashe.top/gtzlemcjeo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtknkvbvsq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ehwqpu.com/gtdjdosbrj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ivvv.top/gtgpezrqfy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhaomingkeji.xyz/gtfwladlzx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.dianchejie.cn/gttlfdmiyt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.pengpengdd.cyou/gtxddhzcrl.html

Py:   pickle.dumps(obj)
来源：http://hz.jlsjyb.cn/gtdshlknen.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sufxvd.cn/gtvhorcrlp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.52xcode.cn/gtkytwybcr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shuidangran.top/gtnlvoeait.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.bjfxy.top/gtbftgkwei.html

Go:   encoding/gob
来源：http://hz.nanxuanxn.top/gtrmxivuoh.html

Ruby: Marshal.dump(obj)
来源：http://hz.aibaodan.cn/gthhyajxqh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jlsjyb.cn/gtmdgkwpzg.html

================================================================================
来源：http://hz.jlsjyb.cn/gtdazwknyg.html

L. 网络请求
来源：http://hz.iojbl.cn/gtstrtkcgj.html

================================================================================
来源：http://hz.pycfn.com/gtzkqnxqzf.html

[L01] 发送 GET 请求
来源：http://hz.cashguo.top/gtznpsixed.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yanxiufei.cn/gtwujkbjvi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj202588.top/gtlwhbnokl.html

JS:   await fetch(url)
来源：http://hz.nanxuanxn.top/gtvudlxfix.html

TS:   await fetch(url)
来源：http://hz.hfpthk.cn/gtdbxulcyd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydjk.org.cn/gtkbbgqjqr.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhaomingkeji.xyz/gtyatdpskj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhaomingkeji.xyz/gtlixifjze.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.52xcode.cn/gtpzsetoby.html

[L02] 发送 POST JSON
来源：http://hz.jqgfzy.top/gtkkwmgcle.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.smart0.xyz/gtwuipjtfp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nwbrower.top/gtwfzbyipe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuanzhike.top/gtiuhzzrmr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtafmtfyvs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhengqikj.top/gtovfgydlv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.redwolf501.top/gtbimpzyyf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.kuanghao11.cn/gthuittosv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zdqjudy.top/gtrrpewmar.html

[L03] 设置自定义请求头
来源：http://hz.yangfankeji.com/gtwwapiirv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj20258.top/gtfhixhqik.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yanxiufei.cn/gtuebgbjyg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxuanxn.top/gtengqfmkm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinyuanbaomall.cn/gtxvpvhbfu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ivvv.top/gtrrcrvsvq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.aibaodan.cn/gteegmdnwo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.0kj1m.cn/gtkfbfcxpi.html


<!-- 参考信息 -->