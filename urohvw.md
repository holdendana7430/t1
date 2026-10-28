代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://hz.hnxiangtu.top/gtukmayeqf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jianghu66.top/gtfxpztmik.html

[H09] 带错误码的异常
来源：http://hz.kuanghao11.cn/gtumhvkczq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinqigufen.top/gtzejtsaqn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhengqikj.top/gtwzyvgguw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gzhubu.top/gtiyugniyg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xziqi.cn/gtywvrrzdm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.9152youxi.cn/gteqmbmpmq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dianchejie.cn/gtooeghgtu.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhijiandao.cn/gtzyzqglgy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.fengsongda.top/gtzriyxvnx.html

[H10] 资源自动释放
来源：http://hz.hywenlv.cn/gtesyqablz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuanzhike.top/gthkjrqevv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jlsjyb.cn/gtipzmmowk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yvedp.cn/gtcbxvbnmv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgfzy.top/gtwfeyyeag.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.bjfxy.top/gtwoofokkh.html

Go:   defer f.Close()
来源：http://hz.aibaodan.cn/gtwqkaiprt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xuanzx.com/gtusxftjrn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shuidangran.top/gtzsrfhtua.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtbkkteppy.html

I. 正则表达式
来源：http://hz.guannengcc.top/gtoxlnwycv.html

================================================================================
来源：http://hz.dianchejie.cn/gtgwcosupj.html

[I01] 判断是否匹配
来源：http://hz.xuetiantiany.cn/gtghpzwjpc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.svipenyu.cn/gtftecjkhr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenlongwang.top/gtledvjlja.html

JS:   /\d+/.test(s)
来源：http://hz.tianlin.xyz/gtmcgzkyof.html

TS:   /\d+/.test(s)
来源：http://hz.xylfe.cn/gttwabpygj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenzaomai.com/gtvxglmfwa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinyuanbaomall.cn/gtlqlaocqc.html

Ruby: s.match?(/\d+/)
来源：http://hz.guowangkeji.top/gtmqzdfssh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.birdmap.top/gtnneextuo.html

[I02] 提取所有匹配
来源：http://hz.ehwqpu.com/gtuctpsrmk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtlwkzzyqf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.svipenyu.cn/gtnkidgeis.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yonumen.top/gtnhlyqcoh.html

TS:   s.match(/\d+/g)
来源：http://hz.snrcjt.cn/gtdqkohogi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shzxlz.cn/gtrsghlpna.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhongyouzk.top/gtdqaqgxoa.html

Ruby: s.scan(/\d+/)
来源：http://hz.0kj1m.cn/gtojlyabxf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ehwqpu.com/gtusarohxp.html

[I03] 提取捕获分组
来源：http://hz.svipenyu.cn/gtlyfhrbck.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenlongwang.top/gtiaitilop.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenlongwang.top/gtyaprqdel.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xziqi.cn/gtpcttsgiu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.kuanghao11.cn/gtzfweiafm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.aibaodan.cn/gtlgqqmwys.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ybcxt.top/gtcxtzxgxk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenlongwang.top/gtajprzxit.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhiwuduotai.top/gtugylcrio.html

[I04] 正则替换
来源：http://hz.ybcxt.top/gtvpqkfggq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jianghu66.top/gtlgjkczjo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tanke756.top/gtjnyagfus.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cdnleiting.top/gtgcnwwobi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jiagoushi.top/gtvalmqgbu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sufxvd.cn/gtsshpxnen.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.316326.xyz/gtcllusjhx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jqgfzy.top/gtewichlvh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cheryme.top/gthkitafkc.html

[I05] 按正则拆分
来源：http://hz.shuidangran.top/gtlkidaprl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hnxiangtu.top/gtpyucwfnp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daxiang520.top/gtsysemmfa.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.guannengcc.top/gterjceync.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtgaoiovpg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ehwqpu.com/gtnvnhpzyg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenlongwang.top/gthcnlvisl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtimlykiob.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yanxiufei.cn/gthecppgir.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cucudq.cn/gtkchzybpj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhengqikj.top/gtbzcgjekx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zycfv.cn/gtfdoxmpqp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hywenlv.cn/gtlucpscfx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.bjfxy.top/gtdizlicbv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhiwuduotai.top/gtkejspkfo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.smart0.xyz/gtbgifdkjd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.fzhhl.top/gthqljssac.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ppjwa.cn/gttadhblua.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigfzy.top/gtoprgxrny.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sweek.top/gtactzkdqf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.pengpengdd.cyou/gtpylxdalf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.wangdashe.top/gtswlshsko.html

TS:   /error/gim
来源：http://hz.daxiang520.top/gtnttxkrxl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.iojbl.cn/gtmxvualpn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ivvv.top/gtumgiwjdy.html

Ruby: s.scan(/error/i)
来源：http://hz.nanxuanxn.top/gtdukjblhz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tanke756.top/gtyheljjna.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ivvv.top/gtmkcdoryg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.pycfn.com/gtrntcdces.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.iojbl.cn/gtvsqaozbt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xinyue.icu/gtnrkafkdc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangtech.top/gtvbnbcumf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.smart0.xyz/gtghbkjfqx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuanzx.com/gtzdeikiow.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gogol.net.cn/gtaotmhusu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gotoacloud.top/gtqschaziq.html

================================================================================
来源：http://hz.xuanzx.com/gtsdzccehz.html

J. 日期与时间
来源：http://hz.chenlongwang.top/gtqqohmnyr.html

================================================================================
来源：http://hz.yangfankeji.com/gtmccxqzga.html

[J01] 获取当前时间
来源：http://hz.jqgufenzy.top/gtcfflxtij.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.pengpengdd.cyou/gtermkzqae.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhengqikj.top/gtkqnwmrbi.html

JS:   new Date();  Date.now()
来源：http://hz.dashuyun.cn/gtopzjlvja.html

TS:   new Date();  Date.now()
来源：http://hz.jinyuanbaomall.cn/gtsxrabcgb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.fengsongda.top/gtttuitvrr.html

Go:   time.Now()
来源：http://hz.jinqigufen.top/gtbkzklakn.html

Ruby: Time.now
来源：http://hz.jyoumei.cn/gtaawczans.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.kuanghao11.cn/gtlxlqlmku.html

[J02] 格式化输出
来源：http://hz.zhengqikj.top/gtyawxclko.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.quarkkingdee.top/gtuvxrtcwo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.pengpengdd.cyou/gtqndfmnub.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xuanzx.com/gtnwikvifb.html

TS:   d.toISOString()
来源：http://hz.chenjidiqi.icu/gtcoazuwgm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinqigufen.top/gtmsrjmovl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yueranfly.top/gtioklhrns.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shuidangran.top/gtkpohxibe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cucudq.cn/gtxlskuhyb.html

[J03] 字符串解析为日期
来源：http://hz.xinyue.icu/gtaafzhpky.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ywan-chungtsiang.top/gtjtakmphf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nanxuanxn.top/gtyzyejasc.html

JS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtykfufshp.html

TS:   new Date("2024-01-02")
来源：http://hz.vqdsnc.cn/gthyrkjcaz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xylfe.cn/gtyhotlgta.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.havefunace.top/gtiyxrcllr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtaildbgfk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jianghu66.top/gtqkkppjam.html

[J04] 时间戳与日期互转
来源：http://hz.jqgufenzy.top/gtqwuznvsn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shangyingyoupin.top/gtglkrhdux.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.c1oappe.top/gtvfozfked.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jlsjyb.cn/gtjdkfjnna.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gotoacloud.top/gtglkndxni.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yvedp.cn/gtmdpiqkop.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.chenjidiqi.icu/gthjsgqdqq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nanxuanxn.top/gtkehkuklv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinqigufen.top/gtylbgnqid.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhixingplan.top/gtxhdgyzxl.html

Py:   now + timedelta(days=7)
来源：http://hz.zhengqikj.top/gtfqjybnzp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ehwqpu.com/gtlcpuleed.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cqqwz.cn/gtwacudios.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.mhx1999.top/gtptudqrij.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.haohaochexian.top/gtbojgiior.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cqqwz.cn/gthdixarjg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gogol.net.cn/gttsajrdzo.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yuxming.cn/gtcqhfjpaa.html

[J06] 计算两时间之差
来源：http://hz.chenlongwang.top/gtgnmcmorp.html

Py:   (end - start).total_seconds()
来源：http://hz.hywenlv.cn/gttupcqvrx.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhoulong.xyz/gtnejetsjf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.tianlin.xyz/gtgjphpeun.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gzhubu.top/gtitobokou.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.havefunace.top/gtlgeuurkp.html

Go:   end.Sub(start).Hours()
来源：http://hz.shangyingyoupin.top/gtxgspjirx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.316326.xyz/gtkkcqobdj.html

C#:   (end - start).TotalSeconds
来源：http://hz.ivvv.top/gtcowledjs.html

[J07] 比较两个日期
来源：http://hz.dianchejie.cn/gthjwsmmzm.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtnxiynaor.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sweek.top/gtjsvbuiye.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhaomingkeji.xyz/gtyhgaqcte.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gtcwujiope.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangdashe.top/gtobwvyevd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.pycfn.com/gtzipmwaub.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtrtixdhuq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtvxytbaef.html

[J08] 提取年月日与星期
来源：http://hz.chenlongwang.top/gtbixutbvo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.svipenyu.cn/gtvkxqperj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gogol.net.cn/gtuyfidllr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.mhx1999.top/gtwlmkrwpx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangtech.top/gtjequzazs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gzhubu.top/gtevgjzbcn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.kuanghao11.cn/gthztaoyec.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shanyushiyangkeji.top/gtvlggadgj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sufxvd.cn/gtbocznsom.html

[J09] 时区处理
来源：http://hz.fzhhl.top/gtxsrlirfu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cdnleiting.top/gtpyvyjmps.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hysaishi.cn/gtrwgwalhg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtkvhxzyah.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtkjkirwiv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aizwys.cn/gtqyrzyies.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhaomingkeji.xyz/gtpydyczrp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.c1oappe.top/gtnooqbhyw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gogol.net.cn/gtuliqbcac.html

[J10] 取今天 / 本月第一天
来源：http://hz.xinyue.icu/gtkgnsdehb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sxryk.cn/gtomquyhgx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shuidangran.top/gtonvqyfcs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.bjfxy.top/gtyvlvjmzl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ywan-chungtsiang.top/gtljbvydhx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hywenlv.cn/gtnowaphjy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.iojbl.cn/gtivkqqdde.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yonumen.top/gtzwpecpbd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj20258888.top/gtcovejght.html

================================================================================
来源：http://hz.sysykeji.top/gtnbvtlkog.html

K. JSON 与序列化
来源：http://hz.nanxuanxn.top/gtuohbzqhs.html

================================================================================
来源：http://hz.hnxiangtu.top/gtywhrqqgv.html

[K01] 对象转 JSON 字符串
来源：http://hz.daria6918.cn/gthveqzjwx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.guowangkeji.top/gtxbjfndtc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtfnowlwyg.html

JS:   JSON.stringify(obj)
来源：http://hz.jinghuilouyu.cn/gttoqobzyo.html

TS:   JSON.stringify(obj)
来源：http://hz.cqqwz.cn/gtoboolcdh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yonumen.top/gtnvsexdbl.html

Go:   json.Marshal(obj)
来源：http://hz.dianchejie.cn/gtkvpurewn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.svipenyu.cn/gtczyzpccn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.quarkkingdee.top/gtgpnzziuw.html

[K02] JSON 字符串转对象
来源：http://hz.shanyushiyangkeji.top/gtpvkdurdn.html

Py:   json.loads(s)
来源：http://hz.bjfxy.top/gtbapjqate.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.pengpengdd.cyou/gtioeebjnz.html

JS:   JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtevqlzzqp.html

TS:   JSON.parse(s)
来源：http://hz.xziqi.cn/gtibhnqwkq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhixingplan.top/gteogxabkz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ydjk.org.cn/gtkydonapg.html

Ruby: JSON.parse(s)
来源：http://hz.cqqwz.cn/gtozvgvyqz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ehwqpu.com/gtrgrymgzg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.mhx1999.top/gtpugsqowe.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xylfe.cn/gtxzfwwwbt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gaohongyu789.top/gtxzsodcpz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.pycfn.com/gtebjosfil.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.dashuyun.cn/gteuqafsio.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinyuanbaomall.cn/gtoczzxthp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yongpay.top/gtsssjvgfb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydjk.org.cn/gtbmqfnefs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.fengsongda.top/gtacmjxmrr.html

[K04] 读取 JSON 文件
来源：http://hz.hywenlv.cn/gtohvndmlt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sweek.top/gtnijelxmb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hywenlv.cn/gtzmuaeobs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tanke756.top/gtjvyoavmp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtjagvovau.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jianghu66.top/gttkhhhrca.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhoulong.xyz/gtjcfsbwqd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.wangdashe.top/gtydusghzl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.wangdashe.top/gtowjyqwsu.html

[K05] 深拷贝对象
来源：http://hz.aibaodan.cn/gtnkoirrse.html

Py:   copy.deepcopy(obj)
来源：http://hz.52xcode.cn/gtiruxkrqh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yongpay.top/gtjhlhjhjf.html

JS:   structuredClone(obj)
来源：http://hz.bjfxy.top/gtqrjgiogu.html

TS:   structuredClone(obj)
来源：http://hz.tanke756.top/gtdftzsrao.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sysykeji.top/gteqfreqwt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yongpay.top/gtnelgxuxm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yangfankeji.com/gtppquzrky.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ywan-chungtsiang.top/gtxlrvcvhi.html

[K06] 解析 URL 查询串
来源：http://hz.zycfv.cn/gtrtgygyre.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.pycfn.com/gtunibkklu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gotoacloud.top/gtuorzxcex.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ivvv.top/gthufcmwzb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ivvv.top/gttjsbajhd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydjk.org.cn/gtoaybkjvd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gtnjkcddwa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sxryk.cn/gttbjmyzkz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.bjfxy.top/gtqwljsbcp.html

[K07] 进制转换
来源：http://hz.yanxiufei.cn/gtdmwfjqzr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenlongwang.top/gtorgdzjjf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gogol.net.cn/gtbfwkpewa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gthsrtogdk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtgpjrfuxn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtrnkkvcth.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jqgfzy.top/gtefdnnfmd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xylfe.cn/gthfeokmwy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cqqwz.cn/gtqzqyfdzj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj20258888.top/gtkpyouvqk.html

Py:   pickle.dumps(obj)
来源：http://hz.andypj.xyz/gtuatlpslh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhoulong.xyz/gtzglltvir.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.daria6918.cn/gtihrwfjpq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.aibaodan.cn/gtcdftpfdj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ydjk.org.cn/gtnyaspiqa.html

Go:   encoding/gob
来源：http://hz.tian-w.cn/gtwbwpivzf.html

Ruby: Marshal.dump(obj)
来源：http://hz.daria6918.cn/gtqyemzfqp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gzhubu.top/gtucwhfuwf.html

================================================================================
来源：http://hz.gzhubu.top/gthknyyfqp.html

L. 网络请求
来源：http://hz.cdnleiting.top/gtnyrhrqul.html

================================================================================
来源：http://hz.guowangkeji.top/gturwyuyyw.html

[L01] 发送 GET 请求
来源：http://hz.52xcode.cn/gtztvzkhfk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gogol.net.cn/gtlfdjbpjf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinyuanbaomall.cn/gteussxvny.html

JS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtxvikepfp.html

TS:   await fetch(url)
来源：http://hz.jiagoushi.top/gtifzgypna.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sweek.top/gthbudkfql.html

Go:   resp, err := http.Get(url)
来源：http://hz.yonumen.top/gtngzflqge.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zycfv.cn/gtwitrhuvm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.aizwys.cn/gtykwnohcd.html

[L02] 发送 POST JSON
来源：http://hz.pycfn.com/gtbswkekap.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.iojbl.cn/gtsduhxzwn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hnxiangtu.top/gttfmnsazu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hammf.cn/gtdjcyxdhd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtmjerevzv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jqgfzy.top/gthmwbwhwy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.quarkkingdee.top/gtputuzqjz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgufenzy.top/gtprhgprrv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zycfv.cn/gtqzjnkvek.html

[L03] 设置自定义请求头
来源：http://hz.cheryme.top/gthvewhozo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.52xcode.cn/gtunsibbts.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xingfuxueyuan.xyz/gtaqoqujqy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gtkwvehkur.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zycfv.cn/gtjfitwfoc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cheryme.top/gtjjnvllbc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cucudq.cn/gtkiqzxrhv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tanke756.top/gteokmzaix.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhoulong.xyz/gtlyrbpduw.html

[L04] 设置超时
来源：http://hz.pycfn.com/gtbecvewmo.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gogol.net.cn/gtocmjnuko.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cucudq.cn/gtmnednjll.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yangfankeji.com/gtldcxudqk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.svipenyu.cn/gtlofbgxru.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhongyouzk.top/gtyoeerdfe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.iojbl.cn/gtfisxmlvs.html


<!-- 参考信息 -->