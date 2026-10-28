代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.havefunace.top/gtocheramc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shuidangran.top/gtsbqixejm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jianghu66.top/gtgpvbyjnm.html

[H10] 资源自动释放
来源：http://hz.cqqwz.cn/gtshszylxa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shuidangran.top/gtxjaxwdjg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jqgfzy.top/gtglwzzjxx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.smart0.xyz/gtydnngozm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuetiantiany.cn/gtdjcbojjg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhijiandao.cn/gtziwishti.html

Go:   defer f.Close()
来源：http://hz.xziqi.cn/gtauksdshi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.fzhhl.top/gtqaxgwvho.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.dashuyun.cn/gtgznxzvrb.html

================================================================================
来源：http://hz.svipenyu.cn/gtqebstzic.html

I. 正则表达式
来源：http://hz.zhoulong.xyz/gtofhzfnub.html

================================================================================
来源：http://hz.jyoumei.cn/gthdqhlpen.html

[I01] 判断是否匹配
来源：http://hz.shanyushiyangtech.top/gtjlpouamu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hongshengwenyu.top/gtisfmuiiu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jyoumei.cn/gtfbkpqgxi.html

JS:   /\d+/.test(s)
来源：http://hz.xylfe.cn/gtdiztsbxl.html

TS:   /\d+/.test(s)
来源：http://hz.jqgfzy.top/gtugbivjzn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jlsjyb.cn/gthevgbtzs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yongpay.top/gtnbsjngvk.html

Ruby: s.match?(/\d+/)
来源：http://hz.gogol.net.cn/gtjpnmnyzk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.feifeiyinyue.top/gtznmggydf.html

[I02] 提取所有匹配
来源：http://hz.redwolf501.top/gtlncjyhqn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhixingplan.top/gtdljxxide.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.guowangkeji.top/gtykfiazpb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gzhubu.top/gtspzjelxm.html

TS:   s.match(/\d+/g)
来源：http://hz.gotoacloud.top/gtgpefxdcg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jlsjyb.cn/gtqftajgrv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hammf.cn/gtniekqpbx.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnqzz.top/gtmjifrtjx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenjidiqi.icu/gtopzdidik.html

[I03] 提取捕获分组
来源：http://hz.tianlin.xyz/gtprafszmp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.smart0.xyz/gtvildnwhy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.316326.xyz/gtmjdizgyg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.bjfxy.top/gtfpcxynws.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.dashuyun.cn/gttymidjjv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.aibaodan.cn/gtgiaiqmtt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hnxiangtu.top/gtmfddathu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yuxming.cn/gtnhwyrsul.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cashguo.top/gtlpqfxpss.html

[I04] 正则替换
来源：http://hz.yonumen.top/gtsxdecrdq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dianchejie.cn/gtoqusrrjm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xziqi.cn/gtveimkxvi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.mhx1999.top/gttwimroqw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.52xcode.cn/gtrvbhfkls.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.316326.xyz/gtqhuenqde.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.fzhhl.top/gtydhwajez.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shuidangran.top/gtsfnnbyqm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cucudq.cn/gtviwazpjt.html

[I05] 按正则拆分
来源：http://hz.chenlongwang.top/gtnaenylvi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cdnleiting.top/gtvjgibkki.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cqqwz.cn/gtrtdozomb.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gtdnxgbdmm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtpqxbbayp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhaomingkeji.xyz/gtrzyoitfz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.haohaochexian.top/gtuoxgoqju.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtingbpscj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.quarkkingdee.top/gttelmyjra.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jiagoushi.top/gtlzfofbdc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jlsjyb.cn/gtadnnqgqv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sufxvd.cn/gtwsxbnuuz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gtsyjxovqt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ppjwa.cn/gtwaeisckz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cqqwz.cn/gtlhtcenhn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.vqdsnc.cn/gtyhereuni.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenlongwang.top/gtfnyyyznj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj20258.top/gtezppgspm.html

[I07] 忽略大小写与多行模式
来源：http://hz.kuanghao11.cn/gtasebtyte.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinqigfzy.top/gtlklhpzci.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.daxiang520.top/gtdbfcppst.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ywan-chungtsiang.top/gtkrvkxkbg.html

TS:   /error/gim
来源：http://hz.yonumen.top/gtjizxdjhr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhixingplan.top/gtbgipnnpf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.kuanghao11.cn/gthajplrcz.html

Ruby: s.scan(/error/i)
来源：http://hz.ivvv.top/gtmifdqaqq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenjidiqi.icu/gtorkzcaol.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gotoacloud.top/gtnyrdwyjo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.pycfn.com/gtzuzfyklu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ydjk.org.cn/gtdyfjrhgc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dashuyun.cn/gtggpytgjx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daxiang520.top/gtrenrdxct.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hnqzz.top/gtwibizcka.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.0kj1m.cn/gtehnhpbvc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.smart0.xyz/gtokkwoprd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xinyue.icu/gtktabyugs.html

================================================================================
来源：http://hz.meibo888.top/gtjxfxtmzs.html

J. 日期与时间
来源：http://hz.ivvv.top/gtynxrajkq.html

================================================================================
来源：http://hz.redwolf501.top/gtgzeaytli.html

[J01] 获取当前时间
来源：http://hz.hongshengwenyu.top/gtdhqvfroz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hysaishi.cn/gtttrkufmg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhoulong.xyz/gthofvnkih.html

JS:   new Date();  Date.now()
来源：http://hz.gogol.net.cn/gtfvmcpama.html

TS:   new Date();  Date.now()
来源：http://hz.tian-w.cn/gttbjnchya.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.guannengcc.top/gtiaengfcj.html

Go:   time.Now()
来源：http://hz.ehwqpu.com/gtaflochtk.html

Ruby: Time.now
来源：http://hz.jinyuanbaomall.cn/gtuotsqrjo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenzaomai.com/gtfstgcyar.html

[J02] 格式化输出
来源：http://hz.yj20258.top/gtsbzngnie.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jianghu66.top/gtgxiogtop.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ppjwa.cn/gtblgxbjfu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zycfv.cn/gtxubsqwma.html

TS:   d.toISOString()
来源：http://hz.chenjidiqi.icu/gtaywwmgyz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.bjfxy.top/gtizmkpdkb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xingfuxueyuan.xyz/gtsqibowyy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yongpay.top/gtwyvtflnb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.snrcjt.cn/gtmvcvicpt.html

[J03] 字符串解析为日期
来源：http://hz.nanxuanxn.top/gtzazmwape.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.kuanghao11.cn/gteuuitxof.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.svipenyu.cn/gtljcuaxzq.html

JS:   new Date("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtxcanemfi.html

TS:   new Date("2024-01-02")
来源：http://hz.sysykeji.top/gtkevvahmw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nanxinkj.top/gtjwznuqzw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtmvjvjwjr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hammf.cn/gtuqywqbni.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj202588.top/gtsfflmqql.html

[J04] 时间戳与日期互转
来源：http://hz.gzhubu.top/gtjlztfwnt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.vqdsnc.cn/gttyruappj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.vqdsnc.cn/gtzhulvgcm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cdnleiting.top/gtmthpqsxz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cheryme.top/gtkmiuebmw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yongpay.top/gtbgesawia.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhiwuduotai.top/gtejhnbhag.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zdqjudy.top/gttrtwlxgy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hnxiangtu.top/gtsurbufko.html

[J05] 时间加减（加 7 天）
来源：http://hz.fengsongda.top/gtwlzegmrn.html

Py:   now + timedelta(days=7)
来源：http://hz.daria6918.cn/gtxqezjnpl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yanxiufei.cn/gtylcphgys.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtqjzomxaf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.mhx1999.top/gtcslucjzy.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.kuanghao11.cn/gtspxxselj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.havefunace.top/gttasqoorv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xuanzx.com/gtcpcscoin.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.daxiang520.top/gtftemctjp.html

[J06] 计算两时间之差
来源：http://hz.xuetiantiany.cn/gtuzzotuyd.html

Py:   (end - start).total_seconds()
来源：http://hz.quarkkingdee.top/gtfeniqwij.html

PHP:  $end->diff($start)->days;
来源：http://hz.shzxlz.cn/gtqcjxdewi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.dianchejie.cn/gtjurkghoa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.fzhhl.top/gtlpdsrduh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jyoumei.cn/gtnvlhbwwp.html

Go:   end.Sub(start).Hours()
来源：http://hz.52xcode.cn/gtayesvhds.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gogol.net.cn/gtwgpelsei.html

C#:   (end - start).TotalSeconds
来源：http://hz.cdnleiting.top/gtapgkgmyj.html

[J07] 比较两个日期
来源：http://hz.chenzaomai.com/gtxyhdeiuw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtlorzjwvp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dashuyun.cn/gtvatxlxno.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.iojbl.cn/gtzvtjvakr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jyoumei.cn/gtlrozcdpl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sysykeji.top/gtrqvhorpg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ivvv.top/gtoeeviqcu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtupwemxtq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtaufwiith.html

[J08] 提取年月日与星期
来源：http://hz.zhengqikj.top/gthkflzall.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.smart0.xyz/gtedceowqt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.daxiang520.top/gtoaqzxuni.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sysykeji.top/gtjyygfqnk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.fengsongda.top/gtfgfkotcu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.tian-w.cn/gtmepsjaox.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.andypj.xyz/gtkzorbooi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.quarkkingdee.top/gtspidkcub.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shzxlz.cn/gtgagolwqq.html

[J09] 时区处理
来源：http://hz.gogol.net.cn/gtnrtecvld.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.316326.xyz/gtllhxbnop.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhiwuduotai.top/gthicknnuh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangkeji.top/gtyorvhmqn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.andypj.xyz/gtjuxvptul.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.daria6918.cn/gtnkasdmun.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.redwolf501.top/gtcjxzusrp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hnqzz.top/gtlbenebqy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj20258.top/gtymcflmbq.html

[J10] 取今天 / 本月第一天
来源：http://hz.gaohongyu789.top/gtqbqhaptr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhixingplan.top/gtghbptlfi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jlsjyb.cn/gtvvfzxoia.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenjidiqi.icu/gtvtndnspj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenjidiqi.icu/gtepohhvaa.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cheryme.top/gtarappbzh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sweek.top/gthqscuvcd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sysykeji.top/gtpdlgjqck.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gogol.net.cn/gtaknmcfzs.html

================================================================================
来源：http://hz.jinqigfzy.top/gtxlrqdaal.html

K. JSON 与序列化
来源：http://hz.snrcjt.cn/gtihjzsxqp.html

================================================================================
来源：http://hz.bjfxy.top/gtroebcjgo.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhixingplan.top/gtibampwby.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tian-w.cn/gtqljnkzsj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gtxlntldgt.html

JS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gtaegnpzrf.html

TS:   JSON.stringify(obj)
来源：http://hz.xingfuxueyuan.xyz/gtgcanseud.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yuanzhike.top/gtcucadaxn.html

Go:   json.Marshal(obj)
来源：http://hz.jqgfzy.top/gtblbamecu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.smart0.xyz/gtfcpxcjoj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhongyouzk.top/gtdgnylfod.html

[K02] JSON 字符串转对象
来源：http://hz.sweek.top/gtfpzabipf.html

Py:   json.loads(s)
来源：http://hz.sufxvd.cn/gtrblryblf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.wangdashe.top/gtkmsrolyv.html

JS:   JSON.parse(s)
来源：http://hz.tian-w.cn/gtbibbbhvl.html

TS:   JSON.parse(s)
来源：http://hz.bjfxy.top/gtoymgbexi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yongpay.top/gtoubtnywh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sweek.top/gtwxlmogip.html

Ruby: JSON.parse(s)
来源：http://hz.cucudq.cn/gtrxqirima.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sufxvd.cn/gtjxilkvcy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.nwbrower.top/gtbsfojvrp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xylfe.cn/gtpnurmhia.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.daria6918.cn/gttfarugcl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jlsjyb.cn/gtszcjruzw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jyoumei.cn/gturzymlnz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yanxiufei.cn/gtyahpnlhd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.daria6918.cn/gtghecazta.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinqigufen.top/gtddgoglgg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ydzc1.top/gtrmwvmfae.html

[K04] 读取 JSON 文件
来源：http://hz.zhoulong.xyz/gthpgpqtnd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jqgufenzy.top/gtaetwcadr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhongyouzk.top/gtsgiomnsy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.kuanghao11.cn/gtbotxbsno.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.haohaochexian.top/gtnimehqzh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cheryme.top/gtcnymzwju.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.iojbl.cn/gteozmdcjh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yanxiufei.cn/gtosfnpawu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.52xcode.cn/gtpagekpdo.html

[K05] 深拷贝对象
来源：http://hz.aizwys.cn/gteybbmeag.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhixingplan.top/gtitrighzs.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jqgfzy.top/gttnbxklgh.html

JS:   structuredClone(obj)
来源：http://hz.yanxiufei.cn/gthqqhvxbi.html

TS:   structuredClone(obj)
来源：http://hz.dashuyun.cn/gtzqwnvzdu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cheryme.top/gtfbxmakdg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.tanke756.top/gtudwowjcv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.nanxinkj.top/gtuomkcunt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cucudq.cn/gtgnqpuenr.html

[K06] 解析 URL 查询串
来源：http://hz.jyoumei.cn/gtwmzggokr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.pengpengdd.cyou/gtqaqsrnbn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.316326.xyz/gtnvtpcezx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenzaomai.com/gtgpifsmvs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ehwqpu.com/gtzhhzpfhi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hysaishi.cn/gtwpbxehxi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.9152youxi.cn/gtdqatfder.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aibaodan.cn/gtlgpudnly.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.daxiang520.top/gtqolqijkp.html

[K07] 进制转换
来源：http://hz.hywenlv.cn/gtnljgerfv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.aibaodan.cn/gtnqeyvrfp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenlongwang.top/gtedymvqmz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtctxbtomn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yonumen.top/gtkvdloqru.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtbohwbffy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ywan-chungtsiang.top/gtqbkulnee.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cqqwz.cn/gtkvjkjwua.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nwbrower.top/gtowebxlia.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yuanzhike.top/gtizegppuo.html

Py:   pickle.dumps(obj)
来源：http://hz.meibo888.top/gtckenlztf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shangyingyoupin.top/gtgdayhqlu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sysykeji.top/gtdkhuxjfz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gtggppzzje.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.mhx1999.top/gtednuefjs.html

Go:   encoding/gob
来源：http://hz.kuanghao11.cn/gtqvlnsiwd.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgfzy.top/gtriowpldb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj202588.top/gtquystcoh.html

================================================================================
来源：http://hz.316326.xyz/gtqjicodno.html

L. 网络请求
来源：http://hz.c1oappe.top/gtwxjfvfzh.html

================================================================================
来源：http://hz.cucudq.cn/gtjamdclfo.html

[L01] 发送 GET 请求
来源：http://hz.xinyue.icu/gtqecjtupv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.meibo888.top/gtujlmvccj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.c1oappe.top/gtgcxhlead.html

JS:   await fetch(url)
来源：http://hz.chenlongwang.top/gtnttbfgag.html

TS:   await fetch(url)
来源：http://hz.jyoumei.cn/gtulmmhybg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jlsjyb.cn/gtgqckjjqh.html

Go:   resp, err := http.Get(url)
来源：http://hz.hfpthk.cn/gtrynesnsx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.dashuyun.cn/gtxxbteeqh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hongshengwenyu.top/gtnbivjtvk.html

[L02] 发送 POST JSON
来源：http://hz.shuidangran.top/gtmycdtlix.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cdnleiting.top/gtpvtjqrmz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxinkj.top/gtptohpbvh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.9152youxi.cn/gtofkeuihf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shuidangran.top/gtjdpcxved.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shanyushiyangkeji.top/gtcnhidmkl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yvedp.cn/gtwxokwktg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj20258888.top/gtngrbskoe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cdnleiting.top/gtqvkejsev.html

[L03] 设置自定义请求头
来源：http://hz.jyoumei.cn/gtpztbbyjq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hammf.cn/gtjeerfaka.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.fzhhl.top/gtvryxhfxx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.quarkkingdee.top/gtkuvnpkhp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtgpipcdgu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.vqdsnc.cn/gtmrfgotes.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.aizwys.cn/gtksqenaiz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinqigfzy.top/gtljmalkev.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ppjwa.cn/gtahgwgkef.html

[L04] 设置超时
来源：http://hz.vqdsnc.cn/gtwprvqdyc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ybcxt.top/gtdxtmtzcx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jlsjyb.cn/gtcwzyvecj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ywan-chungtsiang.top/gtogedhmlu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenzaomai.com/gtubskdoke.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.snrcjt.cn/gtnormqwjo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yueranfly.top/gtylnaagyu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gaohongyu789.top/gtincwjxwx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jiagoushi.top/gtqagqgqmh.html

[L05] 上传文件（multipart）
来源：http://hz.zhiwuduotai.top/gtpwbxnuzf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tian-w.cn/gthyynzajz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jqgufenzy.top/gtrphnnzoc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hammf.cn/gtuzezkqtk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yonumen.top/gtbhkiatiq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shuidangran.top/gtmvouxywk.html


<!-- 参考信息 -->