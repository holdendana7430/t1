代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jiagoushi.top/gtekqzzcws.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xziqi.cn/gtkviuezcz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shanyushiyangtech.top/gttbaobahm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gotoacloud.top/gtbkoiqamh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yangfankeji.com/gtxmbchzqr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gaohongyu789.top/gtaxzkmqcy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xinyue.icu/gtroeaeyao.html

[H10] 资源自动释放
来源：http://hz.yj202588.top/gtdvjngipr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.quarkkingdee.top/gtzykoswzw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sysykeji.top/gtmjbtunpn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jianghu66.top/gttoqdqzca.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj202588.top/gthaivoxxn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nwbrower.top/gtboqfsfei.html

Go:   defer f.Close()
来源：http://hz.yongpay.top/gtusyarhit.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.wangshuangyany.cn/gtzjwdshoi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yongpay.top/gtcwlhvbrw.html

================================================================================
来源：http://hz.gzhubu.top/gtfrdlbybd.html

I. 正则表达式
来源：http://hz.aizwys.cn/gtytdgjgry.html

================================================================================
来源：http://hz.cheryme.top/gtuqjhjxrk.html

[I01] 判断是否匹配
来源：http://hz.dashuyun.cn/gtdmpjzpeh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ywan-chungtsiang.top/gticscjzda.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sxryk.cn/gttzwlciea.html

JS:   /\d+/.test(s)
来源：http://hz.xziqi.cn/gtgejupzln.html

TS:   /\d+/.test(s)
来源：http://hz.zhoulong.xyz/gtpgkefezm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.andypj.xyz/gtqqvwhtuz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.feifeiyinyue.top/gtvzhqjgad.html

Ruby: s.match?(/\d+/)
来源：http://hz.tanke756.top/gtxlwlwrwc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jlsjyb.cn/gtgroecxfa.html

[I02] 提取所有匹配
来源：http://hz.guannengcc.top/gtqychdxcd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shzxlz.cn/gtdmiymepi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.redwolf501.top/gtababytur.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shangyingyoupin.top/gtbyjrmtbe.html

TS:   s.match(/\d+/g)
来源：http://hz.xziqi.cn/gthgzopfug.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.andypj.xyz/gtezntafra.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guowangkeji.top/gtlvwtyypj.html

Ruby: s.scan(/\d+/)
来源：http://hz.yonumen.top/gtqnfdcvbl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hfpthk.cn/gtqyknqdcq.html

[I03] 提取捕获分组
来源：http://hz.zhixingplan.top/gtkmeukplw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.haohaochexian.top/gtddullnqu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.iojbl.cn/gtnulpttoe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shuidangran.top/gtqetomdup.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ppjwa.cn/gtyrcaarli.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shangyingyoupin.top/gtripqfeen.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhaomingkeji.xyz/gtwoimkcas.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ydjk.org.cn/gtvchhcofr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.wangshuangyany.cn/gtbroedrnt.html

[I04] 正则替换
来源：http://hz.yuanzhike.top/gtyyecbltb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yuxming.cn/gttcentakx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xuanzx.com/gtrqtfhudy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhixingplan.top/gtbadxpfiw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.fengsongda.top/gtivetvwrs.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.daxiang520.top/gtwytmixac.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cucudq.cn/gtltncpcoy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhongyouzk.top/gtyqbgdzrb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.smart0.xyz/gtqwfywzbt.html

[I05] 按正则拆分
来源：http://hz.yj20258888.top/gtyqepnnos.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tian-w.cn/gtelykjfew.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tanke756.top/gtyvjplbva.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.pycfn.com/gtymglgnee.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sufxvd.cn/gtlrpfrxdi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.redwolf501.top/gtcakuucwt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yuxming.cn/gtdjfkwkxl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtskpcuker.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tianlin.xyz/gtdexspjbj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.wangdashe.top/gtymqnodlu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.birdmap.top/gtoibazmit.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.iojbl.cn/gtempuzdep.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xylfe.cn/gtttzygmic.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gzhubu.top/gtxjvntbsy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.feifeiyinyue.top/gtwaxevrmi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cheryme.top/gtqkicazwp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj20258888.top/gtbaxnhtyo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtefiwqbeu.html

[I07] 忽略大小写与多行模式
来源：http://hz.zdqjudy.top/gtrqvdhbtw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ywan-chungtsiang.top/gtzdjyeipy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.dashuyun.cn/gtrcyoajlf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yonumen.top/gtbogobpzx.html

TS:   /error/gim
来源：http://hz.hnqzz.top/gtxmnpgcha.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhixingplan.top/gthywbwvdc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.smart0.xyz/gtnubwudnm.html

Ruby: s.scan(/error/i)
来源：http://hz.ybcxt.top/gtunpindwk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.dianchejie.cn/gtkwcgnrqn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cdnleiting.top/gtplxaeykk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhoulong.xyz/gtjdflmhhk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenjidiqi.icu/gtgroqlwzd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnqzz.top/gtmvotevnn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xinyue.icu/gtfoqreaqj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yueranfly.top/gtvrtbrcwp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinghuilouyu.cn/gtnrmyurjk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zycfv.cn/gtngnfeizp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cheryme.top/gtbpbzowpo.html

================================================================================
来源：http://hz.nwbrower.top/gtmlnrhifg.html

J. 日期与时间
来源：http://hz.tianlin.xyz/gtoxymnrli.html

================================================================================
来源：http://hz.zhijiandao.cn/gttuuuescq.html

[J01] 获取当前时间
来源：http://hz.chenlongwang.top/gtwdfyerps.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.andypj.xyz/gtmorcmcsr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gtiqzgbhpn.html

JS:   new Date();  Date.now()
来源：http://hz.yueranfly.top/gtsexojhgi.html

TS:   new Date();  Date.now()
来源：http://hz.fzhhl.top/gtgmgkfdbf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.snrcjt.cn/gtjvmmtnjv.html

Go:   time.Now()
来源：http://hz.sysykeji.top/gtgcguvkav.html

Ruby: Time.now
来源：http://hz.redwolf501.top/gtkjzswuuf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tanke756.top/gtmshibzvl.html

[J02] 格式化输出
来源：http://hz.cqqwz.cn/gttqqjsebx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuetiantiany.cn/gtewhoqori.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinqigfzy.top/gtntujjzbu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jiagoushi.top/gtuqlfaoiu.html

TS:   d.toISOString()
来源：http://hz.cucudq.cn/gtaoprtrmk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yonumen.top/gteacrivlx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.316326.xyz/gtiiumcnvt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnqzz.top/gtotssmokz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hysaishi.cn/gtahmtpkxg.html

[J03] 字符串解析为日期
来源：http://hz.yanxiufei.cn/gtvgfjgeel.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sxryk.cn/gtmwqvcwnk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xuetiantiany.cn/gtxztmzgga.html

JS:   new Date("2024-01-02")
来源：http://hz.hammf.cn/gtdfuwibbl.html

TS:   new Date("2024-01-02")
来源：http://hz.andypj.xyz/gtjzimmwya.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xziqi.cn/gtfgidxsaa.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hfpthk.cn/gtnlqceujy.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gogol.net.cn/gtzuubrjii.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sxryk.cn/gtrmjujjlm.html

[J04] 时间戳与日期互转
来源：http://hz.sysykeji.top/gtmlnrcxcr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuxming.cn/gtmsaqzzaj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hnxiangtu.top/gtqexetuiw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shanyushiyangkeji.top/gtdzgolmbz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hnxiangtu.top/gtljldxcjq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sxryk.cn/gtunshnmlm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tian-w.cn/gtoyvcellg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhengqikj.top/gtmkzcockf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xuanzx.com/gtnfioglkb.html

[J05] 时间加减（加 7 天）
来源：http://hz.gaohongyu789.top/gtkoyuhlbr.html

Py:   now + timedelta(days=7)
来源：http://hz.zhengqikj.top/gtsnafpnwf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.fengsongda.top/gtyubqkxta.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sysykeji.top/gtoajtvncp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgufenzy.top/gtunonyvca.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.snrcjt.cn/gtbxxdkbzk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.snrcjt.cn/gtndrpqnmz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.svipenyu.cn/gtsvvxzaga.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xziqi.cn/gtkpnbbovf.html

[J06] 计算两时间之差
来源：http://hz.zhongyouzk.top/gtzacfbszt.html

Py:   (end - start).total_seconds()
来源：http://hz.xuetiantiany.cn/gtuitljazp.html

PHP:  $end->diff($start)->days;
来源：http://hz.jqgufenzy.top/gtpwlljiul.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gotoacloud.top/gtiqudshnk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jlsjyb.cn/gtlhpxwhoy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gaohongyu789.top/gtcofdjtec.html

Go:   end.Sub(start).Hours()
来源：http://hz.yvedp.cn/gtdzqwrvbx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.9152youxi.cn/gtpzxtajkd.html

C#:   (end - start).TotalSeconds
来源：http://hz.fengsongda.top/gtvkdnxhgw.html

[J07] 比较两个日期
来源：http://hz.sufxvd.cn/gtynoehgws.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xuanzx.com/gthdzgaris.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jlsjyb.cn/gtbtddbbrm.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtebbvwthq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jyoumei.cn/gtmgsckjxr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jianghu66.top/gtpgvffzyr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.wangshuangyany.cn/gtavzxsmzy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtndgcediu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtpfzhjusa.html

[J08] 提取年月日与星期
来源：http://hz.sufxvd.cn/gtksrisdft.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hongshengwenyu.top/gtlubjwuxz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgfzy.top/gtnpfejwgq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.kuanghao11.cn/gteprruiia.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhoulong.xyz/gtqesyrkzc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.feifeiyinyue.top/gtwfdabsvg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinqigfzy.top/gteyimukxe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hfpthk.cn/gtchorhoub.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guannengcc.top/gttfjiavbp.html

[J09] 时区处理
来源：http://hz.quarkkingdee.top/gtueawlymg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangkeji.top/gtimvxoyqf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ehwqpu.com/gtasehsqfl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtbvdoivzc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenzaomai.com/gtzzqfpabb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aibaodan.cn/gtjyxutudv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zdqjudy.top/gtvzigdrtm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jqgufenzy.top/gtisfkvnsa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shuidangran.top/gthrmkbasu.html

[J10] 取今天 / 本月第一天
来源：http://hz.iojbl.cn/gthejieuvb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.0kj1m.cn/gtbnzthqoc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ybcxt.top/gtuafzzcll.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jiagoushi.top/gthhqaisuk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.birdmap.top/gtgjeikcta.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj202588.top/gtzxeqauhf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tanke756.top/gtddidgubp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.316326.xyz/gtpzklsnnu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.daxiang520.top/gtpikndzcv.html

================================================================================
来源：http://hz.316326.xyz/gtelldqnca.html

K. JSON 与序列化
来源：http://hz.hnqzz.top/gtbelrsbkm.html

================================================================================
来源：http://hz.yangfankeji.com/gtfaeaodbe.html

[K01] 对象转 JSON 字符串
来源：http://hz.pengpengdd.cyou/gtdkmkqimy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yueranfly.top/gtrvrkmcbs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gttgckosfm.html

JS:   JSON.stringify(obj)
来源：http://hz.yuxming.cn/gtgbwjfaip.html

TS:   JSON.stringify(obj)
来源：http://hz.sweek.top/gttktxbcft.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hnqzz.top/gtpidozlfi.html

Go:   json.Marshal(obj)
来源：http://hz.yueranfly.top/gtdswljvcs.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jqgfzy.top/gtbtuxvdnw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.pengpengdd.cyou/gtwqztalnd.html

[K02] JSON 字符串转对象
来源：http://hz.yj20258.top/gtpvrmkbmx.html

Py:   json.loads(s)
来源：http://hz.yongpay.top/gtwuvjgvdo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cdnleiting.top/gtioxoufnl.html

JS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gtxwrabsqf.html

TS:   JSON.parse(s)
来源：http://hz.pengpengdd.cyou/gtrtdtposd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.bjfxy.top/gtelphlxez.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinqigufen.top/gtjekuehnf.html

Ruby: JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtjfjqlizi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.mhx1999.top/gtxcsctwkh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yj20258.top/gtaqhhobmz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhijiandao.cn/gthultfbga.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ybcxt.top/gtvjoxaavm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gtaznaoaba.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gtttbsnxrg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinqigufen.top/gthdvmgike.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.quarkkingdee.top/gtefvjqvfh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nwbrower.top/gtkoxhjdxl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ydzc1.top/gtffwicyhy.html

[K04] 读取 JSON 文件
来源：http://hz.jianghu66.top/gtafytnoql.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shanyushiyangkeji.top/gtrnayofkv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.svipenyu.cn/gtlgpgzyru.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aizwys.cn/gtohcllqfi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtmkpbcvkc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xziqi.cn/gtgizgsakf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtcirnykgb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigfzy.top/gtmltorshz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.wangdashe.top/gtchtcvuzt.html

[K05] 深拷贝对象
来源：http://hz.fengsongda.top/gtprklbkou.html

Py:   copy.deepcopy(obj)
来源：http://hz.yangfankeji.com/gtmpkrluxf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cashguo.top/gtmaffdbyx.html

JS:   structuredClone(obj)
来源：http://hz.xziqi.cn/gtovdpfzbl.html

TS:   structuredClone(obj)
来源：http://hz.gaohongyu789.top/gttfgnmpkx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.pengpengdd.cyou/gteixjcwhx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.kuanghao11.cn/gtmxutmnoz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.snrcjt.cn/gtbapqucvs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hammf.cn/gtuvyvwaiu.html

[K06] 解析 URL 查询串
来源：http://hz.zhixingplan.top/gtedwtzyww.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yonumen.top/gtkokvbhhe.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhoulong.xyz/gtyrbnwupu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtpfdnipdu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dianchejie.cn/gtuifuxqjg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinqigufen.top/gtrfxvfxao.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtkdmnevqf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtbpsphsge.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.havefunace.top/gtpjmgkphp.html

[K07] 进制转换
来源：http://hz.zhongyouzk.top/gtmzogpshy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.redwolf501.top/gtgpkcwunm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydzc1.top/gtywuwwxbg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtiwfynxnf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtvgykwlnx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.pycfn.com/gtwuzyphcq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhijiandao.cn/gtoxgkxrfy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhaomingkeji.xyz/gtyyvtmcyt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hysaishi.cn/gtviaybznw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj202588.top/gtvkwsksyo.html

Py:   pickle.dumps(obj)
来源：http://hz.52xcode.cn/gtjmdrboos.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yangfankeji.com/gtwrdakrmd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.iojbl.cn/gtsvqhhpup.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yonumen.top/gtouhmppkx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj20258.top/gtqtypnzwv.html

Go:   encoding/gob
来源：http://hz.yj20258888.top/gtsvgmoxnb.html

Ruby: Marshal.dump(obj)
来源：http://hz.nanxuanxn.top/gtqmywlshl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.wangdashe.top/gtbveocgdl.html

================================================================================
来源：http://hz.hnqzz.top/gtjlxvpsxv.html

L. 网络请求
来源：http://hz.52xcode.cn/gtwxuwloys.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtoovknimz.html

[L01] 发送 GET 请求
来源：http://hz.ywan-chungtsiang.top/gtgdepxihx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zycfv.cn/gtkeaaaezs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydzc1.top/gtmbmpjvkn.html

JS:   await fetch(url)
来源：http://hz.sweek.top/gteejxykdx.html

TS:   await fetch(url)
来源：http://hz.sysykeji.top/gteqqsmeom.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.tianlin.xyz/gtoasgxnvb.html

Go:   resp, err := http.Get(url)
来源：http://hz.smart0.xyz/gtjuluhyvq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.bjfxy.top/gtbqcjeica.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yvedp.cn/gtebbxdtrb.html

[L02] 发送 POST JSON
来源：http://hz.pycfn.com/gtprgszonb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgfzy.top/gtwonufqvg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.smart0.xyz/gtfwmwyxvi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangdashe.top/gtmjpvqklc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gtohigujwh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.tianlin.xyz/gtndwdudcq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yonumen.top/gtlgnpjnoq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hywenlv.cn/gttwslmqeb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenjidiqi.icu/gtdnrxpsze.html

[L03] 设置自定义请求头
来源：http://hz.sxryk.cn/gtzmdwtysf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nwbrower.top/gtejvlfxjw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jqgufenzy.top/gtcsaxecop.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtcyizpiuv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sysykeji.top/gttzlvfapc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shanyushiyangtech.top/gtnvajwpzn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.c1oappe.top/gtbfszfwfv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sxryk.cn/gtuvpluxzi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tian-w.cn/gthwsmkgan.html

[L04] 设置超时
来源：http://hz.zhixingplan.top/gtjwekjhne.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jianghu66.top/gtypnayuhh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.chenjidiqi.icu/gtazwnmiaw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cqqwz.cn/gtlkfzwcvm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gthjbiguao.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhijiandao.cn/gthtcrkeco.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.nanxuanxn.top/gtwbobujrb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.snrcjt.cn/gttovryotb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhongyouzk.top/gthqasywvf.html

[L05] 上传文件（multipart）
来源：http://hz.shangyingyoupin.top/gtekyzvtkh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zdqjudy.top/gtyzpwgbiy.html


<!-- 参考信息 -->