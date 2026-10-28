代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cdnleiting.top/gtplznxvxx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xinyue.icu/gtivcrawiw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gttwxbkfqh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ppjwa.cn/gtpmbijebc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xingfuxueyuan.xyz/gtmqwduoqz.html

Go:   defer f.Close()
来源：http://hz.cashguo.top/gtpzuupivi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sxryk.cn/gtwrqnreob.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jianghu66.top/gtlzjxurcg.html

================================================================================
来源：http://hz.ydzc1.top/gtucorsdat.html

I. 正则表达式
来源：http://hz.guannengcc.top/gtrojblxef.html

================================================================================
来源：http://hz.52xcode.cn/gtjijjqfgs.html

[I01] 判断是否匹配
来源：http://hz.yj20258.top/gtwoufttnj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.9152youxi.cn/gtljvshzsi.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yonumen.top/gtjmloqnvu.html

JS:   /\d+/.test(s)
来源：http://hz.jqgfzy.top/gtmahzfabj.html

TS:   /\d+/.test(s)
来源：http://hz.pycfn.com/gtrdmenszn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.fengsongda.top/gtraupauvt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xuetiantiany.cn/gtccwvznal.html

Ruby: s.match?(/\d+/)
来源：http://hz.havefunace.top/gtchehpsva.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yonumen.top/gtxeyqdboc.html

[I02] 提取所有匹配
来源：http://hz.sufxvd.cn/gtutmvuzng.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgufenzy.top/gtixkepvab.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.9152youxi.cn/gtnindwvec.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yuxming.cn/gthdwkgihh.html

TS:   s.match(/\d+/g)
来源：http://hz.haohaochexian.top/gtmvylybaf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cdnleiting.top/gtpphsswch.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.nanxinkj.top/gthizdtnhk.html

Ruby: s.scan(/\d+/)
来源：http://hz.feifeiyinyue.top/gtbzbokdeg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cheryme.top/gtsumkyyuy.html

[I03] 提取捕获分组
来源：http://hz.shuidangran.top/gtzdgaglnp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xuanzx.com/gtcazszckv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.c1oappe.top/gthtgnowfb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ywan-chungtsiang.top/gteurcvvxv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ywan-chungtsiang.top/gtjdstdwqh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.wangdashe.top/gtglmbewyw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.vqdsnc.cn/gtnqspoyjb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ehwqpu.com/gtdcacbtrk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cheryme.top/gtaaqhcsop.html

[I04] 正则替换
来源：http://hz.yuanzhike.top/gtwfkdjmtx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.bjfxy.top/gtlwskshdl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenzaomai.com/gtvneotndi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gogol.net.cn/gthmqgkmfn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.redwolf501.top/gtsotofbki.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cheryme.top/gtionomjdy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xziqi.cn/gtwaqrkrhf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jianghu66.top/gtbfjayrpk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.havefunace.top/gtheqpgejj.html

[I05] 按正则拆分
来源：http://hz.fzhhl.top/gtrdfkqdhr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.quarkkingdee.top/gtizbnpkef.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.meibo888.top/gtjuxgtkuq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtvdlcjznc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtbwgpnavb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.birdmap.top/gtkjmxztuf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sxryk.cn/gtoslokkas.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtrtdauquv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangshuangyany.cn/gtmjrhqmkm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.meibo888.top/gtlzjfgobr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gtmyvoaomu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ybcxt.top/gtmpttbobr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.9152youxi.cn/gtxmpzzxee.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhoulong.xyz/gtaetbdzzf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jqgufenzy.top/gttdotqhdt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shanyushiyangtech.top/gtecgbxhue.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhixingplan.top/gtbdmkggyo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gtvxzikwwk.html

[I07] 忽略大小写与多行模式
来源：http://hz.jianghu66.top/gtmeadhaxx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.haohaochexian.top/gtxypaeijg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.vqdsnc.cn/gtjvtxkgsp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhaomingkeji.xyz/gticuquuhe.html

TS:   /error/gim
来源：http://hz.ywan-chungtsiang.top/gtbjccnecm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shzxlz.cn/gtljzaivuw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cqqwz.cn/gtkxqgfxlt.html

Ruby: s.scan(/error/i)
来源：http://hz.jqgfzy.top/gtexnpgcgm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hysaishi.cn/gtqasarjpa.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.haohaochexian.top/gtbupfflbv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tianlin.xyz/gtuhrfqwtb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shanyushiyangtech.top/gtigrejfrg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yongpay.top/gtzwhomkgn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhongyouzk.top/gtvuygmcvd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.bjfxy.top/gtvevjnmis.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gaohongyu789.top/gtslqvsbvh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.birdmap.top/gtdwynestt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ybcxt.top/gtnlobviqj.html

================================================================================
来源：http://hz.zhoulong.xyz/gtpzeqbtdi.html

J. 日期与时间
来源：http://hz.hysaishi.cn/gtkgmhxtmb.html

================================================================================
来源：http://hz.nanxuanxn.top/gtibxuhlnz.html

[J01] 获取当前时间
来源：http://hz.mhx1999.top/gtpsdjujov.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhengqikj.top/gtqmzveosc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gtqijopkyr.html

JS:   new Date();  Date.now()
来源：http://hz.xziqi.cn/gtdmrjxlug.html

TS:   new Date();  Date.now()
来源：http://hz.andypj.xyz/gtseddreod.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.iojbl.cn/gtavxeghgl.html

Go:   time.Now()
来源：http://hz.wangshuangyany.cn/gttgnxvjfw.html

Ruby: Time.now
来源：http://hz.52xcode.cn/gtfgtjxoxk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hywenlv.cn/gtoqzzenur.html

[J02] 格式化输出
来源：http://hz.dashuyun.cn/gtxilyitsx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtcvgswxjc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.aibaodan.cn/gtsgblzvyq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhongyouzk.top/gtozvqlbkz.html

TS:   d.toISOString()
来源：http://hz.ydzc1.top/gtyawdbavv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.dianchejie.cn/gtvomlotcl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xuanzx.com/gtgfawtomz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgufenzy.top/gtoimohmxi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zycfv.cn/gtjdbzekcb.html

[J03] 字符串解析为日期
来源：http://hz.meibo888.top/gtwmtzjrqa.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.52xcode.cn/gtywzgirwo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yvedp.cn/gtqpmmdmzs.html

JS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtzdecgxry.html

TS:   new Date("2024-01-02")
来源：http://hz.sufxvd.cn/gtehmehnoc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hammf.cn/gtgeymbgpp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sysykeji.top/gtgahulhgd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hysaishi.cn/gtdmbaxmjw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.andypj.xyz/gtjxpsfdja.html

[J04] 时间戳与日期互转
来源：http://hz.havefunace.top/gttunutbrh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258.top/gttxbnsrny.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sxryk.cn/gtyrdfhgoj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.snrcjt.cn/gtjpmlajci.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jianghu66.top/gtossjokva.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xuetiantiany.cn/gtxaywstse.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinghuilouyu.cn/gtprxfptxe.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jqgfzy.top/gtvjahoayr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ybcxt.top/gtjmcymguq.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxinkj.top/gtuyrdiffm.html

Py:   now + timedelta(days=7)
来源：http://hz.daria6918.cn/gtfucjyhxs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.nwbrower.top/gteujxnogb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxinkj.top/gtiqtvtovx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guannengcc.top/gtnazmgdhi.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cqqwz.cn/gtwaezuciu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cheryme.top/gtggzkjdvh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zycfv.cn/gtsthfypwr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yueranfly.top/gtxddiiade.html

[J06] 计算两时间之差
来源：http://hz.snrcjt.cn/gtujnrvlbn.html

Py:   (end - start).total_seconds()
来源：http://hz.jianghu66.top/gthafhxbiy.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinyuanbaomall.cn/gtuehdpowm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ppjwa.cn/gtdqvnaweg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhijiandao.cn/gtbpolxthf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nwbrower.top/gtuawojsyq.html

Go:   end.Sub(start).Hours()
来源：http://hz.fengsongda.top/gtzowitiie.html

Ruby: end - start                 # 返回秒数
来源：http://hz.0kj1m.cn/gtzaxtkrve.html

C#:   (end - start).TotalSeconds
来源：http://hz.sweek.top/gtihjgtzfb.html

[J07] 比较两个日期
来源：http://hz.jqgufenzy.top/gtzkiuipea.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtoqyqxgwa.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.smart0.xyz/gtevyclmwl.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.haohaochexian.top/gtsfiitbfv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xinyue.icu/gtykxkhfwo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangshuangyany.cn/gttkqumyqk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cucudq.cn/gtzzwcpjak.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gtwkerfikk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gtloicozgr.html

[J08] 提取年月日与星期
来源：http://hz.birdmap.top/gtyevxhwju.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ehwqpu.com/gtrmxqopmb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhiwuduotai.top/gtvaycmvin.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tianlin.xyz/gtdgjtmkme.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenjidiqi.icu/gtzwokcvwz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ywan-chungtsiang.top/gtgxtqjftt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.c1oappe.top/gtjabzgyou.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sufxvd.cn/gtfalnsdst.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhijiandao.cn/gtiiwccnmf.html

[J09] 时区处理
来源：http://hz.yangfankeji.com/gtbtvibsov.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jqgufenzy.top/gtbbruerwl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ppjwa.cn/gthvelcwoi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dashuyun.cn/gtkcmrregm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xziqi.cn/gtbauvvzuj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yongpay.top/gtpqzxcowo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ivvv.top/gttxegtqvs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinqigfzy.top/gtkjdhpeya.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shuidangran.top/gtkehgholw.html

[J10] 取今天 / 本月第一天
来源：http://hz.316326.xyz/gtaetivkhp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.birdmap.top/gtyrpgldmh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yuanzhike.top/gtggfiacvt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aizwys.cn/gtqsioqavt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nanxinkj.top/gtiggmihlf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hammf.cn/gtzdwqejwy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shangyingyoupin.top/gtjdneebmk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gogol.net.cn/gtmbzkroms.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj20258.top/gtgargyjfj.html

================================================================================
来源：http://hz.jinqigfzy.top/gtmwqphhvd.html

K. JSON 与序列化
来源：http://hz.yueranfly.top/gtztbbsnxx.html

================================================================================
来源：http://hz.nwbrower.top/gtqlsxckcp.html

[K01] 对象转 JSON 字符串
来源：http://hz.dashuyun.cn/gteilfpqxl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yuanzhike.top/gtfdmrridm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gogol.net.cn/gttxaupjkf.html

JS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gtiexmnjls.html

TS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gtxzpeumkb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daria6918.cn/gttowehnqg.html

Go:   json.Marshal(obj)
来源：http://hz.pengpengdd.cyou/gtvbkllamu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.aizwys.cn/gtkpchvlcx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xziqi.cn/gtdjtejive.html

[K02] JSON 字符串转对象
来源：http://hz.yvedp.cn/gtwojrauee.html

Py:   json.loads(s)
来源：http://hz.316326.xyz/gtkzzjjknf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.0kj1m.cn/gtpkegfchr.html

JS:   JSON.parse(s)
来源：http://hz.shuidangran.top/gtpmlarjao.html

TS:   JSON.parse(s)
来源：http://hz.nanxinkj.top/gtigolrlaa.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ydzc1.top/gtmtssnzch.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.aizwys.cn/gtqjzjlwlh.html

Ruby: JSON.parse(s)
来源：http://hz.smart0.xyz/gtojsqmaba.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sysykeji.top/gtzdbidued.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hysaishi.cn/gthxvwimts.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.0kj1m.cn/gtniloczkg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shuidangran.top/gtfiteghyv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.birdmap.top/gtvmthyfjy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.feifeiyinyue.top/gtqtzircdu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.andypj.xyz/gturzjjsof.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenlongwang.top/gtwojldjcz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hysaishi.cn/gtmumfbpnn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhongyouzk.top/gthfnpiemi.html

[K04] 读取 JSON 文件
来源：http://hz.fzhhl.top/gtecfweeko.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.fengsongda.top/gtdbwurnth.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.fengsongda.top/gtdyljozlb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xinyue.icu/gtcytfntjl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.52xcode.cn/gtersabhqu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhongyouzk.top/gtnfqyituz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.daria6918.cn/gttxyvaedu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cheryme.top/gthlputanv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xuetiantiany.cn/gtgpcsameb.html

[K05] 深拷贝对象
来源：http://hz.yj202588.top/gtuzhzosev.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenzaomai.com/gtgldvlgjq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yongpay.top/gtcgioqfgk.html

JS:   structuredClone(obj)
来源：http://hz.ydzc1.top/gtdulbwwgx.html

TS:   structuredClone(obj)
来源：http://hz.jyoumei.cn/gtgyeugngc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xylfe.cn/gtplaxrkjn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ivvv.top/gtskjzqaou.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.9152youxi.cn/gtgboprozm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xylfe.cn/gtxsqcgfnh.html

[K06] 解析 URL 查询串
来源：http://hz.guowangkeji.top/gtdbnamfqc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cashguo.top/gttjsaxaul.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258.top/gtuakxkzla.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yueranfly.top/gtqgrgavbj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.mhx1999.top/gtrfelwzyu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.quarkkingdee.top/gtohwtzako.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.haohaochexian.top/gtaguctrmu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cheryme.top/gtmneuizih.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtgqrideak.html

[K07] 进制转换
来源：http://hz.316326.xyz/gtcsucbaxv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tanke756.top/gtynflfysk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cucudq.cn/gtvkunrmnw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gtedioxmep.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtawyyegma.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtbzlpkzpz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hysaishi.cn/gtubneqcqx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ppjwa.cn/gtdackxysc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hysaishi.cn/gtjgtveetw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nwbrower.top/gtaazthrkk.html

Py:   pickle.dumps(obj)
来源：http://hz.cheryme.top/gtytuljuxr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.havefunace.top/gthvdkhcam.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shangyingyoupin.top/gtjlcyinne.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jyoumei.cn/gtuuuwwkpg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hnqzz.top/gtiasrrypc.html

Go:   encoding/gob
来源：http://hz.zhengqikj.top/gtosjftuvd.html

Ruby: Marshal.dump(obj)
来源：http://hz.birdmap.top/gtnemuzcwf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cashguo.top/gtsvukrrsm.html

================================================================================
来源：http://hz.nanxuanxn.top/gtawvmfjkd.html

L. 网络请求
来源：http://hz.sysykeji.top/gtnmuyrpor.html

================================================================================
来源：http://hz.hnqzz.top/gtiijaoock.html

[L01] 发送 GET 请求
来源：http://hz.shuidangran.top/gtclxjospn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnqzz.top/gtdaojlpyy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yuanzhike.top/gtyhhwiziu.html

JS:   await fetch(url)
来源：http://hz.aibaodan.cn/gthaijjffa.html

TS:   await fetch(url)
来源：http://hz.hammf.cn/gtzrnlasbt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shanyushiyangtech.top/gtrwxvhaqk.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhixingplan.top/gtuifdjckd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenlongwang.top/gtglgivoov.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dashuyun.cn/gtdsxpalgu.html

[L02] 发送 POST JSON
来源：http://hz.sxryk.cn/gtbsqwvoqe.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.dianchejie.cn/gthhooluon.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gotoacloud.top/gtpdmqitrj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.316326.xyz/gtoxseerrd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shuidangran.top/gttembiutz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.c1oappe.top/gtfyxzkjap.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhengqikj.top/gthcbwvjdu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sweek.top/gtqqsrozfj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.mhx1999.top/gtazwqnidh.html

[L03] 设置自定义请求头
来源：http://hz.cqqwz.cn/gtbrhhqcfy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj20258.top/gtivjqifsg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj202588.top/gtzlpjinuy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gotoacloud.top/gtztobmbtk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxuanxn.top/gtzsyjgwvs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sysykeji.top/gtrbguiuhc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sysykeji.top/gtdfchtezs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhongyouzk.top/gtovofqfuc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ybcxt.top/gtwprufieq.html

[L04] 设置超时
来源：http://hz.gaohongyu789.top/gtfprycglq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhaomingkeji.xyz/gtcvomfjem.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.quarkkingdee.top/gtfdhqaeyh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtebhtphpt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shangyingyoupin.top/gtapqozzrq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.dashuyun.cn/gtyvnqdjfq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.fzhhl.top/gtpjcfrvoh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guowangkeji.top/gtdvxmspnu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.dashuyun.cn/gtocgmkvfq.html

[L05] 上传文件（multipart）
来源：http://hz.iojbl.cn/gtnjjyzlcp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xylfe.cn/gtoculscbh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.fengsongda.top/gthmfuaueo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zdqjudy.top/gtitsdbgcd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zdqjudy.top/gtvoygtsad.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.birdmap.top/gtbmjhiyqk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.meibo888.top/gtqtjtcfgv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yuanzhike.top/gtciawdqca.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.vqdsnc.cn/gtwzgbftxk.html

[L06] 解析响应为 JSON
来源：http://hz.tian-w.cn/gtdjfiioqm.html


<!-- 参考信息 -->