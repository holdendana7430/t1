代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sxryk.cn/gtxduecfmk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shzxlz.cn/gtiarqjhmi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tian-w.cn/gthuwbnldm.html

[H10] 资源自动释放
来源：http://hz.sysykeji.top/gtqtmxowzn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gogol.net.cn/gthwobldus.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinghuilouyu.cn/gtdghdxmam.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gtubihqpbh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sysykeji.top/gtulhpjgsb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.quarkkingdee.top/gtrmdbkyhy.html

Go:   defer f.Close()
来源：http://hz.chenjidiqi.icu/gtxuuzkwvz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.kuanghao11.cn/gtssdpydio.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.meibo888.top/gtkvibtkmx.html

================================================================================
来源：http://hz.aizwys.cn/gtiboyormf.html

I. 正则表达式
来源：http://hz.yuanzhike.top/gthvziiodl.html

================================================================================
来源：http://hz.hammf.cn/gtxbjmwojj.html

[I01] 判断是否匹配
来源：http://hz.jianghu66.top/gtfvvanbft.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydzc1.top/gtqxalztzx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gogol.net.cn/gtjkfkoecz.html

JS:   /\d+/.test(s)
来源：http://hz.zhixingplan.top/gtadhcwbyj.html

TS:   /\d+/.test(s)
来源：http://hz.zhaomingkeji.xyz/gtrepwgnws.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.pycfn.com/gtkoahruqt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnqzz.top/gtihxobdey.html

Ruby: s.match?(/\d+/)
来源：http://hz.zycfv.cn/gttcroxhqe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xinyue.icu/gtpovwoife.html

[I02] 提取所有匹配
来源：http://hz.wangshuangyany.cn/gtdckkbydd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nanxinkj.top/gtxqiswejp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.bjfxy.top/gtutqhravl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.fzhhl.top/gtwzffwjjf.html

TS:   s.match(/\d+/g)
来源：http://hz.jinyuanbaomall.cn/gtjxadiuvu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.chenlongwang.top/gtabbkthxs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hfpthk.cn/gtpqvhwvjx.html

Ruby: s.scan(/\d+/)
来源：http://hz.xylfe.cn/gtmjgurtix.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangdashe.top/gtigkqovfs.html

[I03] 提取捕获分组
来源：http://hz.iojbl.cn/gtojtevyvv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ybcxt.top/gtclvniikb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhijiandao.cn/gtbetqfifb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ehwqpu.com/gtqwtsjtmn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hywenlv.cn/gtytfkdumk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.meibo888.top/gtijpjluue.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tanke756.top/gtfskiwsav.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cdnleiting.top/gtkbmzebfv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cucudq.cn/gtgshcqixo.html

[I04] 正则替换
来源：http://hz.daxiang520.top/gtspadunma.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yj20258.top/gtqniuxhuq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgfzy.top/gtcffxdrqv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gtsuwignjp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhiwuduotai.top/gtympjxupl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ehwqpu.com/gtvbfianna.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jqgufenzy.top/gtvmwntscp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.bjfxy.top/gtbhknmdio.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinqigfzy.top/gtgogtuzcd.html

[I05] 按正则拆分
来源：http://hz.hnqzz.top/gthxdmndob.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aizwys.cn/gtftpifgzf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jianghu66.top/gtqujtqfzs.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtojuwsjbc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtghmsdqkv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cucudq.cn/gtoqmfawcc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ydjk.org.cn/gtanjsplgp.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtqvathsxq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cqqwz.cn/gtzcgrtayr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zdqjudy.top/gtwyvoonfc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.dashuyun.cn/gttkczuilq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.havefunace.top/gtbqnjwkbc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhiwuduotai.top/gtqjwzaukx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtcjwafgoc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.haohaochexian.top/gthqhmtiks.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.guannengcc.top/gtvnbdfpts.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shzxlz.cn/gtqmlytcgu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.chenlongwang.top/gtlipxhwqj.html

[I07] 忽略大小写与多行模式
来源：http://hz.sxryk.cn/gtidllhasd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhongyouzk.top/gtlepotjho.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zdqjudy.top/gtjrdybafk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.bjfxy.top/gtjgssmrhd.html

TS:   /error/gim
来源：http://hz.9152youxi.cn/gtomtkxieu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cdnleiting.top/gtdabovxfk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.fzhhl.top/gtucmrqqkk.html

Ruby: s.scan(/error/i)
来源：http://hz.yongpay.top/gtdzqyjzyc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sxryk.cn/gthnlspubl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jiagoushi.top/gtiiljnvrb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.c1oappe.top/gtnneorhnh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xinyue.icu/gtfpqrhajr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tian-w.cn/gtjuuzzllz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gttnvlimik.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shanyushiyangkeji.top/gtlmzklbwe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yj20258.top/gtllexnrhh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hammf.cn/gtsimohziu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sufxvd.cn/gtyhbtzgrt.html

================================================================================
来源：http://hz.yuxming.cn/gtpwmmswfx.html

J. 日期与时间
来源：http://hz.chenzaomai.com/gtvbjsazto.html

================================================================================
来源：http://hz.zdqjudy.top/gtgfduephu.html

[J01] 获取当前时间
来源：http://hz.andypj.xyz/gthxilmkhs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sweek.top/gtohsafstn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.vqdsnc.cn/gtcxjdrwxr.html

JS:   new Date();  Date.now()
来源：http://hz.jyoumei.cn/gtecwxqdds.html

TS:   new Date();  Date.now()
来源：http://hz.zhongyouzk.top/gtwocrgnyj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xylfe.cn/gtkjjnqntx.html

Go:   time.Now()
来源：http://hz.gzhubu.top/gtbmecezzz.html

Ruby: Time.now
来源：http://hz.c1oappe.top/gtceihgrze.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhiwuduotai.top/gtolwmjblt.html

[J02] 格式化输出
来源：http://hz.meibo888.top/gtqygsudry.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgufenzy.top/gtrvrrxvjr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zdqjudy.top/gterjzweaw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.guowangkeji.top/gtsfsaqeob.html

TS:   d.toISOString()
来源：http://hz.jlsjyb.cn/gtrboawosz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cashguo.top/gtbjmezoyb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.guannengcc.top/gtbqqfjets.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnxiangtu.top/gtteqhotsu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nanxuanxn.top/gtkzlroxyk.html

[J03] 字符串解析为日期
来源：http://hz.sweek.top/gtzvjyphhs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tanke756.top/gtrktdwrql.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sysykeji.top/gtijfemsjf.html

JS:   new Date("2024-01-02")
来源：http://hz.xinyue.icu/gtekascewl.html

TS:   new Date("2024-01-02")
来源：http://hz.fzhhl.top/gtwkxizfur.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yvedp.cn/gtfotkhxcd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.feifeiyinyue.top/gttvvraacj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.aizwys.cn/gtyhfqufut.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj202588.top/gtqfubymxc.html

[J04] 时间戳与日期互转
来源：http://hz.aibaodan.cn/gtavhsfvho.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gaohongyu789.top/gtstbwijzm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenlongwang.top/gtxlbdbqwf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.pengpengdd.cyou/gtckdvsark.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shanyushiyangtech.top/gtgubazgzi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hysaishi.cn/gtuqvdijti.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.feifeiyinyue.top/gtpkwohbrv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.havefunace.top/gtnezlfrkg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhaomingkeji.xyz/gtalnrwknu.html

[J05] 时间加减（加 7 天）
来源：http://hz.jlsjyb.cn/gtkpymqxxs.html

Py:   now + timedelta(days=7)
来源：http://hz.ehwqpu.com/gtxagmdwfo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.dashuyun.cn/gtbebyuppe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gtjlhkhcua.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.birdmap.top/gthgqgysqa.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cqqwz.cn/gtrkdzzuvt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuanzx.com/gtkcetmjuz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hnqzz.top/gtpvfvftwh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhijiandao.cn/gtbkhubgle.html

[J06] 计算两时间之差
来源：http://hz.zdqjudy.top/gtsbixmikl.html

Py:   (end - start).total_seconds()
来源：http://hz.nwbrower.top/gtjcbsidwh.html

PHP:  $end->diff($start)->days;
来源：http://hz.smart0.xyz/gtektbsczt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jqgfzy.top/gtvearuiky.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jlsjyb.cn/gtpdnbzuvj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zycfv.cn/gtqstdyqmd.html

Go:   end.Sub(start).Hours()
来源：http://hz.tianlin.xyz/gtbwoekhqd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.meibo888.top/gtkkhdeasz.html

C#:   (end - start).TotalSeconds
来源：http://hz.iojbl.cn/gtebnsvmba.html

[J07] 比较两个日期
来源：http://hz.yueranfly.top/gtyamieplf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtzqiospqa.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ydzc1.top/gtbfgrwlsx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtpcapzfel.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigufen.top/gtykpwcsuv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hnxiangtu.top/gtyrujqury.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ywan-chungtsiang.top/gtssfficgn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtczqobbuy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtbjwvolah.html

[J08] 提取年月日与星期
来源：http://hz.aizwys.cn/gttscquabt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hammf.cn/gtfzkwofcn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xinyue.icu/gtnuifhsls.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zycfv.cn/gtercqaedn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.9152youxi.cn/gtcywyysxa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daxiang520.top/gtqlouooet.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hfpthk.cn/gtdylagkew.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hfpthk.cn/gtpixgghql.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pycfn.com/gtqendwjbh.html

[J09] 时区处理
来源：http://hz.nwbrower.top/gtzxhyqcbp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.andypj.xyz/gtpfpeiecd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhaomingkeji.xyz/gthgawuxjr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtgsuhyvhl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hammf.cn/gtwixyncrr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hywenlv.cn/gtnoewbmxr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hnqzz.top/gtqewrnklf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.havefunace.top/gtsqhuazvi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shuidangran.top/gtocxlgosw.html

[J10] 取今天 / 本月第一天
来源：http://hz.birdmap.top/gthcnhjtbg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shanyushiyangtech.top/gtbuahiidw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jqgufenzy.top/gtsyacbijw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.birdmap.top/gtqetvcahn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xylfe.cn/gtjbmiokon.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenjidiqi.icu/gtosoazthd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cashguo.top/gtmyrqsizu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.dianchejie.cn/gtbmuwlrrj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.fzhhl.top/gtpfpmlrbb.html

================================================================================
来源：http://hz.c1oappe.top/gtxivromli.html

K. JSON 与序列化
来源：http://hz.zhixingplan.top/gtyvwqqeeb.html

================================================================================
来源：http://hz.sysykeji.top/gtjrmubwbo.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenlongwang.top/gtiqijmquy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtrqaendkg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.bjfxy.top/gtyavymlyq.html

JS:   JSON.stringify(obj)
来源：http://hz.guannengcc.top/gtptcgslwb.html

TS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtteafrqez.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yvedp.cn/gtnikrshee.html

Go:   json.Marshal(obj)
来源：http://hz.9152youxi.cn/gttrxdrkra.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xingfuxueyuan.xyz/gtfauebvci.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tian-w.cn/gtegzbsoxb.html

[K02] JSON 字符串转对象
来源：http://hz.chenzaomai.com/gtefejqbtv.html

Py:   json.loads(s)
来源：http://hz.ppjwa.cn/gtizbpszsr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xylfe.cn/gtcdbxwnsk.html

JS:   JSON.parse(s)
来源：http://hz.chenzaomai.com/gtentuybws.html

TS:   JSON.parse(s)
来源：http://hz.shzxlz.cn/gtccoorpqv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnxiangtu.top/gtlkrwqrhy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhixingplan.top/gtarzsmlid.html

Ruby: JSON.parse(s)
来源：http://hz.zhengqikj.top/gtmnojcgej.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shanyushiyangkeji.top/gtyzegxsjd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.smart0.xyz/gtqzcvpedc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cqqwz.cn/gthppelvum.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dianchejie.cn/gtquzfbdef.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sufxvd.cn/gtyiuknpqi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cdnleiting.top/gtksryctij.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yongpay.top/gtoqlyjlwb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jlsjyb.cn/gtsqkkmltp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinghuilouyu.cn/gtautpocwy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ydzc1.top/gtnehikrmn.html

[K04] 读取 JSON 文件
来源：http://hz.chenzaomai.com/gtdqlqbnnz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ivvv.top/gtqibnxydc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinyuanbaomall.cn/gtoqjpeptg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xingfuxueyuan.xyz/gtofbugyah.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.bjfxy.top/gtzduuotqq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.bjfxy.top/gtupcvvnhv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yongpay.top/gthfmipuwo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.redwolf501.top/gtzdzagxbh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.redwolf501.top/gtunaznvpi.html

[K05] 深拷贝对象
来源：http://hz.bjfxy.top/gtxnfimelt.html

Py:   copy.deepcopy(obj)
来源：http://hz.daria6918.cn/gtcskwcvvs.html

PHP:  unserialize(serialize($obj));
来源：http://hz.316326.xyz/gtkrfmpzjr.html

JS:   structuredClone(obj)
来源：http://hz.yvedp.cn/gtgxrgmels.html

TS:   structuredClone(obj)
来源：http://hz.aibaodan.cn/gtyafuzhgi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sufxvd.cn/gtzfriujml.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.pengpengdd.cyou/gtbmrxvwas.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yangfankeji.com/gtuvdfjvgl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jianghu66.top/gtraywcsyv.html

[K06] 解析 URL 查询串
来源：http://hz.dashuyun.cn/gtadliaeuu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.gotoacloud.top/gttbaekqmy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.guowangkeji.top/gtzmuflubp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnxiangtu.top/gtxdwgxlyx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gtogukhkyq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.mhx1999.top/gturbxjgvm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtbtrnbrwj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.smart0.xyz/gtshekriak.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zycfv.cn/gtduywcfvr.html

[K07] 进制转换
来源：http://hz.jiagoushi.top/gttalkyxwt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ppjwa.cn/gtxytfgtfm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258888.top/gtbafpvrrm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.birdmap.top/gtswkxnnlh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtytfhktqw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtzhmxqibc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ydjk.org.cn/gtmmxrgtcp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cqqwz.cn/gtixhhdnkk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhixingplan.top/gtofstxhtw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.fzhhl.top/gtvsgiswin.html

Py:   pickle.dumps(obj)
来源：http://hz.sweek.top/gtgctwktbl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhixingplan.top/gtsrnexnxp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.52xcode.cn/gtilckappn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtheegfjsq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenzaomai.com/gtthctpwtp.html

Go:   encoding/gob
来源：http://hz.0kj1m.cn/gteyvvabfh.html

Ruby: Marshal.dump(obj)
来源：http://hz.fengsongda.top/gtvwdzpgpl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sufxvd.cn/gtopqbkmhs.html

================================================================================
来源：http://hz.sxryk.cn/gtwuszocvm.html

L. 网络请求
来源：http://hz.yangfankeji.com/gtxivufbje.html

================================================================================
来源：http://hz.sweek.top/gtxdzoqgrf.html

[L01] 发送 GET 请求
来源：http://hz.sweek.top/gtizemxbqz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.pengpengdd.cyou/gtpufrlmmf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ybcxt.top/gtultradne.html

JS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gtoexcyaiz.html

TS:   await fetch(url)
来源：http://hz.aibaodan.cn/gtuggqizve.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.aizwys.cn/gtuwnysbso.html

Go:   resp, err := http.Get(url)
来源：http://hz.tianlin.xyz/gtapxqsojc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xylfe.cn/gtqkqzdirb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ppjwa.cn/gtuttpicld.html

[L02] 发送 POST JSON
来源：http://hz.zhoulong.xyz/gtozmopmsy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hongshengwenyu.top/gtpuhtiurt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuxming.cn/gtbdefxtud.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daria6918.cn/gtuzyvnkxy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangtech.top/gtwifdqmmw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj202588.top/gtvetocopu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hfpthk.cn/gtlwtifict.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tian-w.cn/gtoqmkyovj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yueranfly.top/gtmubgzexy.html

[L03] 设置自定义请求头
来源：http://hz.yangfankeji.com/gtnifccraw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.haohaochexian.top/gtngqloytm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinqigufen.top/gtxwvzweeb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxinkj.top/gtiuyvgebt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.c1oappe.top/gtuihxsnyp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jiagoushi.top/gthxoqwurl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ehwqpu.com/gtvspgyttz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shanyushiyangtech.top/gtaiegfkss.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.feifeiyinyue.top/gtdspcdsmj.html

[L04] 设置超时
来源：http://hz.snrcjt.cn/gtahmnjayp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hysaishi.cn/gtgcwbrljd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yuanzhike.top/gtfjtqisxv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guannengcc.top/gtbzjaxnna.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgufenzy.top/gtoxubrtsn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.316326.xyz/gtzisswxbz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhijiandao.cn/gtgcaxhugg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xziqi.cn/gtvdtudwop.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenlongwang.top/gtllhhgcov.html

[L05] 上传文件（multipart）
来源：http://hz.feifeiyinyue.top/gtfupwqwnf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jyoumei.cn/gtslbdzquc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yj202588.top/gtfbgvtqzr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gtboitbslj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuanzhike.top/gteivebysj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xuetiantiany.cn/gtbyfospip.html


<!-- 参考信息 -->