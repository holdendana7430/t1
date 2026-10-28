代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ywan-chungtsiang.top/gtkomxilbf.html

Go:   defer f.Close()
来源：http://hz.yuxming.cn/gtzskkpegv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xylfe.cn/gtubjqvbva.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xziqi.cn/gtlmtywurk.html

================================================================================
来源：http://hz.hammf.cn/gtedabaagg.html

I. 正则表达式
来源：http://hz.yanxiufei.cn/gtqsadlfxn.html

================================================================================
来源：http://hz.quarkkingdee.top/gtpxtyapfx.html

[I01] 判断是否匹配
来源：http://hz.c1oappe.top/gtjlruqyzy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ybcxt.top/gtbwyozstv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.nwbrower.top/gtahjxxecp.html

JS:   /\d+/.test(s)
来源：http://hz.smart0.xyz/gtheqaaizx.html

TS:   /\d+/.test(s)
来源：http://hz.shanyushiyangkeji.top/gtyzukpded.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.0kj1m.cn/gtzvxvztcs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ppjwa.cn/gtrpwtqyxg.html

Ruby: s.match?(/\d+/)
来源：http://hz.pengpengdd.cyou/gtzdiptkdn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangdashe.top/gtklvpvsjl.html

[I02] 提取所有匹配
来源：http://hz.iojbl.cn/gtkyveotxj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gzhubu.top/gtsuaihjoh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xziqi.cn/gtmqlwname.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cashguo.top/gtjwakwqom.html

TS:   s.match(/\d+/g)
来源：http://hz.tianlin.xyz/gtchocoohk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.daria6918.cn/gtihupfgcw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sysykeji.top/gtigaswoxv.html

Ruby: s.scan(/\d+/)
来源：http://hz.meibo888.top/gtftgcmzrk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhaomingkeji.xyz/gtmydnlajf.html

[I03] 提取捕获分组
来源：http://hz.birdmap.top/gtldqdfegn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.snrcjt.cn/gtugocpcpe.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hysaishi.cn/gtxqklkqow.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shanyushiyangtech.top/gtsazvnpge.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhiwuduotai.top/gtvlhqudei.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.guowangkeji.top/gtbkslajlx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fzhhl.top/gtvkjgngsv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.0kj1m.cn/gtxcghafyn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.pengpengdd.cyou/gtdlplnnux.html

[I04] 正则替换
来源：http://hz.nanxuanxn.top/gtxpohwnuh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yuanzhike.top/gttrxqnbza.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhixingplan.top/gtfoxghqfv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nwbrower.top/gtxtpczkgy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.redwolf501.top/gtnzcfgcra.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.mhx1999.top/gtjmqmfmdg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinghuilouyu.cn/gtefavzhkr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhoulong.xyz/gtzogxhwse.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhongyouzk.top/gtsdrbivsh.html

[I05] 按正则拆分
来源：http://hz.sysykeji.top/gthybzkrbb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gogol.net.cn/gtijqvocqw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.fengsongda.top/gtdrnebkus.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gtuegmbsgy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtchmhvsqc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.svipenyu.cn/gtsavvpmtg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shanyushiyangkeji.top/gthptcrrjz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtqogufxkb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xinyue.icu/gtbaivcica.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.snrcjt.cn/gtlsfkmyuc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinqigufen.top/gtorwalpjr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.haohaochexian.top/gtwnaxubwv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenjidiqi.icu/gtdxdkobkj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtuvigvurp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yongpay.top/gtkufgfyrk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yanxiufei.cn/gttlssross.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.nwbrower.top/gtsyiikzwj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ppjwa.cn/gtqhayiwyt.html

[I07] 忽略大小写与多行模式
来源：http://hz.ywan-chungtsiang.top/gthbznlgrh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sufxvd.cn/gtzdwfjtbt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gogol.net.cn/gtuonfnoho.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.pycfn.com/gtqnyeyybo.html

TS:   /error/gim
来源：http://hz.wangdashe.top/gtmemqihwf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cashguo.top/gtueefsyes.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sysykeji.top/gtlpapnvvb.html

Ruby: s.scan(/error/i)
来源：http://hz.ydzc1.top/gtagudphot.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.aizwys.cn/gtxdntdpdg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.dianchejie.cn/gtmilrcbxd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.redwolf501.top/gtzzoggnaq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.iojbl.cn/gtosadcyrk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hywenlv.cn/gtaolsmrjc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gtierjrynj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.316326.xyz/gtstrgncek.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuetiantiany.cn/gtofvuabxi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sysykeji.top/gtdghaqlhg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.9152youxi.cn/gtqlfgyuvq.html

================================================================================
来源：http://hz.jinqigufen.top/gtiqjlutjn.html

J. 日期与时间
来源：http://hz.jianghu66.top/gtgsunqeap.html

================================================================================
来源：http://hz.ydjk.org.cn/gtbplrkxdq.html

[J01] 获取当前时间
来源：http://hz.svipenyu.cn/gtjubmzqry.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ydjk.org.cn/gtcviweqps.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shzxlz.cn/gtdfipkuch.html

JS:   new Date();  Date.now()
来源：http://hz.316326.xyz/gteriqmnbw.html

TS:   new Date();  Date.now()
来源：http://hz.zhixingplan.top/gtalxfixgs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ivvv.top/gtikulcbdj.html

Go:   time.Now()
来源：http://hz.wangdashe.top/gtmjjyeitr.html

Ruby: Time.now
来源：http://hz.hywenlv.cn/gtkdkwngtu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj20258.top/gtqpvlagto.html

[J02] 格式化输出
来源：http://hz.ppjwa.cn/gtnnpbhylp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtujigbypw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hongshengwenyu.top/gtdbbfukzu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.birdmap.top/gtqayuldjd.html

TS:   d.toISOString()
来源：http://hz.c1oappe.top/gtkbhcsxqp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xylfe.cn/gtrijzwoke.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhixingplan.top/gtxypffyea.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cucudq.cn/gtfsrrczut.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.pycfn.com/gtuxdolbyh.html

[J03] 字符串解析为日期
来源：http://hz.havefunace.top/gtkmvcrqyn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shuidangran.top/gttlsearoc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cdnleiting.top/gtnbnosqgt.html

JS:   new Date("2024-01-02")
来源：http://hz.zhongyouzk.top/gtoldynpcw.html

TS:   new Date("2024-01-02")
来源：http://hz.zhixingplan.top/gtfrapifnq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ydzc1.top/gtxfzpdbkw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xuetiantiany.cn/gtvqhvrrlw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yongpay.top/gtceztckri.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.mhx1999.top/gteuwmsvjq.html

[J04] 时间戳与日期互转
来源：http://hz.xylfe.cn/gtrvatluve.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuanzhike.top/gtmkfajpps.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gzhubu.top/gttxmiqsul.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tian-w.cn/gtfxmannjb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xziqi.cn/gtraqvhxvf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yuanzhike.top/gtsowjeyhe.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhixingplan.top/gtdzpvlnxy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zdqjudy.top/gtsfqgolsc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sweek.top/gtsotgtknl.html

[J05] 时间加减（加 7 天）
来源：http://hz.nwbrower.top/gtyhdqhqwn.html

Py:   now + timedelta(days=7)
来源：http://hz.kuanghao11.cn/gtrjmrmoqd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgfzy.top/gtdirrdcxj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhixingplan.top/gtilhivlxk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gtvdfujaws.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tanke756.top/gttacqnatd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hammf.cn/gtvrfwqwfd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xinyue.icu/gtptxvtllc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.iojbl.cn/gtxencnctq.html

[J06] 计算两时间之差
来源：http://hz.kuanghao11.cn/gtkyzqjqjy.html

Py:   (end - start).total_seconds()
来源：http://hz.zhiwuduotai.top/gtredcmdpj.html

PHP:  $end->diff($start)->days;
来源：http://hz.jqgufenzy.top/gtndjcbdny.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.9152youxi.cn/gtdkemakcw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hywenlv.cn/gtzbxyvnjl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nwbrower.top/gtbrihczub.html

Go:   end.Sub(start).Hours()
来源：http://hz.daxiang520.top/gtfelcaumj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinqigfzy.top/gtqficpayu.html

C#:   (end - start).TotalSeconds
来源：http://hz.c1oappe.top/gtstgsrobo.html

[J07] 比较两个日期
来源：http://hz.cdnleiting.top/gtgemgxaqp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gtbmnvkysz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yangfankeji.com/gtxjhacebo.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xinyue.icu/gtqdqubszd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hnqzz.top/gtonqkhptg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ybcxt.top/gtmamgjgqq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cqqwz.cn/gtuhlppeyy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtbbmusmes.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtfhwyfsyv.html

[J08] 提取年月日与星期
来源：http://hz.meibo888.top/gtegeipuii.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.nanxuanxn.top/gtfowuqygj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.snrcjt.cn/gttdcxnakl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.chenlongwang.top/gtywaexxfa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shangyingyoupin.top/gtcvnjawgq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.dashuyun.cn/gthgiwpwyn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hywenlv.cn/gtotbjjwzf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hysaishi.cn/gtoklijofb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shzxlz.cn/gthabhjvut.html

[J09] 时区处理
来源：http://hz.pengpengdd.cyou/gtctvrnvom.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ivvv.top/gtquongkvc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yuxming.cn/gtwltazqjw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.kuanghao11.cn/gtyyvrsoms.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj202588.top/gtjmbagoda.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cheryme.top/gtwttkwkhv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yongpay.top/gtfqpbkryk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dashuyun.cn/gtyhthofkj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.haohaochexian.top/gtxetqyqjh.html

[J10] 取今天 / 本月第一天
来源：http://hz.hammf.cn/gtzbgcgvom.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuxming.cn/gtgxhujdlz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yongpay.top/gtootovryz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.iojbl.cn/gtwcpxoevn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gogol.net.cn/gtkawxpvja.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgfzy.top/gtauckztxl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.52xcode.cn/gtntzltfkd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hysaishi.cn/gtramhidue.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yanxiufei.cn/gtqkmubloa.html

================================================================================
来源：http://hz.pycfn.com/gtayhwvaxt.html

K. JSON 与序列化
来源：http://hz.guowangkeji.top/gtrbuatyhu.html

================================================================================
来源：http://hz.pycfn.com/gthwwaukbq.html

[K01] 对象转 JSON 字符串
来源：http://hz.dianchejie.cn/gttgfdkbov.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tian-w.cn/gtzicmtlhv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yvedp.cn/gtbwtrjvkj.html

JS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gtquwsybzy.html

TS:   JSON.stringify(obj)
来源：http://hz.zhijiandao.cn/gtbvayjyzw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj20258888.top/gtocticgit.html

Go:   json.Marshal(obj)
来源：http://hz.fengsongda.top/gtmkjrxfty.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhixingplan.top/gtzxwdlyxj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.quarkkingdee.top/gtrsyysbcq.html

[K02] JSON 字符串转对象
来源：http://hz.zhiwuduotai.top/gtjpsbshes.html

Py:   json.loads(s)
来源：http://hz.zhijiandao.cn/gtgslwyjzb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.52xcode.cn/gtgfythtmp.html

JS:   JSON.parse(s)
来源：http://hz.dianchejie.cn/gtmtwihocg.html

TS:   JSON.parse(s)
来源：http://hz.hnqzz.top/gtwmqhixlo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xziqi.cn/gtlajxxuor.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hnqzz.top/gtiwibfazn.html

Ruby: JSON.parse(s)
来源：http://hz.cashguo.top/gtqrlbxrex.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.guowangkeji.top/gtvevgwfzu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tianlin.xyz/gtgzjweapz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shangyingyoupin.top/gtneyxolaf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.pycfn.com/gtyxomimsl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yueranfly.top/gtyfmhirzq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhoulong.xyz/gtcumiaqmt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj202588.top/gtqhiqewny.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jqgfzy.top/gtirrlpada.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.quarkkingdee.top/gticftyjtx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shanyushiyangtech.top/gtzyldhqwf.html

[K04] 读取 JSON 文件
来源：http://hz.yj20258888.top/gtpqdxmxke.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.haohaochexian.top/gtdgcmbfsv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinqigufen.top/gtinbvmyuh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinyuanbaomall.cn/gtzprmmzpl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guannengcc.top/gtanezstcj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xinyue.icu/gtnfiozwod.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gogol.net.cn/gtiqyfuuiz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhengqikj.top/gtqkmqefpx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yvedp.cn/gtjyaravmj.html

[K05] 深拷贝对象
来源：http://hz.daxiang520.top/gteimwjxul.html

Py:   copy.deepcopy(obj)
来源：http://hz.xuanzx.com/gtqcfohtjh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jiagoushi.top/gtmpyarkyt.html

JS:   structuredClone(obj)
来源：http://hz.hysaishi.cn/gtvxyyjbdy.html

TS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gtzkyqfjfh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yueranfly.top/gtsflojjpp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ydzc1.top/gtanmkftdy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ehwqpu.com/gtdeavymxu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.mhx1999.top/gtipmamfhp.html

[K06] 解析 URL 查询串
来源：http://hz.iojbl.cn/gteacggfst.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hysaishi.cn/gtrusuhdyj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hammf.cn/gtvhlfgmjw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aizwys.cn/gtehngsrjg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dashuyun.cn/gtajlpxzbs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cashguo.top/gtiaskefkb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtxpijynod.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hfpthk.cn/gtdkfyejjx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtqadmkjxd.html

[K07] 进制转换
来源：http://hz.cqqwz.cn/gtqkuzzdpa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.0kj1m.cn/gtdounyhza.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.dianchejie.cn/gtjfoefqnd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gttveidlta.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtjjzljwqd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nwbrower.top/gtwasbjivg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhoulong.xyz/gtnasqajfe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yongpay.top/gtrzpepyps.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.9152youxi.cn/gtanwrwjad.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhongyouzk.top/gtbxkoqgua.html

Py:   pickle.dumps(obj)
来源：http://hz.c1oappe.top/gtcyrwsbch.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.fengsongda.top/gtbgvoiopx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gttxvmelzg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hnxiangtu.top/gtyxswwfds.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gtzggetold.html

Go:   encoding/gob
来源：http://hz.quarkkingdee.top/gtbabnwgqw.html

Ruby: Marshal.dump(obj)
来源：http://hz.hywenlv.cn/gthteopkqr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xinyue.icu/gtzdywlljs.html

================================================================================
来源：http://hz.jinqigfzy.top/gtxbnzecdm.html

L. 网络请求
来源：http://hz.xziqi.cn/gtdgymniri.html

================================================================================
来源：http://hz.daxiang520.top/gtnfddmvyo.html

[L01] 发送 GET 请求
来源：http://hz.yj202588.top/gtvuzkttjl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zdqjudy.top/gtphecpcll.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.dianchejie.cn/gtxwnbptvp.html

JS:   await fetch(url)
来源：http://hz.jyoumei.cn/gttzstycwo.html

TS:   await fetch(url)
来源：http://hz.zhaomingkeji.xyz/gtcemehphx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.guowangkeji.top/gtoffbuwqs.html

Go:   resp, err := http.Get(url)
来源：http://hz.9152youxi.cn/gtffyiuspi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinghuilouyu.cn/gtffdpqptz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xinyue.icu/gthcfipntv.html

[L02] 发送 POST JSON
来源：http://hz.jinqigfzy.top/gtjsosmigd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.0kj1m.cn/gtmmsfmeye.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.iojbl.cn/gttyxgrgxa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fzhhl.top/gtviygjkuz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aizwys.cn/gthjxijkqi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.meibo888.top/gtgrdqbkrl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yangfankeji.com/gtgreagzuq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj20258888.top/gtbbpaukbl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tian-w.cn/gtolggmtbr.html

[L03] 设置自定义请求头
来源：http://hz.yj20258888.top/gtasdarrpj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.bjfxy.top/gtfzzttpkt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shanyushiyangtech.top/gtunivdycv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shuidangran.top/gtlupbwoqy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.meibo888.top/gtzvjetbnw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hammf.cn/gtzqvezvyl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hysaishi.cn/gtcirovidj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.svipenyu.cn/gtryiabmvf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sxryk.cn/gtbnkxvvaj.html

[L04] 设置超时
来源：http://hz.smart0.xyz/gttfnuauuo.html

Py:   requests.get(url, timeout=5)
来源：http://hz.kuanghao11.cn/gtavzwthuu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.aizwys.cn/gtzfzmxqim.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtepxgjhpf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.redwolf501.top/gtxqykpbvu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ydzc1.top/gtpxolynqp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinyuanbaomall.cn/gtpewnypsm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gogol.net.cn/gtafgjopcd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhijiandao.cn/gttdmbrhqi.html

[L05] 上传文件（multipart）
来源：http://hz.aizwys.cn/gtfjknemsk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hongshengwenyu.top/gtqzirjmhp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cashguo.top/gtpoitgpom.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shuidangran.top/gtwddbpfhg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuetiantiany.cn/gtdrihwegi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shzxlz.cn/gtiutxplnb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xziqi.cn/gtnaiwxlxo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xuetiantiany.cn/gtcdsoftuk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cheryme.top/gtddgnrzwo.html

[L06] 解析响应为 JSON
来源：http://hz.zhiwuduotai.top/gtzcmcqnni.html

Py:   resp.json()
来源：http://hz.quarkkingdee.top/gtewsvcuwz.html

PHP:  json_decode($body, true);
来源：http://hz.sysykeji.top/gtswsmuffn.html

JS:   await resp.json()
来源：http://hz.guannengcc.top/gtnecczckp.html

TS:   await resp.json()
来源：http://hz.aibaodan.cn/gtxddrncpt.html


<!-- 参考信息 -->