代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.0kj1m.cn/gtshshgqvn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.chenjidiqi.icu/gtbmqkygoy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cucudq.cn/gtcauyhnty.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ydjk.org.cn/gtcivccyhr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ivvv.top/gtpbgebsnx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shuidangran.top/gtowlwlges.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yongpay.top/gtfnyuhaki.html

[H10] 资源自动释放
来源：http://hz.gogol.net.cn/gtkuntbaek.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.aizwys.cn/gtznnclsyi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nanxuanxn.top/gtcuqfccpy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jyoumei.cn/gtsdbrpilq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangdashe.top/gtolbeakmb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xziqi.cn/gttjifkphm.html

Go:   defer f.Close()
来源：http://hz.shuidangran.top/gtupfolnpv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cdnleiting.top/gtelfagnel.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.andypj.xyz/gtmxrkoyml.html

================================================================================
来源：http://hz.jqgufenzy.top/gtxhvfkhup.html

I. 正则表达式
来源：http://hz.hnqzz.top/gtknpbwakj.html

================================================================================
来源：http://hz.ydzc1.top/gtmwumbwoa.html

[I01] 判断是否匹配
来源：http://hz.wangdashe.top/gtmcxbdzmv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.nwbrower.top/gthvavhfbv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jqgfzy.top/gtclmhcaxp.html

JS:   /\d+/.test(s)
来源：http://hz.ivvv.top/gtaharjvxn.html

TS:   /\d+/.test(s)
来源：http://hz.aizwys.cn/gtwmeenmre.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinghuilouyu.cn/gtdkpffygs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shzxlz.cn/gtsxgqckje.html

Ruby: s.match?(/\d+/)
来源：http://hz.jianghu66.top/gticxsuric.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sxryk.cn/gtvewnshvp.html

[I02] 提取所有匹配
来源：http://hz.cdnleiting.top/gteppqjfjz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shangyingyoupin.top/gtcbovvvga.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.daxiang520.top/gtqasrxctz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cheryme.top/gtjcliywib.html

TS:   s.match(/\d+/g)
来源：http://hz.cqqwz.cn/gtafwswqfd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinqigfzy.top/gtgxoqbiag.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shzxlz.cn/gtnpmfscuo.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxuanxn.top/gtnofdyqqw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.haohaochexian.top/gtlijcrxqs.html

[I03] 提取捕获分组
来源：http://hz.guannengcc.top/gtpruxxhup.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shuidangran.top/gtmwmgbwjo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gotoacloud.top/gtelrrjael.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gogol.net.cn/gtqybyzaub.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yuanzhike.top/gtiintewnl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shangyingyoupin.top/gtlcsyetbd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.bjfxy.top/gtiqlopvva.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.0kj1m.cn/gtvqwxczyu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhijiandao.cn/gtvdhemkbn.html

[I04] 正则替换
来源：http://hz.hnqzz.top/gtmkpbcehf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hongshengwenyu.top/gtkkimecux.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zycfv.cn/gtyuyfzaiq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigfzy.top/gtkvdoznhy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.pengpengdd.cyou/gtqqxomdkm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hongshengwenyu.top/gtdfibgbfo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.havefunace.top/gtemeeldnd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ehwqpu.com/gtoucwvrvl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.birdmap.top/gtdowdwcef.html

[I05] 按正则拆分
来源：http://hz.gogol.net.cn/gtbnbzykbz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tanke756.top/gteralboem.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.fengsongda.top/gtsdsaytvq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtlzrtatqr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtgkweloat.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shzxlz.cn/gttooxpkse.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.fengsongda.top/gtjtaezjsz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtyhpoczvh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.vqdsnc.cn/gtesevnnpb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shzxlz.cn/gtlfeazpqj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtqyflegww.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yanxiufei.cn/gtsxprtguz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.smart0.xyz/gtvhzkhwlo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenjidiqi.icu/gtozmtcega.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ivvv.top/gtulyhjzdt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shangyingyoupin.top/gteukegobn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangtech.top/gtkcfwixqo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gtwtctiyve.html

[I07] 忽略大小写与多行模式
来源：http://hz.chenzaomai.com/gtblqmqcjz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinghuilouyu.cn/gtcsoevkrg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yongpay.top/gtjsoqeooc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nanxinkj.top/gtrwehtjgg.html

TS:   /error/gim
来源：http://hz.cqqwz.cn/gtkqtczlfd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.aizwys.cn/gtbyznbdcq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.0kj1m.cn/gtbhsqictr.html

Ruby: s.scan(/error/i)
来源：http://hz.zhijiandao.cn/gtbhaofhfq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cqqwz.cn/gtfogpvwao.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yanxiufei.cn/gtgsaavnfu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xinyue.icu/gtxbhoshfh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenjidiqi.icu/gtrdsjkxlj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aibaodan.cn/gtzclpyojf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.c1oappe.top/gtvptoyzsk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.bjfxy.top/gthfudxlki.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gotoacloud.top/gtzfwwnrec.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xziqi.cn/gtcgepudbj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.pengpengdd.cyou/gtixtulmab.html

================================================================================
来源：http://hz.zycfv.cn/gtrvkbvnpg.html

J. 日期与时间
来源：http://hz.tianlin.xyz/gtdsajvetp.html

================================================================================
来源：http://hz.wangdashe.top/gtropkaest.html

[J01] 获取当前时间
来源：http://hz.hongshengwenyu.top/gtegibeksf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guowangkeji.top/gtfuvvfxpu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gtoalvkbnx.html

JS:   new Date();  Date.now()
来源：http://hz.xuanzx.com/gtlitlexho.html

TS:   new Date();  Date.now()
来源：http://hz.zhiwuduotai.top/gtyzejxrxx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xuetiantiany.cn/gtgnrvbavp.html

Go:   time.Now()
来源：http://hz.yanxiufei.cn/gtyfxmqtah.html

Ruby: Time.now
来源：http://hz.wangshuangyany.cn/gtrgepxmer.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.birdmap.top/gtljtccbfo.html

[J02] 格式化输出
来源：http://hz.jlsjyb.cn/gtogklmqbh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gthrctagpp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jqgufenzy.top/gtfrsovssf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cucudq.cn/gtmrksabuz.html

TS:   d.toISOString()
来源：http://hz.ppjwa.cn/gtnucdugjq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hongshengwenyu.top/gtrrftzlam.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.havefunace.top/gtqpqpnoal.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shzxlz.cn/gttfomqbsn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yangfankeji.com/gtemdffxyr.html

[J03] 字符串解析为日期
来源：http://hz.chenjidiqi.icu/gtxyyudqqo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cheryme.top/gtyvjimiry.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shanyushiyangtech.top/gtwcpuuxtb.html

JS:   new Date("2024-01-02")
来源：http://hz.hysaishi.cn/gtduobmkgw.html

TS:   new Date("2024-01-02")
来源：http://hz.svipenyu.cn/gtznefubvk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nanxinkj.top/gtmoeqvvaz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.c1oappe.top/gtmfmjzhpw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.nanxuanxn.top/gtvpldrbhi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.fzhhl.top/gtvhcjbszk.html

[J04] 时间戳与日期互转
来源：http://hz.iojbl.cn/gtosgujtmr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xinyue.icu/gteivvxinu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shzxlz.cn/gtjpmiuyng.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.dashuyun.cn/gteujaykuc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gzhubu.top/gtrnyamure.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yuxming.cn/gtzmvwhvwg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yueranfly.top/gtegdoynnh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gogol.net.cn/gtmspwvkkb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gotoacloud.top/gtyrrgdbsk.html

[J05] 时间加减（加 7 天）
来源：http://hz.shuidangran.top/gtaioewbdy.html

Py:   now + timedelta(days=7)
来源：http://hz.quarkkingdee.top/gtechsobrt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shanyushiyangkeji.top/gtbndayzak.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhoulong.xyz/gtwaebstbb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xziqi.cn/gtjmvenotg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuxming.cn/gtquaocwtk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenzaomai.com/gtaibucbde.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yj202588.top/gtvndergje.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hnqzz.top/gtojljfsbo.html

[J06] 计算两时间之差
来源：http://hz.shangyingyoupin.top/gtujyyuxsg.html

Py:   (end - start).total_seconds()
来源：http://hz.yj20258888.top/gtkoyzvgad.html

PHP:  $end->diff($start)->days;
来源：http://hz.sufxvd.cn/gtvlrlrdhu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yongpay.top/gtdzbyolgs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.svipenyu.cn/gtgujkikaq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.havefunace.top/gtspulrpqs.html

Go:   end.Sub(start).Hours()
来源：http://hz.cheryme.top/gtrpaatfxc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenzaomai.com/gtdwaiwiow.html

C#:   (end - start).TotalSeconds
来源：http://hz.nanxinkj.top/gtlcjasksa.html

[J07] 比较两个日期
来源：http://hz.feifeiyinyue.top/gtnukrjskb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nanxuanxn.top/gtsumtogiv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yvedp.cn/gtuxymddwi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.kuanghao11.cn/gtktjnweuw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtmonewmqy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jqgufenzy.top/gtfgdfpjvd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.birdmap.top/gttcbkblvz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yueranfly.top/gtjvxnqhvs.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtkihclfug.html

[J08] 提取年月日与星期
来源：http://hz.cheryme.top/gtmcgzedyc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xylfe.cn/gtsmaxhtpl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gogol.net.cn/gtxszcrffh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.vqdsnc.cn/gtbxwzmotx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhaomingkeji.xyz/gtlavjzztb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.52xcode.cn/gtoxmtqocx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xinyue.icu/gtlvalpbmk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hywenlv.cn/gtnsrascne.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sxryk.cn/gtsmrsnzsh.html

[J09] 时区处理
来源：http://hz.snrcjt.cn/gtokvpenow.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.vqdsnc.cn/gtwlnczgfs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jqgufenzy.top/gttgoeaxqi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jyoumei.cn/gtpagcxfso.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtktlrhbgk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nwbrower.top/gtqslynwim.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cucudq.cn/gtilpoicfj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cashguo.top/gtulhzgtaj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cdnleiting.top/gtdakgtjws.html

[J10] 取今天 / 本月第一天
来源：http://hz.tianlin.xyz/gtlilcvput.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.c1oappe.top/gtmufgtbnv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.vqdsnc.cn/gtaovpyvtd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.c1oappe.top/gtxaatrgpw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dianchejie.cn/gtdrsfmlmu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.dashuyun.cn/gtutbrejya.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yanxiufei.cn/gtdpcyigzj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sweek.top/gtwmvvelpz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ehwqpu.com/gtfdecjgeb.html

================================================================================
来源：http://hz.chenlongwang.top/gtmmrnyofw.html

K. JSON 与序列化
来源：http://hz.xinyue.icu/gtimaksbqp.html

================================================================================
来源：http://hz.tianlin.xyz/gtcefntzae.html

[K01] 对象转 JSON 字符串
来源：http://hz.shanyushiyangkeji.top/gtkjvvegef.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gttlmkjtkc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xuetiantiany.cn/gtbjuoqcey.html

JS:   JSON.stringify(obj)
来源：http://hz.cheryme.top/gtrqlkrtkd.html

TS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gtqtorpuap.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.smart0.xyz/gtodypqoey.html

Go:   json.Marshal(obj)
来源：http://hz.mhx1999.top/gtauyzzhpl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhiwuduotai.top/gtzmtjqsjf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.dianchejie.cn/gtzflsygpq.html

[K02] JSON 字符串转对象
来源：http://hz.feifeiyinyue.top/gtsmhelyet.html

Py:   json.loads(s)
来源：http://hz.hnxiangtu.top/gtpkehdstm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinghuilouyu.cn/gtdwrdokai.html

JS:   JSON.parse(s)
来源：http://hz.zhongyouzk.top/gtrnjsgtll.html

TS:   JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtjuioiana.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yongpay.top/gtbtprffwm.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gaohongyu789.top/gtjnyfoeyd.html

Ruby: JSON.parse(s)
来源：http://hz.ppjwa.cn/gtrhbvwoyw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigufen.top/gttvnysrfr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shuidangran.top/gtrhcsmgkw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.9152youxi.cn/gthvgfecpj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.316326.xyz/gtuodicres.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gzhubu.top/gtssjpmmxm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gtntzqslox.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dianchejie.cn/gtydnwcgrw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenzaomai.com/gtvgzkfvld.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnqzz.top/gtnrqxnpvl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgufenzy.top/gtctjfyyaq.html

[K04] 读取 JSON 文件
来源：http://hz.jinqigufen.top/gtvajfvlix.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yongpay.top/gtttxwwgsj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yuxming.cn/gtxmwlkqbe.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.birdmap.top/gtrlsqfmcp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cqqwz.cn/gtyqbdsfiy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gzhubu.top/gtxsgcckiu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sufxvd.cn/gthtcprkwe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hywenlv.cn/gtezahoeub.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.9152youxi.cn/gtmbhpgvqz.html

[K05] 深拷贝对象
来源：http://hz.yuanzhike.top/gtzsmlavwg.html

Py:   copy.deepcopy(obj)
来源：http://hz.hammf.cn/gtoijrxpsn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.smart0.xyz/gtbpzxckrx.html

JS:   structuredClone(obj)
来源：http://hz.zhixingplan.top/gtosxxntyj.html

TS:   structuredClone(obj)
来源：http://hz.zhongyouzk.top/gtkljsdgky.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jiagoushi.top/gtrneeursc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xylfe.cn/gtzrvkevyu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cucudq.cn/gtbhuvwzqy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.iojbl.cn/gtuuxjnazz.html

[K06] 解析 URL 查询串
来源：http://hz.nanxinkj.top/gttrzileyw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhiwuduotai.top/gtfoisbawk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.meibo888.top/gtfirffcjh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hywenlv.cn/gtpfpvcksm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinyuanbaomall.cn/gtiguwqtyw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.316326.xyz/gtkzdmvzia.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sxryk.cn/gtrsoedgeq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yonumen.top/gttqyftptk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.aibaodan.cn/gtbodlvkhl.html

[K07] 进制转换
来源：http://hz.yueranfly.top/gtqfogblrf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hnqzz.top/gtqnokomgl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258888.top/gtqshwlrmr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtprkwrfdj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtttwqhasm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtegorscaf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhongyouzk.top/gttzpdnxnr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.316326.xyz/gtwctwclbh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shangyingyoupin.top/gtzncnmgjp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tian-w.cn/gtaxhcswou.html

Py:   pickle.dumps(obj)
来源：http://hz.havefunace.top/gtnaiatuva.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ppjwa.cn/gtreyufnxk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gaohongyu789.top/gtoelywyti.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gtgepqbiwe.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yuxming.cn/gtuqgcnggc.html

Go:   encoding/gob
来源：http://hz.smart0.xyz/gtcsabhayq.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenjidiqi.icu/gtbjgqfnis.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.9152youxi.cn/gtyniqvjzl.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtqrteowvk.html

L. 网络请求
来源：http://hz.cashguo.top/gtwtmyzipz.html

================================================================================
来源：http://hz.sxryk.cn/gtoujbjqud.html

[L01] 发送 GET 请求
来源：http://hz.aizwys.cn/gtevgmznew.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gotoacloud.top/gtfmddxrqs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.havefunace.top/gtptnxdaln.html

JS:   await fetch(url)
来源：http://hz.jinyuanbaomall.cn/gtvdjupvqc.html

TS:   await fetch(url)
来源：http://hz.zhengqikj.top/gtidycrclt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gaohongyu789.top/gtjikvmogc.html

Go:   resp, err := http.Get(url)
来源：http://hz.wangshuangyany.cn/gttnghhxhj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.quarkkingdee.top/gtizkozbdc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gotoacloud.top/gtspbkznpn.html

[L02] 发送 POST JSON
来源：http://hz.jinqigfzy.top/gtmnbaikkd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ehwqpu.com/gtnyowdskt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinqigfzy.top/gtsuizhsva.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jyoumei.cn/gtjvtworwr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuetiantiany.cn/gtyhexyfgb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.daria6918.cn/gtvjtnzydc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ydjk.org.cn/gtzrxgfdza.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.bjfxy.top/gtryunrijj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shangyingyoupin.top/gteyuusvgr.html

[L03] 设置自定义请求头
来源：http://hz.xuanzx.com/gtibsuiutg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xinyue.icu/gtryjrubmk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.feifeiyinyue.top/gtxstlvgbd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pycfn.com/gtczdjxhvf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.9152youxi.cn/gteahuvnpv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinghuilouyu.cn/gtisikfpxy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.316326.xyz/gtjvdefwtq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.quarkkingdee.top/gtsvoarbwh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhoulong.xyz/gtfhesbmtt.html

[L04] 设置超时
来源：http://hz.pycfn.com/gtwssfehvt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.dashuyun.cn/gtnoffinrm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tianlin.xyz/gtgemtntqv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tian-w.cn/gtzrghnxsn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jyoumei.cn/gtophxthup.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.snrcjt.cn/gtpujxgsyx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tianlin.xyz/gtxtutsyvf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhixingplan.top/gtpqrghjzy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhixingplan.top/gtechdxvfb.html

[L05] 上传文件（multipart）
来源：http://hz.quarkkingdee.top/gthcpitwqw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yanxiufei.cn/gttztdqtdr.html


<!-- 参考信息 -->