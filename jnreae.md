代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cucudq.cn/gtampihvfp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.snrcjt.cn/gtkqwocbhm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.wangdashe.top/gtwwpownqc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenlongwang.top/gtwbdmvtoh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.birdmap.top/gtvkvnscrb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xinyue.icu/gtweqgooyd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydzc1.top/gtgiebzyfh.html

[H10] 资源自动释放
来源：http://hz.zdqjudy.top/gtnehrmnqk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinqigfzy.top/gtdyuoonzo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.guannengcc.top/gtzrjeqtdn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.quarkkingdee.top/gtnxbhvtlh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gtwuwbsull.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenzaomai.com/gtswsuzkto.html

Go:   defer f.Close()
来源：http://hz.chenlongwang.top/gtuomrulgo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.fengsongda.top/gtcceeqlzs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhixingplan.top/gtryntxzeg.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtblrdxlzk.html

I. 正则表达式
来源：http://hz.daxiang520.top/gtkfjyyjrb.html

================================================================================
来源：http://hz.jqgfzy.top/gtinxjavma.html

[I01] 判断是否匹配
来源：http://hz.jianghu66.top/gtffqnnung.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dashuyun.cn/gtujfefqrc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhoulong.xyz/gtgjmdywyu.html

JS:   /\d+/.test(s)
来源：http://hz.zhengqikj.top/gtapoqqfqj.html

TS:   /\d+/.test(s)
来源：http://hz.daria6918.cn/gtecvppdmc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ivvv.top/gtuwvujcne.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.316326.xyz/gtigxjfbqv.html

Ruby: s.match?(/\d+/)
来源：http://hz.yonumen.top/gtlzvmkfru.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ydzc1.top/gtjqhykkfy.html

[I02] 提取所有匹配
来源：http://hz.zhixingplan.top/gtnynpkuhw.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgfzy.top/gtgeotojtb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.redwolf501.top/gtkvapwyqv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinqigfzy.top/gtoxuzkpdr.html

TS:   s.match(/\d+/g)
来源：http://hz.jinyuanbaomall.cn/gtqqfxkefz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cashguo.top/gtbmhluteb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.meibo888.top/gteibyjblu.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhongyouzk.top/gtkuomyqnr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xziqi.cn/gtxdxzssgs.html

[I03] 提取捕获分组
来源：http://hz.yj20258888.top/gtugikmibc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cheryme.top/gtvgbnkqvl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.redwolf501.top/gtwlocvivn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.aizwys.cn/gtbmvqxddp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hfpthk.cn/gtpftfugmi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pengpengdd.cyou/gtguzqxwkh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ivvv.top/gtnvzaogck.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenjidiqi.icu/gtgrunbavl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.c1oappe.top/gtyoenlicw.html

[I04] 正则替换
来源：http://hz.zhongyouzk.top/gtymngnlmn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gzhubu.top/gtgwoqwtbk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.guowangkeji.top/gtwaxylunu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yonumen.top/gtfohilnku.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yueranfly.top/gtzinokynv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.fengsongda.top/gtznxqqdsz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xziqi.cn/gtgcprdwxe.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gzhubu.top/gtamqsysah.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ybcxt.top/gtqgchxxhl.html

[I05] 按正则拆分
来源：http://hz.hnxiangtu.top/gtedwvpdmw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.guowangkeji.top/gtaqfsqyld.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.smart0.xyz/gtgktiplbw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtztueqhxg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtsoapkyhp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.svipenyu.cn/gtvyjhwpre.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sweek.top/gthgvuavsq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yangfankeji.com/gtiixdhsjv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jyoumei.cn/gtgbeybrdk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.havefunace.top/gtsyrdpjdb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.daria6918.cn/gtpytylmcn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ivvv.top/gtbkmsjajo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yonumen.top/gtvacmujtz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xziqi.cn/gtcdrqzsfr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gogol.net.cn/gtopuutmyq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hnqzz.top/gtzsyttvfy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daxiang520.top/gtvudexgiv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hysaishi.cn/gtywrbadkd.html

[I07] 忽略大小写与多行模式
来源：http://hz.gzhubu.top/gtqtfymjvj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ydzc1.top/gtxnowbzly.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shuidangran.top/gtmduirkni.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jqgufenzy.top/gtycjjrhio.html

TS:   /error/gim
来源：http://hz.wangdashe.top/gtrosnayqs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ehwqpu.com/gtfzhfwgrq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yangfankeji.com/gthpkqgbbm.html

Ruby: s.scan(/error/i)
来源：http://hz.chenlongwang.top/gttufabstt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xuanzx.com/gtzlnbkenj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sxryk.cn/gtplxatqyn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xuetiantiany.cn/gtrcbefjek.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cucudq.cn/gtmkymvapy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtekddryjl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenzaomai.com/gtarhdupzl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yueranfly.top/gtfkdxbpdg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shuidangran.top/gtnrsiamba.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gzhubu.top/gtqzwletfo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sxryk.cn/gtcumkpfgc.html

================================================================================
来源：http://hz.c1oappe.top/gttobbeexg.html

J. 日期与时间
来源：http://hz.pengpengdd.cyou/gtfekxxubt.html

================================================================================
来源：http://hz.ivvv.top/gtztehhsnh.html

[J01] 获取当前时间
来源：http://hz.yueranfly.top/gtrluyxgxp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.mhx1999.top/gtezwwxttm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhijiandao.cn/gtyjvfxsql.html

JS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtdhcbswqd.html

TS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtgufnwsxj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.iojbl.cn/gtuxqhrntt.html

Go:   time.Now()
来源：http://hz.sysykeji.top/gthohbdiry.html

Ruby: Time.now
来源：http://hz.cqqwz.cn/gtcjnmfvho.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinqigufen.top/gtjwwnikza.html

[J02] 格式化输出
来源：http://hz.yuxming.cn/gtjhhhjays.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.c1oappe.top/gtiuhfplds.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.snrcjt.cn/gtrxfruksn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258888.top/gttyyjkuqw.html

TS:   d.toISOString()
来源：http://hz.shanyushiyangkeji.top/gtlyxwebwv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.tian-w.cn/gttijaboof.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ehwqpu.com/gtqwptlrwp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigufen.top/gtgnojrlyj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.dashuyun.cn/gtqzoilwbs.html

[J03] 字符串解析为日期
来源：http://hz.jiagoushi.top/gtrdtahkqm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zycfv.cn/gtjyyzqzwl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jyoumei.cn/gtckvubkzf.html

JS:   new Date("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtcfoqxuog.html

TS:   new Date("2024-01-02")
来源：http://hz.zycfv.cn/gtpkpdkpgz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jianghu66.top/gtwydkylog.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sysykeji.top/gtcysuadvd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.9152youxi.cn/gteujanfbc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.snrcjt.cn/gteshemhrc.html

[J04] 时间戳与日期互转
来源：http://hz.hysaishi.cn/gtwizwqcup.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hammf.cn/gtprryixto.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xuanzx.com/gtyhdunrub.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xziqi.cn/gtqrqvmtod.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.aibaodan.cn/gtkpwdlzyz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.chenzaomai.com/gtldauelnb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhaomingkeji.xyz/gtaxxebcsb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.feifeiyinyue.top/gthzrvgpro.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jlsjyb.cn/gtjawwwwhs.html

[J05] 时间加减（加 7 天）
来源：http://hz.vqdsnc.cn/gtrnfntszf.html

Py:   now + timedelta(days=7)
来源：http://hz.jlsjyb.cn/gtokgwqjgi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinyuanbaomall.cn/gticwbuuty.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xinyue.icu/gtswaavgqz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.vqdsnc.cn/gtrtguszpw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xuetiantiany.cn/gtgsqoawft.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhixingplan.top/gtzwxgtngl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.iojbl.cn/gtkcokksnx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.svipenyu.cn/gtsiqizrzs.html

[J06] 计算两时间之差
来源：http://hz.0kj1m.cn/gtizssbzuo.html

Py:   (end - start).total_seconds()
来源：http://hz.tianlin.xyz/gtimxzuxqe.html

PHP:  $end->diff($start)->days;
来源：http://hz.ydjk.org.cn/gtrkhxwboh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.chenzaomai.com/gtdmtyujqo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pengpengdd.cyou/gtsxcjgytq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sysykeji.top/gtnyxqpkgf.html

Go:   end.Sub(start).Hours()
来源：http://hz.redwolf501.top/gtqxtahyiu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.fengsongda.top/gtjyrxufql.html

C#:   (end - start).TotalSeconds
来源：http://hz.guannengcc.top/gtvesdlwkg.html

[J07] 比较两个日期
来源：http://hz.hysaishi.cn/gtshlotyxq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtdkvcvmkx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sxryk.cn/gtxqgqihke.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ivvv.top/gtjvdpkhlg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.iojbl.cn/gtvciqdvex.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cqqwz.cn/gtxgqkqmyt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.9152youxi.cn/gtrnjvcjlg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtteqsvxwh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.feifeiyinyue.top/gtqnedfzxf.html

[J08] 提取年月日与星期
来源：http://hz.fengsongda.top/gtdmqzyvuy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yonumen.top/gtehmiitet.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gzhubu.top/gtkshaveyd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sufxvd.cn/gtytexudux.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgfzy.top/gtysxmmcsg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.nwbrower.top/gtijfiyncp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.smart0.xyz/gtvlveiyja.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shanyushiyangkeji.top/gtaaukntrc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guowangkeji.top/gtbqygakmw.html

[J09] 时区处理
来源：http://hz.zhoulong.xyz/gtsoakcnss.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj20258.top/gtdlqjcbdm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.havefunace.top/gtyzuxjdqt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xziqi.cn/gtgicenmsn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guannengcc.top/gtxbbwqdnm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yonumen.top/gtzihslftr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.fzhhl.top/gtqawbmnup.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shzxlz.cn/gtzhvrqddj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.snrcjt.cn/gtmlzflxal.html

[J10] 取今天 / 本月第一天
来源：http://hz.quarkkingdee.top/gthiurwgit.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.meibo888.top/gtmgbmzdcw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuanzx.com/gtdptwvxqu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tianlin.xyz/gtcfrriwum.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yangfankeji.com/gtkfjokuph.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shuidangran.top/gtvfgjfadu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.redwolf501.top/gtgxtnkdda.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yongpay.top/gtlrygaifu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.0kj1m.cn/gtgqmryewq.html

================================================================================
来源：http://hz.9152youxi.cn/gtxpibxfuj.html

K. JSON 与序列化
来源：http://hz.xuetiantiany.cn/gtdgbmxeke.html

================================================================================
来源：http://hz.cashguo.top/gtwlqwkyla.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinyuanbaomall.cn/gttwpyrexx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jianghu66.top/gtcqvhcwah.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.smart0.xyz/gtfbbltmvq.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangtech.top/gtmvkptlci.html

TS:   JSON.stringify(obj)
来源：http://hz.pengpengdd.cyou/gtebdwbpos.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.52xcode.cn/gtgviwfyhl.html

Go:   json.Marshal(obj)
来源：http://hz.yangfankeji.com/gtcuovmosg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xziqi.cn/gtpqsdmjbt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nwbrower.top/gtiiniebmp.html

[K02] JSON 字符串转对象
来源：http://hz.yj202588.top/gtbhvtvioi.html

Py:   json.loads(s)
来源：http://hz.pycfn.com/gttjarmeud.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yangfankeji.com/gtigtltxhn.html

JS:   JSON.parse(s)
来源：http://hz.quarkkingdee.top/gtolkvwmuk.html

TS:   JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtetzqjfrs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zdqjudy.top/gtnmjcexac.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.kuanghao11.cn/gtbibfloku.html

Ruby: JSON.parse(s)
来源：http://hz.guowangkeji.top/gtywmsradj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jqgfzy.top/gtztrzywef.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.dashuyun.cn/gthgpvutug.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.daria6918.cn/gtsocvljqf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cqqwz.cn/gtdzauynoo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gtoxasuskk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.iojbl.cn/gtbzyfsbol.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jqgfzy.top/gtsooiohtj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tian-w.cn/gtpuszwfkr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yongpay.top/gtzgjsvayq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhijiandao.cn/gtfzuhezjc.html

[K04] 读取 JSON 文件
来源：http://hz.yuxming.cn/gtetfhdpow.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shanyushiyangtech.top/gtpkgulyyh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.haohaochexian.top/gtfzspsoqd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daxiang520.top/gtjbncbulf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.haohaochexian.top/gtnupfuyhy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenlongwang.top/gtjckdvgjt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jyoumei.cn/gtxtkmmsbl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hywenlv.cn/gtmczqvcwl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ydzc1.top/gtdwyhnovn.html

[K05] 深拷贝对象
来源：http://hz.hfpthk.cn/gtcpchylxy.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenjidiqi.icu/gtehzgfzjc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhaomingkeji.xyz/gtkwoifefj.html

JS:   structuredClone(obj)
来源：http://hz.chenlongwang.top/gtslyuqjzj.html

TS:   structuredClone(obj)
来源：http://hz.jqgufenzy.top/gtrbriveyq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xinyue.icu/gtiinezofq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ywan-chungtsiang.top/gtkgapxmpp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydzc1.top/gtvlptlasi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.fzhhl.top/gtunoakaqi.html

[K06] 解析 URL 查询串
来源：http://hz.chenlongwang.top/gthlpxfmlw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuxming.cn/gttmfbhesq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zdqjudy.top/gtmbabdxhx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinyuanbaomall.cn/gtiacdqlzz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuanzhike.top/gtaguuooaj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tian-w.cn/gtqgnaemuy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jianghu66.top/gtobobmkzw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hammf.cn/gtjjrdfecn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtyqcplksc.html

[K07] 进制转换
来源：http://hz.pengpengdd.cyou/gtdxlcdqee.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtucsxkzci.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.meibo888.top/gthlzhcnbq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtttfpvlfb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtmrzbrchp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.316326.xyz/gtpljoxvge.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yanxiufei.cn/gtwhetnmqr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhijiandao.cn/gtcdscpraq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ehwqpu.com/gtnidudnbi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhixingplan.top/gtozsafxsc.html

Py:   pickle.dumps(obj)
来源：http://hz.sxryk.cn/gtkuxtkvdx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.feifeiyinyue.top/gtuntxwkfm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gtplsaviqx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258.top/gtipbpibod.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhiwuduotai.top/gtqkwanpfu.html

Go:   encoding/gob
来源：http://hz.pengpengdd.cyou/gtxoippyhu.html

Ruby: Marshal.dump(obj)
来源：http://hz.cdnleiting.top/gtoonxlfeg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuanzx.com/gtzbwlbdiy.html

================================================================================
来源：http://hz.hywenlv.cn/gthirmfxaq.html

L. 网络请求
来源：http://hz.cucudq.cn/gtcxqvikmu.html

================================================================================
来源：http://hz.bjfxy.top/gtplyseasr.html

[L01] 发送 GET 请求
来源：http://hz.tianlin.xyz/gtmlwwsrpy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daria6918.cn/gtcphknool.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenlongwang.top/gtonrsujlq.html

JS:   await fetch(url)
来源：http://hz.meibo888.top/gtfrxmrxoo.html

TS:   await fetch(url)
来源：http://hz.ppjwa.cn/gtkmhgohye.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.fzhhl.top/gttsukywgr.html

Go:   resp, err := http.Get(url)
来源：http://hz.hnqzz.top/gtoewipxuh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nanxinkj.top/gtgeculupe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.svipenyu.cn/gtemrxtbeb.html

[L02] 发送 POST JSON
来源：http://hz.hongshengwenyu.top/gtdgbgpxha.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guannengcc.top/gtbsnagkuw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xylfe.cn/gtjudbpmag.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gtuwrpjlvb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnqzz.top/gtswfulpav.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinqigfzy.top/gtbyvgccqa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.quarkkingdee.top/gtqeuytkxb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yangfankeji.com/gtubbngqet.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.pengpengdd.cyou/gteejvffno.html

[L03] 设置自定义请求头
来源：http://hz.feifeiyinyue.top/gtmwerzvyb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.fengsongda.top/gtmxdmygyq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.0kj1m.cn/gtysaziaty.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sweek.top/gtkfyqngvi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xingfuxueyuan.xyz/gtjjpkzjfc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.0kj1m.cn/gtckfawwlp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.havefunace.top/gtuuqwhenb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gotoacloud.top/gtxqzkudwv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cashguo.top/gtajcggsut.html

[L04] 设置超时
来源：http://hz.quarkkingdee.top/gtjzaabuwd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.feifeiyinyue.top/gtvyuykrdk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.0kj1m.cn/gthwlbgbfo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtlfdxshgg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gtthovzyqq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.pengpengdd.cyou/gtqtywidqv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.aizwys.cn/gttdymffsb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ehwqpu.com/gthcxsmxus.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj20258888.top/gtisylnkuy.html

[L05] 上传文件（multipart）
来源：http://hz.hfpthk.cn/gtyiiyjmkc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhoulong.xyz/gtayeylnpg.html


<!-- 参考信息 -->