代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhixingplan.top/gtttnibgft.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tianlin.xyz/gtvkwntvgc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.wangshuangyany.cn/gtqnvtzpfy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cashguo.top/gtjegouxfl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xinyue.icu/gtjtenmwdc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nwbrower.top/gtgnozqzoo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hongshengwenyu.top/gtwbfhyfwk.html

[H10] 资源自动释放
来源：http://hz.sysykeji.top/gtxcmqhwkt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.9152youxi.cn/gthdolmptt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dianchejie.cn/gtcgwcasvb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtopueznjj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gtoocxhzsj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.havefunace.top/gtwvntipdv.html

Go:   defer f.Close()
来源：http://hz.tianlin.xyz/gtfhhsduke.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tianlin.xyz/gtziimaywh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hammf.cn/gtyrhcsktu.html

================================================================================
来源：http://hz.ivvv.top/gtorrhlyxi.html

I. 正则表达式
来源：http://hz.yangfankeji.com/gtkqlxtzpo.html

================================================================================
来源：http://hz.jqgufenzy.top/gtycfkbkqz.html

[I01] 判断是否匹配
来源：http://hz.cheryme.top/gtbbvvqplv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtnofpcowg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.316326.xyz/gtzvfdpcre.html

JS:   /\d+/.test(s)
来源：http://hz.snrcjt.cn/gtadtzskua.html

TS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gtsxskswoo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yj20258888.top/gtppvqavzw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.fzhhl.top/gtgjanmzpm.html

Ruby: s.match?(/\d+/)
来源：http://hz.ydjk.org.cn/gtvnjeaebi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangdashe.top/gtdpdxuopm.html

[I02] 提取所有匹配
来源：http://hz.xziqi.cn/gtbtukxyep.html

Py:   re.findall(r"\d+", s)
来源：http://hz.havefunace.top/gtgpokzddn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.pycfn.com/gttlqbcpft.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nwbrower.top/gtftcmtmug.html

TS:   s.match(/\d+/g)
来源：http://hz.chenjidiqi.icu/gtnqogwtqk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sxryk.cn/gtxdwhuhgn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gotoacloud.top/gtniciysej.html

Ruby: s.scan(/\d+/)
来源：http://hz.gaohongyu789.top/gtdeglecdo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.smart0.xyz/gtmxbbvmxs.html

[I03] 提取捕获分组
来源：http://hz.mhx1999.top/gtsvsukeid.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.daxiang520.top/gtfyhxkohp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ivvv.top/gtylpbldyh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.mhx1999.top/gtzdxfthih.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.fengsongda.top/gtkaucinkq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pengpengdd.cyou/gtjlzlelvc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhengqikj.top/gtgwcwhypq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xylfe.cn/gtoyoqlcnd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ydzc1.top/gtmuhbsqmu.html

[I04] 正则替换
来源：http://hz.jiagoushi.top/gthvbewyde.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gotoacloud.top/gtltcxfymc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sufxvd.cn/gthjrllhhd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtzogrwhra.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gtudwzacum.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.bjfxy.top/gteabiaduf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinqigfzy.top/gtuelwvugc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhengqikj.top/gthdyttvlb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jqgufenzy.top/gtvumlyhqt.html

[I05] 按正则拆分
来源：http://hz.svipenyu.cn/gtorysfzbp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jqgfzy.top/gtwiyhuwgt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shuidangran.top/gttfsinrks.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtgxpwdzov.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtljmtvmax.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jyoumei.cn/gtnizjjnhb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ydjk.org.cn/gtfthlridd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtfwgrrxkg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ybcxt.top/gtuoewpovo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.pycfn.com/gtkrvjjnoi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtacmvjlnd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnqzz.top/gtfhhuduli.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtlejiqphv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenjidiqi.icu/gtxjnsject.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtwfllonpp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hammf.cn/gtiniaieqq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yueranfly.top/gtcwmnjdjl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtjpyieore.html

[I07] 忽略大小写与多行模式
来源：http://hz.0kj1m.cn/gtrmdskhyv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yvedp.cn/gtrubfsscl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.pengpengdd.cyou/gtgaskdnrb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cheryme.top/gtdqtwghtk.html

TS:   /error/gim
来源：http://hz.meibo888.top/gtyvyjesqi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinqigufen.top/gteevvvpqt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinqigfzy.top/gtrygmarxc.html

Ruby: s.scan(/error/i)
来源：http://hz.bjfxy.top/gtnfdkbhgd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.iojbl.cn/gtufrfdnlg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ywan-chungtsiang.top/gtzwiwbjoi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhoulong.xyz/gtxygnpxot.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.kuanghao11.cn/gtuosaxqlo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.snrcjt.cn/gtvnfqwhcf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtcraatday.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sweek.top/gthimvdizu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zycfv.cn/gtcxvekqze.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hongshengwenyu.top/gtiqaveslo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.svipenyu.cn/gtrheqwfkn.html

================================================================================
来源：http://hz.ivvv.top/gtznoelxjv.html

J. 日期与时间
来源：http://hz.fengsongda.top/gtjraiobzb.html

================================================================================
来源：http://hz.yuanzhike.top/gtaprfjais.html

[J01] 获取当前时间
来源：http://hz.nwbrower.top/gtvffybnvz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhaomingkeji.xyz/gtezbwqlgo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sufxvd.cn/gtskjinkyx.html

JS:   new Date();  Date.now()
来源：http://hz.bjfxy.top/gtcmvfzgor.html

TS:   new Date();  Date.now()
来源：http://hz.zhiwuduotai.top/gtpuxwqsiy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenlongwang.top/gtnrqucnmi.html

Go:   time.Now()
来源：http://hz.yvedp.cn/gtrsqszmqa.html

Ruby: Time.now
来源：http://hz.hysaishi.cn/gtfdribzqr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jlsjyb.cn/gtnuzqbzhy.html

[J02] 格式化输出
来源：http://hz.zhengqikj.top/gtdhqejwcv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.havefunace.top/gtcnexdmir.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.52xcode.cn/gtdannrebf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hammf.cn/gtziargsro.html

TS:   d.toISOString()
来源：http://hz.aizwys.cn/gtwpdnvnii.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.havefunace.top/gtbgjbgfsh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yvedp.cn/gtmkwskvww.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yongpay.top/gtqbyqclex.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.havefunace.top/gtqakorduw.html

[J03] 字符串解析为日期
来源：http://hz.c1oappe.top/gtnmgawecc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zdqjudy.top/gtqgajmjdl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cucudq.cn/gtxmpuvatj.html

JS:   new Date("2024-01-02")
来源：http://hz.ppjwa.cn/gtvvftuerj.html

TS:   new Date("2024-01-02")
来源：http://hz.jianghu66.top/gtrqkkkltr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhongyouzk.top/gtwjomvewo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.birdmap.top/gtnpmpdbym.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xuanzx.com/gtxvsyeqbs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cashguo.top/gtohtvwopr.html

[J04] 时间戳与日期互转
来源：http://hz.ywan-chungtsiang.top/gtwbbauqkd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhengqikj.top/gtaclkflrc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guowangkeji.top/gtvovfnalq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yanxiufei.cn/gtzuowjfct.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sufxvd.cn/gtgaqjetym.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.vqdsnc.cn/gtfxyxxxgg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgfzy.top/gtbkcpzibe.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ivvv.top/gtstjtcqrg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.iojbl.cn/gtxliuspzk.html

[J05] 时间加减（加 7 天）
来源：http://hz.haohaochexian.top/gtsrpadsjh.html

Py:   now + timedelta(days=7)
来源：http://hz.cdnleiting.top/gtbknbtpqf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.andypj.xyz/gtwxbpqtve.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ivvv.top/gtikfhwngi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cashguo.top/gtunxzvroo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hnxiangtu.top/gtqznksfqx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.wangshuangyany.cn/gtvdksjkea.html

Ruby: Time.now + 7 * 86400
来源：http://hz.meibo888.top/gtmdicfqcp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zdqjudy.top/gttphrafwu.html

[J06] 计算两时间之差
来源：http://hz.tian-w.cn/gtrnxartin.html

Py:   (end - start).total_seconds()
来源：http://hz.jianghu66.top/gtwjywxkvu.html

PHP:  $end->diff($start)->days;
来源：http://hz.xuetiantiany.cn/gtqvxxdifp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhiwuduotai.top/gtrvvarxfx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxuanxn.top/gtbavxgywv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zdqjudy.top/gtcnsjsqfi.html

Go:   end.Sub(start).Hours()
来源：http://hz.yangfankeji.com/gtmasyxgnk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.aizwys.cn/gtknkmulys.html

C#:   (end - start).TotalSeconds
来源：http://hz.redwolf501.top/gtfryktwlj.html

[J07] 比较两个日期
来源：http://hz.tanke756.top/gtbbgylhbk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.birdmap.top/gtfztprvlw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cucudq.cn/gtxrmlijrx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ppjwa.cn/gthpcvgssw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhoulong.xyz/gtyhinhlgv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.iojbl.cn/gtdiikjxcy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhengqikj.top/gtxkyttowy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtyyukzsde.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtwjqeeexi.html

[J08] 提取年月日与星期
来源：http://hz.gogol.net.cn/gtycotnstj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hongshengwenyu.top/gtjadzwbkn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gotoacloud.top/gtnsplycus.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ehwqpu.com/gtmqpwgtzb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.aizwys.cn/gtzqxjvedh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ehwqpu.com/gtpdzlvomr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.quarkkingdee.top/gtjeqwliqr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yvedp.cn/gtvjyohncg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sweek.top/gthhrwqhlg.html

[J09] 时区处理
来源：http://hz.cashguo.top/gtwrspoact.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yanxiufei.cn/gtsktvovus.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yj20258888.top/gtgmvpskjp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jiagoushi.top/gtbodkfzvj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhiwuduotai.top/gtzufccbhs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.meibo888.top/gtclzgbwrj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ydzc1.top/gtkdijngsd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jlsjyb.cn/gteuuznnpk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinqigfzy.top/gtglljbnfv.html

[J10] 取今天 / 本月第一天
来源：http://hz.jyoumei.cn/gticaplbaw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hammf.cn/gteiazzfve.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shangyingyoupin.top/gtskyujkcu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.dianchejie.cn/gtotsbmaxl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.mhx1999.top/gtboubcpgg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shzxlz.cn/gtftcevkyx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.feifeiyinyue.top/gthwfziqvp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.bjfxy.top/gtjledlotq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xylfe.cn/gtgbnioact.html

================================================================================
来源：http://hz.mhx1999.top/gtzewtftzp.html

K. JSON 与序列化
来源：http://hz.xuetiantiany.cn/gtjortciby.html

================================================================================
来源：http://hz.jqgfzy.top/gtupkysoaz.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenjidiqi.icu/gtyrkvuofe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tanke756.top/gtccsctuhy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydzc1.top/gthimgprqx.html

JS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gthjdruxuw.html

TS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtezwycwhn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinghuilouyu.cn/gteczadeuy.html

Go:   json.Marshal(obj)
来源：http://hz.zhongyouzk.top/gttvasbbie.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.aibaodan.cn/gtsebiszms.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yonumen.top/gtggcwiruq.html

[K02] JSON 字符串转对象
来源：http://hz.sysykeji.top/gtxbaegyre.html

Py:   json.loads(s)
来源：http://hz.nanxinkj.top/gtnirwrhpe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shanyushiyangtech.top/gtwdriydic.html

JS:   JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtnmkosfcq.html

TS:   JSON.parse(s)
来源：http://hz.ppjwa.cn/gttcvqqtqf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gzhubu.top/gtsdyajixn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtxryomfsx.html

Ruby: JSON.parse(s)
来源：http://hz.havefunace.top/gtuaghyhzm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shzxlz.cn/gtrtlqcinw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.chenzaomai.com/gtvpihygoh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.dianchejie.cn/gtanjupjdh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangkeji.top/gtpmyrlplz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhijiandao.cn/gtpivugbpg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenjidiqi.icu/gtwumvpcne.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinqigufen.top/gtdzkkvhax.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xingfuxueyuan.xyz/gtcncofeen.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhijiandao.cn/gtmewveqeu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.meibo888.top/gtiumrrgqu.html

[K04] 读取 JSON 文件
来源：http://hz.daria6918.cn/gtlxccycxv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jqgufenzy.top/gtbvwgimqx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.dashuyun.cn/gtrglmreft.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hammf.cn/gtkmvpadna.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tanke756.top/gtqrzmhbgi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yueranfly.top/gtbmqtljqj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jianghu66.top/gtgfapkavh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cashguo.top/gtstikntar.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ydjk.org.cn/gtlsflvbps.html

[K05] 深拷贝对象
来源：http://hz.hysaishi.cn/gtzadjizxb.html

Py:   copy.deepcopy(obj)
来源：http://hz.xinyue.icu/gtirgpcdnu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenjidiqi.icu/gtvpouysvh.html

JS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtbqyxyhsb.html

TS:   structuredClone(obj)
来源：http://hz.9152youxi.cn/gtgtykqavf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zdqjudy.top/gtrphrrqeb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zycfv.cn/gtqkwpfzfd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hongshengwenyu.top/gtioqlocwf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhengqikj.top/gtnkqrxoco.html

[K06] 解析 URL 查询串
来源：http://hz.feifeiyinyue.top/gtrcibnfwr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhaomingkeji.xyz/gtojficmok.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258.top/gtfraxqese.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sysykeji.top/gttmjacita.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yanxiufei.cn/gtxcautrdx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nanxuanxn.top/gtkufdkagi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cucudq.cn/gtnyqweeef.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.quarkkingdee.top/gtkuoupfoq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tanke756.top/gtvdpxhche.html

[K07] 进制转换
来源：http://hz.xuanzx.com/gtkbhwohox.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.iojbl.cn/gtwjuqoakp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yongpay.top/gtuovtrcrm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtaxxovfdq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtribqtyee.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtqelugdsm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.redwolf501.top/gtppdlmlll.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ivvv.top/gtwhfybgea.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.dashuyun.cn/gtyzwhtpdf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.snrcjt.cn/gtsuvgyhtf.html

Py:   pickle.dumps(obj)
来源：http://hz.svipenyu.cn/gtkitzyfyf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.chenlongwang.top/gtajbptppc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gtlqnxgsfx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cucudq.cn/gtdlotiwfk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ehwqpu.com/gtipuveflw.html

Go:   encoding/gob
来源：http://hz.sweek.top/gtryzbjyei.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhaomingkeji.xyz/gtsbdytmhd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jiagoushi.top/gtkpgluxjj.html

================================================================================
来源：http://hz.cdnleiting.top/gtvwifrbpn.html

L. 网络请求
来源：http://hz.meibo888.top/gtzlmxhuag.html

================================================================================
来源：http://hz.ivvv.top/gtsgctwusj.html

[L01] 发送 GET 请求
来源：http://hz.9152youxi.cn/gtswhbjylq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hammf.cn/gtpollzrbb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sysykeji.top/gthqoplmil.html

JS:   await fetch(url)
来源：http://hz.zhiwuduotai.top/gtseycpklm.html

TS:   await fetch(url)
来源：http://hz.ydzc1.top/gtrscofmxp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.nwbrower.top/gtosubiodb.html

Go:   resp, err := http.Get(url)
来源：http://hz.hongshengwenyu.top/gtkllyppou.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sysykeji.top/gtxgorxtch.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.fzhhl.top/gtclvjlvgb.html

[L02] 发送 POST JSON
来源：http://hz.hysaishi.cn/gtipwkjdsq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenlongwang.top/gtrjrzhrpk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tanke756.top/gttelmzeih.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gtbaqjhoot.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhijiandao.cn/gtyipwqmrt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhoulong.xyz/gtotdeemzs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhongyouzk.top/gtlxtlgtgj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.andypj.xyz/gtzdfolzzj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sxryk.cn/gtoseukbct.html

[L03] 设置自定义请求头
来源：http://hz.gotoacloud.top/gtpyhjysmc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.feifeiyinyue.top/gtuceyykbm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.iojbl.cn/gtdlhmlgec.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinyuanbaomall.cn/gtgghargoi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pengpengdd.cyou/gtyxkgcywl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenlongwang.top/gtdnsuyzey.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hongshengwenyu.top/gtopcugkph.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinqigufen.top/gtkzilszgm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.quarkkingdee.top/gtdnudfkkb.html

[L04] 设置超时
来源：http://hz.gzhubu.top/gtgpwxbccd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xinyue.icu/gtldorctxh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinqigufen.top/gtjqdraubr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gtuuayhqss.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gttkhgvwwm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhijiandao.cn/gtqolhizlf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.nanxuanxn.top/gtncydlkeq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cheryme.top/gtfpwfcyxe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ehwqpu.com/gtajpvqrse.html

[L05] 上传文件（multipart）
来源：http://hz.xziqi.cn/gtpmwvmhpb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj20258888.top/gtbxuuqqkc.html


<!-- 参考信息 -->