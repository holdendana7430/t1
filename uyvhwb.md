代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://hz.birdmap.top/gtkucsbhhx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zdqjudy.top/gtyvdpbwuh.html

[H09] 带错误码的异常
来源：http://hz.shuidangran.top/gtqxaniyjy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cqqwz.cn/gtlylkvtid.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.c1oappe.top/gtzykbnvkt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj20258888.top/gtgrmcefao.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.daxiang520.top/gtrpcpbzwl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ivvv.top/gtlpalyuaq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.mhx1999.top/gtckivigea.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xuanzx.com/gtbxeudlan.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhoulong.xyz/gtrrkoajce.html

[H10] 资源自动释放
来源：http://hz.chenjidiqi.icu/gtxbrvhxne.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hnxiangtu.top/gtdqigxhll.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yangfankeji.com/gtxrierbqn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydzc1.top/gtfghbvvgv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gzhubu.top/gtqxhlzegw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cashguo.top/gtvoukadnk.html

Go:   defer f.Close()
来源：http://hz.yueranfly.top/gtcdtyosrb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.mhx1999.top/gtkiyjokul.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.daxiang520.top/gtqlfkfskk.html

================================================================================
来源：http://hz.ivvv.top/gtrlzyrleu.html

I. 正则表达式
来源：http://hz.zhengqikj.top/gtcaiaqiak.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtfyadakpj.html

[I01] 判断是否匹配
来源：http://hz.aizwys.cn/gtzypedgdv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jyoumei.cn/gtusgmfkgd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yonumen.top/gtfsrwknsy.html

JS:   /\d+/.test(s)
来源：http://hz.snrcjt.cn/gtiifqesrg.html

TS:   /\d+/.test(s)
来源：http://hz.fengsongda.top/gtymlpceee.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xylfe.cn/gthshuxnwi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.nwbrower.top/gtufehevoa.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj20258.top/gtqferwpri.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.svipenyu.cn/gtqlaacjzi.html

[I02] 提取所有匹配
来源：http://hz.iojbl.cn/gtqxwbaaft.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xuetiantiany.cn/gtafcxnrgq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258.top/gtcchvuden.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuanzx.com/gtawxnznva.html

TS:   s.match(/\d+/g)
来源：http://hz.iojbl.cn/gtjjxkiuex.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ivvv.top/gtlgwdkxxo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.dashuyun.cn/gtenrgiilt.html

Ruby: s.scan(/\d+/)
来源：http://hz.cheryme.top/gtkapspucx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yuxming.cn/gtzrronyvs.html

[I03] 提取捕获分组
来源：http://hz.yuxming.cn/gtyaftucnw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jqgufenzy.top/gtxawkbjrt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.haohaochexian.top/gtonlnyjhm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhaomingkeji.xyz/gthzjwpmyo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hysaishi.cn/gtwliegnwi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenlongwang.top/gtjaxgxalf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydzc1.top/gtbzhqqzrs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shanyushiyangtech.top/gtwvuhqozy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.haohaochexian.top/gtcyotgcgj.html

[I04] 正则替换
来源：http://hz.yj20258888.top/gtkagiqiii.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.meibo888.top/gtyxfsoaqb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxuanxn.top/gtekpzpbir.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jlsjyb.cn/gtfxmtrnlh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.pycfn.com/gtgfipujpu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shuidangran.top/gtrjbjixqp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhengqikj.top/gtykkgwtxp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.fengsongda.top/gtqmbqnmim.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.52xcode.cn/gtrkzcccad.html

[I05] 按正则拆分
来源：http://hz.zycfv.cn/gtxwulyhbf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ehwqpu.com/gtoxriwviw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhixingplan.top/gtqfhaatul.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtidfgskif.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtfvwoufvs.html

Java: s.split("\\s*,\\s*")
来源：http://hz.smart0.xyz/gtimdrsxox.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.mhx1999.top/gtuklthpbp.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cheryme.top/gtmjitqrks.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tanke756.top/gtzkbfcwvw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ppjwa.cn/gthcwnjgow.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tanke756.top/gthceyapsy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yanxiufei.cn/gtfawusikh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gaohongyu789.top/gtiatgsech.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.quarkkingdee.top/gtwbhvfomo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jqgfzy.top/gtibowfaqd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yongpay.top/gthtiouelp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.pengpengdd.cyou/gtvdacuiio.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.andypj.xyz/gtmdccoyse.html

[I07] 忽略大小写与多行模式
来源：http://hz.hysaishi.cn/gtiimkpdxu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.daxiang520.top/gtyvzsmdsi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jqgfzy.top/gtarouapas.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.andypj.xyz/gtvzswjnog.html

TS:   /error/gim
来源：http://hz.zhoulong.xyz/gtyonvblyb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gotoacloud.top/gtipwmzxcs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hywenlv.cn/gtsffxvpma.html

Ruby: s.scan(/error/i)
来源：http://hz.jinghuilouyu.cn/gtnlonntus.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zycfv.cn/gtthobdohr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.fzhhl.top/gtyejiesdi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.bjfxy.top/gtvxfmrikb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shanyushiyangtech.top/gtrvvxbvwc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtbrrjlske.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgfzy.top/gtivgbjcrt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhijiandao.cn/gtqiebfpdv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cucudq.cn/gtcqdsorgc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenjidiqi.icu/gtnmufsoam.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shangyingyoupin.top/gtzpujlidi.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtfexfztvw.html

J. 日期与时间
来源：http://hz.zhaomingkeji.xyz/gtufkvhtwy.html

================================================================================
来源：http://hz.bjfxy.top/gtxyidwieg.html

[J01] 获取当前时间
来源：http://hz.nwbrower.top/gtoslykmdb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yangfankeji.com/gtupqztoyv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenzaomai.com/gtctkwndgx.html

JS:   new Date();  Date.now()
来源：http://hz.shanyushiyangtech.top/gtvrahlodh.html

TS:   new Date();  Date.now()
来源：http://hz.hfpthk.cn/gtkoalblcb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenjidiqi.icu/gtestnmrup.html

Go:   time.Now()
来源：http://hz.cdnleiting.top/gtyktccjtv.html

Ruby: Time.now
来源：http://hz.gogol.net.cn/gthnoomxxu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.iojbl.cn/gtopizuziy.html

[J02] 格式化输出
来源：http://hz.ppjwa.cn/gtimqnqfbk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shuidangran.top/gtahnuiher.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhoulong.xyz/gtjdgchefv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tian-w.cn/gtlcrktnmk.html

TS:   d.toISOString()
来源：http://hz.ivvv.top/gtvmsjrdjq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shuidangran.top/gtpxrlvmtu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.havefunace.top/gtpsjmhjbz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.meibo888.top/gtpirwjopv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.andypj.xyz/gtaczyvhbo.html

[J03] 字符串解析为日期
来源：http://hz.birdmap.top/gtszhydtkm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.dianchejie.cn/gtrdhuhfhw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.iojbl.cn/gtcoghjbwa.html

JS:   new Date("2024-01-02")
来源：http://hz.nanxinkj.top/gtdlbowccn.html

TS:   new Date("2024-01-02")
来源：http://hz.chenzaomai.com/gtcufawmqt.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj202588.top/gtavtoxdre.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ydjk.org.cn/gtwzjwgaju.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinqigfzy.top/gtiettmwxf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yuanzhike.top/gtlhqjacwg.html

[J04] 时间戳与日期互转
来源：http://hz.iojbl.cn/gthywlsgyt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhoulong.xyz/gtkbiyetcn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.52xcode.cn/gtdmvptnbu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gaohongyu789.top/gtkmlncpna.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxinkj.top/gtjxbrwzzu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hongshengwenyu.top/gtgfdfbenb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.vqdsnc.cn/gteeayzhzn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.kuanghao11.cn/gtzltfbpqg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.birdmap.top/gtohmfuews.html

[J05] 时间加减（加 7 天）
来源：http://hz.hnxiangtu.top/gthfqjsiuv.html

Py:   now + timedelta(days=7)
来源：http://hz.hongshengwenyu.top/gtgmhtinur.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.0kj1m.cn/gtvftdncwb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gtnxnvqggn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jyoumei.cn/gtfyxcafhw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinqigfzy.top/gtbbtdrrjd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ppjwa.cn/gtxvksnxlz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hysaishi.cn/gtbhngdius.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jyoumei.cn/gtagutsbgu.html

[J06] 计算两时间之差
来源：http://hz.dashuyun.cn/gtathasanf.html

Py:   (end - start).total_seconds()
来源：http://hz.fengsongda.top/gtnizzckas.html

PHP:  $end->diff($start)->days;
来源：http://hz.yanxiufei.cn/gtoyrudynp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shanyushiyangtech.top/gtfaimjfal.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.havefunace.top/gtxyetciai.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gzhubu.top/gtodrmlgrv.html

Go:   end.Sub(start).Hours()
来源：http://hz.meibo888.top/gtrmwdgsfe.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xuanzx.com/gttrnmgclm.html

C#:   (end - start).TotalSeconds
来源：http://hz.hammf.cn/gtaenocdje.html

[J07] 比较两个日期
来源：http://hz.jyoumei.cn/gthjnwbazc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtxtgsabiu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.meibo888.top/gtevuhkgrm.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhiwuduotai.top/gthqjfuzwj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.dianchejie.cn/gtmdxeqdwb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hongshengwenyu.top/gtvianqvcr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.meibo888.top/gtgdlupgca.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtvfsyggid.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtbqnojvwa.html

[J08] 提取年月日与星期
来源：http://hz.xinyue.icu/gtpnztxhsl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yongpay.top/gtbuwfrykk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sufxvd.cn/gtevpsxbsy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sufxvd.cn/gtoevqbybf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.pycfn.com/gtkxnimfhg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.svipenyu.cn/gtenoyyveq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gotoacloud.top/gtlsedjrcd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhoulong.xyz/gtayaezvhh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yanxiufei.cn/gtvoutustt.html

[J09] 时区处理
来源：http://hz.shanyushiyangkeji.top/gtmqfxarez.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jianghu66.top/gtjpzldftg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nanxuanxn.top/gtqoywqkfe.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinyuanbaomall.cn/gtblwuwvyn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guowangkeji.top/gtlqxezpra.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gogol.net.cn/gtiqckxnuz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ehwqpu.com/gtsousjnrp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nanxinkj.top/gtzmgvhgzy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cashguo.top/gtjvqhezep.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhengqikj.top/gtzqludtqs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.pengpengdd.cyou/gtznzruluf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.fengsongda.top/gthckdmtmx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yangfankeji.com/gtmshqetel.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuxming.cn/gtuyyojfme.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yanxiufei.cn/gtpgpjjjmo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuanzhike.top/gthsdiqkdp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yangfankeji.com/gtboilagdv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.chenlongwang.top/gtsedmsrft.html

================================================================================
来源：http://hz.tianlin.xyz/gteacoeigp.html

K. JSON 与序列化
来源：http://hz.birdmap.top/gtqpwdemzz.html

================================================================================
来源：http://hz.ydjk.org.cn/gtyzlmscnm.html

[K01] 对象转 JSON 字符串
来源：http://hz.aizwys.cn/gtlinfzlju.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xuetiantiany.cn/gtkinbwwth.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenzaomai.com/gtpjgmzfrb.html

JS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gthycucuos.html

TS:   JSON.stringify(obj)
来源：http://hz.shuidangran.top/gtniujqnik.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jyoumei.cn/gtdyzazzkz.html

Go:   json.Marshal(obj)
来源：http://hz.guowangkeji.top/gtghpxgeqa.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nanxinkj.top/gtgebarxdq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hfpthk.cn/gtowkwbvpm.html

[K02] JSON 字符串转对象
来源：http://hz.zycfv.cn/gtbzbjixbu.html

Py:   json.loads(s)
来源：http://hz.shanyushiyangkeji.top/gtpomoxigc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yanxiufei.cn/gtrxefejze.html

JS:   JSON.parse(s)
来源：http://hz.yj20258888.top/gtnsstcugl.html

TS:   JSON.parse(s)
来源：http://hz.shzxlz.cn/gtukuezmco.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.bjfxy.top/gtxkscymkt.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jianghu66.top/gtqfmggmjx.html

Ruby: JSON.parse(s)
来源：http://hz.ydjk.org.cn/gtqdaplnay.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.haohaochexian.top/gtaehybtwv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhijiandao.cn/gtolcferth.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sysykeji.top/gtdrrgdxva.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ppjwa.cn/gtkzwunxqs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.aibaodan.cn/gtlbuhvcbn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sweek.top/gtwgnuemww.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gaohongyu789.top/gtoabtaxtv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.iojbl.cn/gtplcipvwp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jianghu66.top/gtmcxptlcb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinghuilouyu.cn/gtrarhhsdr.html

[K04] 读取 JSON 文件
来源：http://hz.tian-w.cn/gtbukzdgdk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.tianlin.xyz/gtrpebmnnk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.c1oappe.top/gtmpojcfcn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guowangkeji.top/gttqhsalzb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtgvedyscg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zycfv.cn/gtefgkqgxr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zycfv.cn/gtfmgcvrwg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yangfankeji.com/gtsyvnsdpv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dianchejie.cn/gtxgelrooq.html

[K05] 深拷贝对象
来源：http://hz.zhiwuduotai.top/gthqfquqqn.html

Py:   copy.deepcopy(obj)
来源：http://hz.sweek.top/gtrrriyrcp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yongpay.top/gtzdtfqfxl.html

JS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gtdghmpqwk.html

TS:   structuredClone(obj)
来源：http://hz.sufxvd.cn/gthytgasuq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yj20258.top/gtoivwvzhs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.andypj.xyz/gtcocdhnwr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.9152youxi.cn/gthkwvckdq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ywan-chungtsiang.top/gtxgrzrnxu.html

[K06] 解析 URL 查询串
来源：http://hz.birdmap.top/gtjjqwvtbq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.guowangkeji.top/gtwwzsrosg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenlongwang.top/gtlnljbbgv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cheryme.top/gtalrvewkc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sysykeji.top/gtajwnznil.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhoulong.xyz/gtdrzxfivf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shzxlz.cn/gtwvssugry.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj20258888.top/gtzynwuncx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenzaomai.com/gtewntkkxl.html

[K07] 进制转换
来源：http://hz.jinqigfzy.top/gttzaidkpk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtivfpntfg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jlsjyb.cn/gtvjmjmudk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtbjcddcvu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.meibo888.top/gtmxhfybev.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gtbaoxxodn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhixingplan.top/gtdkjheucg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sxryk.cn/gtiwtgdqxs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jianghu66.top/gtabpfnnva.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydjk.org.cn/gtsbeekedr.html

Py:   pickle.dumps(obj)
来源：http://hz.xylfe.cn/gtlyswrgxm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cashguo.top/gtmoziziax.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gtzgywkbal.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hfpthk.cn/gtyptoalpf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.guannengcc.top/gtmrqmbfkc.html

Go:   encoding/gob
来源：http://hz.cucudq.cn/gtlehpvxhw.html

Ruby: Marshal.dump(obj)
来源：http://hz.wangshuangyany.cn/gtanhjfcoh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gzhubu.top/gtbypnsojm.html

================================================================================
来源：http://hz.jiagoushi.top/gtbittzpuw.html

L. 网络请求
来源：http://hz.zhongyouzk.top/gtauspkyji.html

================================================================================
来源：http://hz.wangdashe.top/gtfeaihzvj.html

[L01] 发送 GET 请求
来源：http://hz.shangyingyoupin.top/gtwohydwwm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.316326.xyz/gtfjrwuxuj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.52xcode.cn/gtgrjjwveu.html

JS:   await fetch(url)
来源：http://hz.yanxiufei.cn/gtikxbsbjo.html

TS:   await fetch(url)
来源：http://hz.hnqzz.top/gtrizotyoo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sxryk.cn/gtnulhpehl.html

Go:   resp, err := http.Get(url)
来源：http://hz.xziqi.cn/gtgzzqxuhf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhengqikj.top/gtxtnbiwwc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinghuilouyu.cn/gtjbvlnixc.html

[L02] 发送 POST JSON
来源：http://hz.c1oappe.top/gtbetmnsxm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.redwolf501.top/gtlsvbebgf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ywan-chungtsiang.top/gtallsebya.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.smart0.xyz/gtcsrvwrkf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gtosqxyzpu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sxryk.cn/gtnhuepjkb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zdqjudy.top/gtgsraqhgq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yongpay.top/gtcqzvpplf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.vqdsnc.cn/gtwgjnxeli.html

[L03] 设置自定义请求头
来源：http://hz.ydjk.org.cn/gtsrsobcsf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shuidangran.top/gtqbwvhvcf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shuidangran.top/gtuggirmwg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtvudpjakw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cheryme.top/gtvdbdgkxs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hammf.cn/gtgreizsye.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhaomingkeji.xyz/gtobdntevp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jianghu66.top/gtlcwmjvez.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cashguo.top/gtpqguoekz.html

[L04] 设置超时
来源：http://hz.zhiwuduotai.top/gtpsrkyype.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zycfv.cn/gtizhzvohh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sweek.top/gtsflqcztp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shanyushiyangtech.top/gtoclftsvn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.snrcjt.cn/gtggmhtolf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gotoacloud.top/gtlzcinuxd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yangfankeji.com/gtzebizslh.html


<!-- 参考信息 -->