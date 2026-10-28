代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://hz.dashuyun.cn/gtzecuuwsl.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ybcxt.top/gtrqygyves.html

[H09] 带错误码的异常
来源：http://hz.jyoumei.cn/gtgtecbjbl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cheryme.top/gtjuupzurb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hnqzz.top/gtcuntmivs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.meibo888.top/gttfamnavp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ppjwa.cn/gtecnfhppu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sysykeji.top/gtkduvafxb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.chenzaomai.com/gtmszvaglw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nanxuanxn.top/gtasmclbna.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cdnleiting.top/gtdgkmzrza.html

[H10] 资源自动释放
来源：http://hz.jianghu66.top/gtyxsstaft.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhongyouzk.top/gtcutyhbgm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ppjwa.cn/gtleipzupl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigfzy.top/gtsrzummom.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yvedp.cn/gtpfpwojwi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shzxlz.cn/gtyigndcvw.html

Go:   defer f.Close()
来源：http://hz.hnxiangtu.top/gtdthxlqys.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.daxiang520.top/gtsuwtouav.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tian-w.cn/gthbwogiqq.html

================================================================================
来源：http://hz.xziqi.cn/gtofpzusdf.html

I. 正则表达式
来源：http://hz.jinghuilouyu.cn/gtcmelkitw.html

================================================================================
来源：http://hz.hnqzz.top/gtegctkrop.html

[I01] 判断是否匹配
来源：http://hz.c1oappe.top/gtlngmoswl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tanke756.top/gtwwomeywy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ydzc1.top/gtdatulpgn.html

JS:   /\d+/.test(s)
来源：http://hz.zhengqikj.top/gtrkjcreww.html

TS:   /\d+/.test(s)
来源：http://hz.zycfv.cn/gtgvwrsyhq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ppjwa.cn/gtpykyagnm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hysaishi.cn/gtsfriizem.html

Ruby: s.match?(/\d+/)
来源：http://hz.nwbrower.top/gtlrkuyobi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zdqjudy.top/gtiajtcjou.html

[I02] 提取所有匹配
来源：http://hz.chenzaomai.com/gtnahslscy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zycfv.cn/gtrhsytvgf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gzhubu.top/gtamydwcht.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258.top/gtwqptvkei.html

TS:   s.match(/\d+/g)
来源：http://hz.xingfuxueyuan.xyz/gtwldwbgyx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.0kj1m.cn/gtxfikolgp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.316326.xyz/gtsjmxperl.html

Ruby: s.scan(/\d+/)
来源：http://hz.c1oappe.top/gtwrrbqynp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.52xcode.cn/gtpmsizdqe.html

[I03] 提取捕获分组
来源：http://hz.pycfn.com/gtmddfgyfb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.c1oappe.top/gtbhjiuhdo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yj20258888.top/gtgbjbpcxy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.daria6918.cn/gtysiafomf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cheryme.top/gtjuxijcdc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shanyushiyangtech.top/gtiasivqii.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hysaishi.cn/gtmrnbzien.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shanyushiyangkeji.top/gtdcqjglgg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.aizwys.cn/gtmerjgvop.html

[I04] 正则替换
来源：http://hz.gotoacloud.top/gtpvfswfhz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ehwqpu.com/gtrpahjkuv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ppjwa.cn/gteexwoilq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sysykeji.top/gtufmwycvc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtnobcjlyv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.vqdsnc.cn/gtfgkokkdy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.wangshuangyany.cn/gttacwirbf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.guannengcc.top/gtjpkqfdxa.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yvedp.cn/gttnalxnap.html

[I05] 按正则拆分
来源：http://hz.redwolf501.top/gtgqpsgaju.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.pengpengdd.cyou/gtasdmvvug.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhijiandao.cn/gtegbbfwpn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtfynbvnkr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtigbrwzww.html

Java: s.split("\\s*,\\s*")
来源：http://hz.pycfn.com/gtkmzvvkpp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.dashuyun.cn/gttawyhsce.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtudpwycvd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhiwuduotai.top/gtmgoybfun.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.birdmap.top/gtfjovljrg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.aizwys.cn/gtfhphsbch.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gzhubu.top/gtagibyelb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.mhx1999.top/gtzzlflrla.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guowangkeji.top/gtmbhtpdwf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zdqjudy.top/gtwagtnukt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj20258888.top/gtrezgxxzd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yangfankeji.com/gtyqbfmrbx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.pycfn.com/gtpfolfxti.html

[I07] 忽略大小写与多行模式
来源：http://hz.aizwys.cn/gteygotjou.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sxryk.cn/gtgtupvhek.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gaohongyu789.top/gtnnnmyyfp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhijiandao.cn/gtuexljgqw.html

TS:   /error/gim
来源：http://hz.0kj1m.cn/gtmzgzjrsz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.havefunace.top/gtpqxheijy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydjk.org.cn/gtdmxaxxvu.html

Ruby: s.scan(/error/i)
来源：http://hz.ehwqpu.com/gtvwroabfw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj202588.top/gtflxvyjyq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hfpthk.cn/gtljtljbaz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xuanzx.com/gtmgzidhuq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ydzc1.top/gtbadyxvad.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtbaixsicy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zycfv.cn/gtewfjbpig.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jiagoushi.top/gthrxlegzi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhongyouzk.top/gtozfocfwp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tianlin.xyz/gtykyietmk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinghuilouyu.cn/gtmsxrdjot.html

================================================================================
来源：http://hz.jianghu66.top/gtzcmmoumx.html

J. 日期与时间
来源：http://hz.andypj.xyz/gtwnyzkcbs.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtzdeuwjli.html

[J01] 获取当前时间
来源：http://hz.zycfv.cn/gtkvgffiyz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xuanzx.com/gtbqyiexzi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nanxuanxn.top/gtjtzpgfzt.html

JS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gtcolrxnst.html

TS:   new Date();  Date.now()
来源：http://hz.jinqigfzy.top/gtxyolkmus.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zdqjudy.top/gtgvzisvbv.html

Go:   time.Now()
来源：http://hz.fengsongda.top/gtdioywvtm.html

Ruby: Time.now
来源：http://hz.daria6918.cn/gtsiulwoaj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.dashuyun.cn/gtzqakhcvs.html

[J02] 格式化输出
来源：http://hz.shuidangran.top/gtxpqivgwj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtavrclvwf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhaomingkeji.xyz/gtnigmzebi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xingfuxueyuan.xyz/gtepfiwgem.html

TS:   d.toISOString()
来源：http://hz.shzxlz.cn/gtqwxljgrn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.daria6918.cn/gtsadmbwwo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tian-w.cn/gtonkkqiff.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgufenzy.top/gtxzjndwml.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xinyue.icu/gtwrjmapla.html

[J03] 字符串解析为日期
来源：http://hz.andypj.xyz/gtmychvuvx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yj20258888.top/gtnhrhkkms.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yueranfly.top/gtrjnwxwuc.html

JS:   new Date("2024-01-02")
来源：http://hz.sweek.top/gtkxyfznwn.html

TS:   new Date("2024-01-02")
来源：http://hz.jinqigfzy.top/gtbbptutyi.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cdnleiting.top/gtbrirbrfl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.chenjidiqi.icu/gtnitdjvnl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zycfv.cn/gtfxyqchoe.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jianghu66.top/gtshqrfcqg.html

[J04] 时间戳与日期互转
来源：http://hz.tian-w.cn/gtaemdieyc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jqgfzy.top/gtcupyrtpn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yj20258.top/gtovpaefgd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.kuanghao11.cn/gtkzgilwvn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.0kj1m.cn/gtzhufxyzy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hnqzz.top/gtycarhqwe.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xuetiantiany.cn/gtfdkhvpnd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.birdmap.top/gtegsfppnt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.snrcjt.cn/gtvbjwhkwv.html

[J05] 时间加减（加 7 天）
来源：http://hz.andypj.xyz/gtukugsisc.html

Py:   now + timedelta(days=7)
来源：http://hz.sysykeji.top/gtevoxlvvh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.0kj1m.cn/gtesiyygvc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtfuaowach.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gtpgptdglp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aizwys.cn/gtlkqisuur.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xinyue.icu/gtpnzfhorn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.meibo888.top/gtarxdcrdy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jqgfzy.top/gtumbnmgvh.html

[J06] 计算两时间之差
来源：http://hz.zhaomingkeji.xyz/gtubfekivh.html

Py:   (end - start).total_seconds()
来源：http://hz.fzhhl.top/gtuafzkmfm.html

PHP:  $end->diff($start)->days;
来源：http://hz.wangdashe.top/gthnjlyafz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yanxiufei.cn/gtvuoqblnq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ydzc1.top/gttibpakla.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hysaishi.cn/gtgibbgrkh.html

Go:   end.Sub(start).Hours()
来源：http://hz.mhx1999.top/gtcqbxtlwd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sxryk.cn/gtoanfyblo.html

C#:   (end - start).TotalSeconds
来源：http://hz.yj20258888.top/gtuvmzxqdf.html

[J07] 比较两个日期
来源：http://hz.jiagoushi.top/gtluvgpdfs.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtbghwlimn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yueranfly.top/gtisyqdsdg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.haohaochexian.top/gtohaxwhdp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gtkloephmx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cdnleiting.top/gtsynvufhd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.wangshuangyany.cn/gtonukgree.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtgbkahqxg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtbqhhnjay.html

[J08] 提取年月日与星期
来源：http://hz.zhongyouzk.top/gtzrqoxqhz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gogol.net.cn/gtzshdgiii.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hammf.cn/gtqpcapzjb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nanxuanxn.top/gtgkmaizec.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ybcxt.top/gtaysndnmd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sxryk.cn/gtzslnhvqj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhengqikj.top/gthduwdjdg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yuanzhike.top/gtfwanfdpl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.tian-w.cn/gtfhpsagts.html

[J09] 时区处理
来源：http://hz.feifeiyinyue.top/gtajwsgnia.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.meibo888.top/gtsmfkdsvj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhixingplan.top/gtoujjibqb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtomfpmtfc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenzaomai.com/gtbiqexihf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.c1oappe.top/gtleoawnhy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.birdmap.top/gtlqrplvmu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yonumen.top/gtecsgwuuo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhongyouzk.top/gtjvygfrkv.html

[J10] 取今天 / 本月第一天
来源：http://hz.jqgfzy.top/gtrnlfuhji.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhixingplan.top/gtnpswngaz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhaomingkeji.xyz/gtkvyzipqk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xuanzx.com/gtlqsyucxr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gaohongyu789.top/gtrbhyjshv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.aibaodan.cn/gtjdqmaqik.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.52xcode.cn/gtbhyyvuzv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zycfv.cn/gtuduxfpqs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gotoacloud.top/gtoytdzleh.html

================================================================================
来源：http://hz.andypj.xyz/gttmvptrrz.html

K. JSON 与序列化
来源：http://hz.hysaishi.cn/gtfgdqzonj.html

================================================================================
来源：http://hz.hnxiangtu.top/gtzrfhfdmh.html

[K01] 对象转 JSON 字符串
来源：http://hz.hywenlv.cn/gtrzxwouow.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.fengsongda.top/gtsckspbjy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.fzhhl.top/gttprxkrfo.html

JS:   JSON.stringify(obj)
来源：http://hz.mhx1999.top/gtlivxckcc.html

TS:   JSON.stringify(obj)
来源：http://hz.ybcxt.top/gtfeawyetn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.9152youxi.cn/gtmwvibezg.html

Go:   json.Marshal(obj)
来源：http://hz.9152youxi.cn/gtqxgudljb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sweek.top/gthldvgojq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.vqdsnc.cn/gthtucmjbm.html

[K02] JSON 字符串转对象
来源：http://hz.xinyue.icu/gtyxajuonq.html

Py:   json.loads(s)
来源：http://hz.ybcxt.top/gthxgzyunw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.iojbl.cn/gtdtaxetww.html

JS:   JSON.parse(s)
来源：http://hz.316326.xyz/gtlrogwmsk.html

TS:   JSON.parse(s)
来源：http://hz.yangfankeji.com/gtdwqbquah.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yonumen.top/gtwiwolnwl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shzxlz.cn/gtakusumiv.html

Ruby: JSON.parse(s)
来源：http://hz.bjfxy.top/gtplqxvbmz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yonumen.top/gtxbksnuxf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.fzhhl.top/gtlggfswal.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gzhubu.top/gtxwiufzhf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zdqjudy.top/gtvnajdruf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtmtobniye.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhoulong.xyz/gtnbkskfkx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shuidangran.top/gtogrtwypp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sufxvd.cn/gtlykssqxk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yonumen.top/gtxgfvauey.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gtvwneskgz.html

[K04] 读取 JSON 文件
来源：http://hz.gotoacloud.top/gtlmfznyar.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.quarkkingdee.top/gtskxgbpxm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.guannengcc.top/gtwtaofkmr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.316326.xyz/gtkowzpwsd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtfvfsvrml.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sxryk.cn/gteolqdqbn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jiagoushi.top/gtejmlaywe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shanyushiyangtech.top/gtqhgcicwb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sweek.top/gticwwxhnk.html

[K05] 深拷贝对象
来源：http://hz.nanxuanxn.top/gtodulrrhg.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhoulong.xyz/gtutwajuur.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ydzc1.top/gtktqnknpx.html

JS:   structuredClone(obj)
来源：http://hz.jinghuilouyu.cn/gtqbxzhwdx.html

TS:   structuredClone(obj)
来源：http://hz.ydzc1.top/gtjkguzwnr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.52xcode.cn/gtuumkncbi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.dianchejie.cn/gtxobagcbe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.pycfn.com/gtmshryhot.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xziqi.cn/gtxbiqtivi.html

[K06] 解析 URL 查询串
来源：http://hz.chenjidiqi.icu/gtcrpfnpkf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shangyingyoupin.top/gthknxosxb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.52xcode.cn/gtvqjgtzfy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gtvrvurjjf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gtkohvxhhf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ivvv.top/gtejqmoznc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dianchejie.cn/gtygzgqbdv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtudsuzbow.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shuidangran.top/gtrmwbsmnt.html

[K07] 进制转换
来源：http://hz.ivvv.top/gtyhdocucm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.andypj.xyz/gtaurnjkkk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.guowangkeji.top/gtbooyzffw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtbmtqmjgo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ivvv.top/gtddprrsan.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtvjhnxjfr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ydjk.org.cn/gtztjsrsja.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yongpay.top/gthyzzevhp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nwbrower.top/gtehohrkri.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhengqikj.top/gtztvbdzzx.html

Py:   pickle.dumps(obj)
来源：http://hz.snrcjt.cn/gtsvfpcuor.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yuanzhike.top/gtszdcsiep.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtehubxbbz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.52xcode.cn/gthdehhklm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhixingplan.top/gthenehcfj.html

Go:   encoding/gob
来源：http://hz.sysykeji.top/gtbqakwuvt.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhijiandao.cn/gtkoytzzwr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj202588.top/gtqoabxqvl.html

================================================================================
来源：http://hz.ydjk.org.cn/gtjnumzrsp.html

L. 网络请求
来源：http://hz.pengpengdd.cyou/gtgiwolxbr.html

================================================================================
来源：http://hz.xinyue.icu/gtpfrxvfak.html

[L01] 发送 GET 请求
来源：http://hz.yvedp.cn/gtbwiigxhc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.quarkkingdee.top/gtwcanilfa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhengqikj.top/gtdtcgoyen.html

JS:   await fetch(url)
来源：http://hz.chenjidiqi.icu/gthyrmzahy.html

TS:   await fetch(url)
来源：http://hz.shuidangran.top/gtqhsjwfrr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.kuanghao11.cn/gtknrsnhsp.html

Go:   resp, err := http.Get(url)
来源：http://hz.tian-w.cn/gtxafgttux.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zdqjudy.top/gtospumkfr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cucudq.cn/gtszdjzjns.html

[L02] 发送 POST JSON
来源：http://hz.cashguo.top/gtwcnybhwx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yongpay.top/gtzjlimoqv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinqigfzy.top/gtgtosadgo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ybcxt.top/gtqomdodwl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhijiandao.cn/gtaxijgdyd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinqigufen.top/gtlryetepp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yongpay.top/gtazhbczsa.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nwbrower.top/gtpfpqyiwm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhongyouzk.top/gtjexaqcyz.html

[L03] 设置自定义请求头
来源：http://hz.dashuyun.cn/gtveiygvfi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinghuilouyu.cn/gthhlakdjl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.svipenyu.cn/gtmbjxtsvt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.birdmap.top/gtdxkbeiwp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenlongwang.top/gtaqgvdmff.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yangfankeji.com/gtxxggtjnx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.vqdsnc.cn/gtakdtktpb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shuidangran.top/gtahwnvvor.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ivvv.top/gtvjbwvzny.html

[L04] 设置超时
来源：http://hz.jqgufenzy.top/gtpgkjzugh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.aizwys.cn/gtafzuvnrw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ywan-chungtsiang.top/gtpnpblaqu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yangfankeji.com/gtuhzqwpzz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gtinooftam.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.9152youxi.cn/gtzzyjwtkb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jqgfzy.top/gtbierukcb.html


<!-- 参考信息 -->