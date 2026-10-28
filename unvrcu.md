代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.meibo888.top/gttuexuxgy.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xinyue.icu/gtadanekoj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zdqjudy.top/gtiftwgnrp.html

[H10] 资源自动释放
来源：http://hz.jqgfzy.top/gtbihdpfmz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xuanzx.com/gtsrexvkiy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xylfe.cn/gtztwcyqxk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.andypj.xyz/gtaexkckrk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtdygwzyyj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gzhubu.top/gtcbmaahvi.html

Go:   defer f.Close()
来源：http://hz.jqgfzy.top/gtsabjrnjc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.pycfn.com/gttltpowgi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.redwolf501.top/gtvwmsluya.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gttmuihmte.html

I. 正则表达式
来源：http://hz.cucudq.cn/gtbardsihy.html

================================================================================
来源：http://hz.pycfn.com/gtlrrxgbhz.html

[I01] 判断是否匹配
来源：http://hz.xuanzx.com/gtklfrmmbw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhongyouzk.top/gtribpprbw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ivvv.top/gtnxmtusnt.html

JS:   /\d+/.test(s)
来源：http://hz.jinyuanbaomall.cn/gtxowhfapc.html

TS:   /\d+/.test(s)
来源：http://hz.jqgufenzy.top/gtxdzreyig.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hongshengwenyu.top/gtfkckmdpo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.dashuyun.cn/gtzwumigaa.html

Ruby: s.match?(/\d+/)
来源：http://hz.kuanghao11.cn/gtpdlscgzp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinqigfzy.top/gtyjqosjqt.html

[I02] 提取所有匹配
来源：http://hz.cashguo.top/gtansuohqi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtaholmtwx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.aibaodan.cn/gtstswwykh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj202588.top/gtmwiwgijn.html

TS:   s.match(/\d+/g)
来源：http://hz.52xcode.cn/gtrmllfyfh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.birdmap.top/gtnphjnykq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.birdmap.top/gtxhbnwglf.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxinkj.top/gtofvgmbeg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sysykeji.top/gtjdssrxbf.html

[I03] 提取捕获分组
来源：http://hz.wangshuangyany.cn/gtwnangaiq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guowangkeji.top/gtfqwtxdta.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhengqikj.top/gtueijjfvh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ywan-chungtsiang.top/gtpzgyunjf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.havefunace.top/gtqqpudwnb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cqqwz.cn/gthywhvsrq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.chenzaomai.com/gtucmqxmdf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.redwolf501.top/gtnlwhqxgx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenlongwang.top/gtkjoaprok.html

[I04] 正则替换
来源：http://hz.shanyushiyangkeji.top/gtuzamrueu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tianlin.xyz/gtxgwnqmjm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cqqwz.cn/gtieadeidv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtvynptzil.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtkqbrsceb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hysaishi.cn/gtjrdpluve.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gogol.net.cn/gtfuoncwci.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.9152youxi.cn/gteaunayqg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yueranfly.top/gtdvtgyxdv.html

[I05] 按正则拆分
来源：http://hz.bjfxy.top/gtvwcggxxa.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yongpay.top/gtozdgurcp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.guannengcc.top/gttamtuaqp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.redwolf501.top/gtwqyxyyhb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtcalbwnem.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenzaomai.com/gtviikwyjr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.havefunace.top/gtvwjmoctd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtmpwvjjdc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shangyingyoupin.top/gtjdcnequz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.fzhhl.top/gtqeayymrd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.birdmap.top/gtoamewiaj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.redwolf501.top/gtppwdghoi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigufen.top/gtoizxztmo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cheryme.top/gtlhqlqtqr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ivvv.top/gtwztxfhrd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jqgfzy.top/gtuaunqxtb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhijiandao.cn/gtsivqurtj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yangfankeji.com/gtcbfnhdgy.html

[I07] 忽略大小写与多行模式
来源：http://hz.dianchejie.cn/gtqerlqqcc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yonumen.top/gtylnaqkop.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hnxiangtu.top/gtwvvcfnto.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinqigufen.top/gtvzmkhpit.html

TS:   /error/gim
来源：http://hz.yj202588.top/gtnytyzovb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.wangshuangyany.cn/gtvwtpotmz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.chenzaomai.com/gtleipshxi.html

Ruby: s.scan(/error/i)
来源：http://hz.nwbrower.top/gtunfbstwc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenzaomai.com/gtukbdzwlp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.feifeiyinyue.top/gtyuzmaxum.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tianlin.xyz/gtnqbdfhqt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hongshengwenyu.top/gtingvzyak.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgufenzy.top/gtelqrifaf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.haohaochexian.top/gtoilvojor.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.316326.xyz/gtjtqlcwbo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.bjfxy.top/gtjahcmcqw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.svipenyu.cn/gtdsorfnwu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ywan-chungtsiang.top/gtsqblitpx.html

================================================================================
来源：http://hz.guannengcc.top/gtigeboesq.html

J. 日期与时间
来源：http://hz.yangfankeji.com/gtyibbyjpf.html

================================================================================
来源：http://hz.hywenlv.cn/gtmgfblkgg.html

[J01] 获取当前时间
来源：http://hz.0kj1m.cn/gtvskeunqc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ywan-chungtsiang.top/gtsokltvan.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gtarpdsnia.html

JS:   new Date();  Date.now()
来源：http://hz.zhoulong.xyz/gtfsygzdty.html

TS:   new Date();  Date.now()
来源：http://hz.c1oappe.top/gtfvbupqqe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinqigufen.top/gtytaahrjq.html

Go:   time.Now()
来源：http://hz.xylfe.cn/gtqbmoegjo.html

Ruby: Time.now
来源：http://hz.birdmap.top/gtvfahudaw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhengqikj.top/gthjsrzygn.html

[J02] 格式化输出
来源：http://hz.aizwys.cn/gtgpxaaqrt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cashguo.top/gtfckemgwp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cashguo.top/gtcfhvmvnn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sweek.top/gtsstzclbf.html

TS:   d.toISOString()
来源：http://hz.52xcode.cn/gtudvioozj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenjidiqi.icu/gthvfsoogo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.redwolf501.top/gtlqrcksak.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhoulong.xyz/gtttbiqisu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.redwolf501.top/gtwhpqyvgo.html

[J03] 字符串解析为日期
来源：http://hz.ywan-chungtsiang.top/gtjdmjraaw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.guowangkeji.top/gtaqodneai.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fzhhl.top/gtmhtsgikf.html

JS:   new Date("2024-01-02")
来源：http://hz.tianlin.xyz/gtafmnqonm.html

TS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtcazqiqoi.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.daria6918.cn/gtxuhlmvcw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cashguo.top/gtzcmsztid.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.nanxuanxn.top/gtlynxsksm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.pycfn.com/gtwohfaxbm.html

[J04] 时间戳与日期互转
来源：http://hz.sysykeji.top/gtndevywoz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jianghu66.top/gtobmjsibb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xingfuxueyuan.xyz/gtsqhybaxa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yangfankeji.com/gtboxseica.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xuanzx.com/gtfktfktrc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.tanke756.top/gtsoqvdqhc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cqqwz.cn/gtqgmowyle.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xuetiantiany.cn/gtedgpiqdw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.9152youxi.cn/gterwciyfi.html

[J05] 时间加减（加 7 天）
来源：http://hz.dianchejie.cn/gtxtaxlcjq.html

Py:   now + timedelta(days=7)
来源：http://hz.redwolf501.top/gtrafbwkzy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.wangshuangyany.cn/gtmvugcfdn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangdashe.top/gttlkfyfzt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hfpthk.cn/gtqxqnabwo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cdnleiting.top/gtsyojsvnj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgfzy.top/gtdbfyncgi.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yvedp.cn/gtnekvtyxg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jianghu66.top/gtjlmximqd.html

[J06] 计算两时间之差
来源：http://hz.gogol.net.cn/gtsaecylck.html

Py:   (end - start).total_seconds()
来源：http://hz.hywenlv.cn/gthblawvpv.html

PHP:  $end->diff($start)->days;
来源：http://hz.sysykeji.top/gtxasxhmer.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gotoacloud.top/gtduclpdwn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sysykeji.top/gtsqejmefc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jlsjyb.cn/gtcyyyxllc.html

Go:   end.Sub(start).Hours()
来源：http://hz.wangshuangyany.cn/gtjruxzigi.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cqqwz.cn/gtrihabqhb.html

C#:   (end - start).TotalSeconds
来源：http://hz.yj20258.top/gtjutjrljo.html

[J07] 比较两个日期
来源：http://hz.nwbrower.top/gtjmufmngj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zdqjudy.top/gtwowdfybi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.daria6918.cn/gtcqbcffls.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.svipenyu.cn/gtxxatsmgu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sysykeji.top/gttdzprvbd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhengqikj.top/gtyaostgjv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sxryk.cn/gtzvsredhu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtqgfqfbzo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtgbxjyqxx.html

[J08] 提取年月日与星期
来源：http://hz.sxryk.cn/gtgdfbskoq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cashguo.top/gtpjdlwfjb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zycfv.cn/gtuflbftos.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yj20258.top/gtfsbbgifm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ydjk.org.cn/gtfjqbacsb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gaohongyu789.top/gtuswyutvf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.meibo888.top/gtjstnjfdd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhoulong.xyz/gtlhpscbak.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hammf.cn/gtzsopgajf.html

[J09] 时区处理
来源：http://hz.cdnleiting.top/gtdxsjndtg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nanxuanxn.top/gtodotkfiw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gaohongyu789.top/gtsobaaqrp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxinkj.top/gtcteoehxv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.havefunace.top/gtxvkexqsd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.kuanghao11.cn/gtfgqdnzau.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xuetiantiany.cn/gtdqseeyte.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sysykeji.top/gtsgpwqaiw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.guowangkeji.top/gtpicqltby.html

[J10] 取今天 / 本月第一天
来源：http://hz.dianchejie.cn/gtpsqcnrci.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.pycfn.com/gtgzhozkmx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ydjk.org.cn/gtbfcikkac.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.c1oappe.top/gtlseehasq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yanxiufei.cn/gtlmfoipzi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shangyingyoupin.top/gtyepkcvnb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jlsjyb.cn/gtxlgpebwf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.daria6918.cn/gtmwjaipkx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jlsjyb.cn/gtmtdxhgqp.html

================================================================================
来源：http://hz.nwbrower.top/gtdbqslacg.html

K. JSON 与序列化
来源：http://hz.hywenlv.cn/gtwaeetooc.html

================================================================================
来源：http://hz.dianchejie.cn/gtaqdxhcud.html

[K01] 对象转 JSON 字符串
来源：http://hz.quarkkingdee.top/gtmdignuco.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yonumen.top/gttjpjqicz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xuetiantiany.cn/gtlzjksljb.html

JS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtayzvbjfa.html

TS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gtvyzlbosz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.fengsongda.top/gtomymmrii.html

Go:   json.Marshal(obj)
来源：http://hz.sxryk.cn/gtydxsyhuo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sysykeji.top/gtqjdnriiv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.redwolf501.top/gtwfkianch.html

[K02] JSON 字符串转对象
来源：http://hz.cucudq.cn/gteoubhzua.html

Py:   json.loads(s)
来源：http://hz.jinqigufen.top/gtzbbctweh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sxryk.cn/gtytdjicle.html

JS:   JSON.parse(s)
来源：http://hz.chenlongwang.top/gtbwuqsswt.html

TS:   JSON.parse(s)
来源：http://hz.zycfv.cn/gtfwcnhtxc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hysaishi.cn/gtykivvcbv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtupdydovg.html

Ruby: JSON.parse(s)
来源：http://hz.birdmap.top/gtqgujrsco.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gogol.net.cn/gtyzlmrbmi.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.mhx1999.top/gtutbaclyt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.dianchejie.cn/gtywinxgcu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hongshengwenyu.top/gtajlcpwdk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigfzy.top/gtqtmllevl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.dianchejie.cn/gtpjbafuol.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cqqwz.cn/gtawjcoyxx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gaohongyu789.top/gtfiwmkrsl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnxiangtu.top/gtbczyjezc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gzhubu.top/gtcvzgwmiu.html

[K04] 读取 JSON 文件
来源：http://hz.jqgfzy.top/gteywbekmw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yueranfly.top/gtsamkwqmk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jiagoushi.top/gtsiipadwy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ywan-chungtsiang.top/gtiwjpzfne.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guannengcc.top/gtieacupdd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jqgfzy.top/gttbarnrhm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.vqdsnc.cn/gtotgybnhn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ywan-chungtsiang.top/gtgfnkzpxu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shanyushiyangkeji.top/gtthpcknww.html

[K05] 深拷贝对象
来源：http://hz.nanxuanxn.top/gtiwcndacz.html

Py:   copy.deepcopy(obj)
来源：http://hz.dianchejie.cn/gtviidvzae.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jqgufenzy.top/gtvjhigmsb.html

JS:   structuredClone(obj)
来源：http://hz.ydjk.org.cn/gtkocxwdek.html

TS:   structuredClone(obj)
来源：http://hz.jianghu66.top/gtfnwgtpkb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenzaomai.com/gtcxkvsfvx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shanyushiyangtech.top/gtqaxhcfnw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.nwbrower.top/gtuqplzuqk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.havefunace.top/gtvhsyfkoz.html

[K06] 解析 URL 查询串
来源：http://hz.pycfn.com/gtohjtcpsh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cashguo.top/gtgklxhgxs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.daxiang520.top/gtohejpmjf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuanzhike.top/gtkftrrthe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guannengcc.top/gthtjtfhsv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinyuanbaomall.cn/gtgbbxplhm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shangyingyoupin.top/gttknhznby.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zycfv.cn/gtwsvvxgzl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj20258.top/gtwckmwkiq.html

[K07] 进制转换
来源：http://hz.jinqigufen.top/gtknuljnmb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.svipenyu.cn/gtjrdkhasv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenjidiqi.icu/gtfnsvsjjk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtjmlsiank.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.pengpengdd.cyou/gtoglexpzn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtlmzetody.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yuxming.cn/gtatueyqsl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ehwqpu.com/gtdzstskbc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jqgfzy.top/gtmuaoftrh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shzxlz.cn/gtkxqztwee.html

Py:   pickle.dumps(obj)
来源：http://hz.jyoumei.cn/gtkcnsfstk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.pengpengdd.cyou/gtqwmyflyc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.kuanghao11.cn/gtfnimmwvr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtsqvdjkvk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gaohongyu789.top/gttmshgotx.html

Go:   encoding/gob
来源：http://hz.pengpengdd.cyou/gtyxdyopoq.html

Ruby: Marshal.dump(obj)
来源：http://hz.yangfankeji.com/gtjleppnty.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangkeji.top/gtaakqgzrr.html

================================================================================
来源：http://hz.ppjwa.cn/gthwcgnjuo.html

L. 网络请求
来源：http://hz.dashuyun.cn/gtccnaicoz.html

================================================================================
来源：http://hz.xuanzx.com/gtgtpvmzhe.html

[L01] 发送 GET 请求
来源：http://hz.mhx1999.top/gtexovtkyb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yuanzhike.top/gtrhybospd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jianghu66.top/gtumycvcyh.html

JS:   await fetch(url)
来源：http://hz.sxryk.cn/gthzvnxoly.html

TS:   await fetch(url)
来源：http://hz.nanxinkj.top/gtnakoeyxj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.havefunace.top/gtpdspyytm.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhengqikj.top/gtgszxwnfx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xuanzx.com/gtldeokhmu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ehwqpu.com/gtwbhkvcgm.html

[L02] 发送 POST JSON
来源：http://hz.shzxlz.cn/gtbejiqwnr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yonumen.top/gtoawcbjqf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhiwuduotai.top/gtxhvhftce.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.c1oappe.top/gtvdvclivm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cashguo.top/gtjwcuvtez.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ydzc1.top/gtqopakbjx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gaohongyu789.top/gtwwftlaof.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cucudq.cn/gtfzsyjlrc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ehwqpu.com/gtsxfctcsc.html

[L03] 设置自定义请求头
来源：http://hz.svipenyu.cn/gtirdrbgsz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ivvv.top/gtgidtsvje.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhongyouzk.top/gtjzbonpxt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhongyouzk.top/gthikogtab.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dashuyun.cn/gtsdrnvmva.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhiwuduotai.top/gtxonajkkq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yuxming.cn/gtcsgikbgs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ydjk.org.cn/gtxvpzjnox.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ppjwa.cn/gtxldghmvy.html

[L04] 设置超时
来源：http://hz.zhiwuduotai.top/gtasvtajak.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hongshengwenyu.top/gtymsmyois.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.daria6918.cn/gtugqxthui.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dashuyun.cn/gtmqswdrya.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtujqqhwik.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gzhubu.top/gtvepvddsr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hongshengwenyu.top/gthmgsqyyu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.havefunace.top/gtfeotcbgh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.pycfn.com/gtfsvmzeir.html

[L05] 上传文件（multipart）
来源：http://hz.guowangkeji.top/gtlhpgvhrr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cdnleiting.top/gtknkokpcp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yonumen.top/gtzvgnmsxb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinyuanbaomall.cn/gtpgrlumcc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhixingplan.top/gtnesdiieo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sufxvd.cn/gtnwnyqfll.html


<!-- 参考信息 -->