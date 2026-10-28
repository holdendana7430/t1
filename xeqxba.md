代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.meibo888.top/gthefmpxkm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cucudq.cn/gtsralavez.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ybcxt.top/gtvralyrte.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258.top/gtuexjqmyc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.svipenyu.cn/gtlzanuyzs.html

Go:   defer f.Close()
来源：http://hz.jqgufenzy.top/gtisuymyxy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhoulong.xyz/gtlwckcnzd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cqqwz.cn/gtbqwghemd.html

================================================================================
来源：http://hz.hammf.cn/gtferpvvem.html

I. 正则表达式
来源：http://hz.shanyushiyangtech.top/gtsqvatnkn.html

================================================================================
来源：http://hz.hammf.cn/gtoewljdxn.html

[I01] 判断是否匹配
来源：http://hz.redwolf501.top/gtogfpmxzu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xuanzx.com/gtesegmcwe.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.daxiang520.top/gtkqhhpjwj.html

JS:   /\d+/.test(s)
来源：http://hz.redwolf501.top/gtfwggpinc.html

TS:   /\d+/.test(s)
来源：http://hz.sysykeji.top/gtjtcuqmgz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zycfv.cn/gtknbarhqx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenjidiqi.icu/gtlwbatwih.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinghuilouyu.cn/gtyuizlkwr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.vqdsnc.cn/gtuuwugybe.html

[I02] 提取所有匹配
来源：http://hz.dashuyun.cn/gtgcprvaih.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nwbrower.top/gtdbxggfdg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xylfe.cn/gtekmazago.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.havefunace.top/gtmghadelm.html

TS:   s.match(/\d+/g)
来源：http://hz.xinyue.icu/gtjudyvqkn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.aibaodan.cn/gtthnvcrhy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.snrcjt.cn/gtrzibqxeu.html

Ruby: s.scan(/\d+/)
来源：http://hz.jiagoushi.top/gtfpnebhfv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zdqjudy.top/gtpctzocja.html

[I03] 提取捕获分组
来源：http://hz.pycfn.com/gtktibnfqr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yueranfly.top/gtkjhkbtmp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.fzhhl.top/gttrteoowq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhaomingkeji.xyz/gtqbndhsid.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.mhx1999.top/gtewmmqfoz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhongyouzk.top/gtjewgrauz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fengsongda.top/gtqmvgwciy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhiwuduotai.top/gtbfkiklcz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhijiandao.cn/gttvlaoclh.html

[I04] 正则替换
来源：http://hz.zhixingplan.top/gtewjecuwv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.meibo888.top/gtkenpcmfe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenjidiqi.icu/gtdsxcsmec.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtgogacwxc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.haohaochexian.top/gthqjjfkun.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yonumen.top/gtxpwegicf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj202588.top/gtfujowqfh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cheryme.top/gtrtwxbrtz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sxryk.cn/gtkhredklp.html

[I05] 按正则拆分
来源：http://hz.zhiwuduotai.top/gtbowdzqow.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sxryk.cn/gtynffghsy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.0kj1m.cn/gtizchszel.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gtzccngnjk.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtewnmdrab.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cucudq.cn/gtlaxcennc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.wangshuangyany.cn/gtqdhncjml.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cucudq.cn/gtzdjpgpsu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ivvv.top/gtxkbcsfus.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.c1oappe.top/gtgqzcstqv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.daxiang520.top/gtrttrhliz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.vqdsnc.cn/gtrvayqlmw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jyoumei.cn/gtrghmbhri.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtimodnpib.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aibaodan.cn/gtahifpwac.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yuxming.cn/gtxvvhkjcg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.pengpengdd.cyou/gtojwffllk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ybcxt.top/gtzcvcjmcl.html

[I07] 忽略大小写与多行模式
来源：http://hz.wangdashe.top/gttrejcsil.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tanke756.top/gtooajhsve.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xinyue.icu/gteuarhfmx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yueranfly.top/gtngoflcey.html

TS:   /error/gim
来源：http://hz.wangshuangyany.cn/gtnrqahaov.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sufxvd.cn/gtdfimfuga.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.mhx1999.top/gtgmoofbep.html

Ruby: s.scan(/error/i)
来源：http://hz.52xcode.cn/gtlinbigjc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.c1oappe.top/gtekkudsgf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hfpthk.cn/gtrqywfekm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ybcxt.top/gtoidjvoce.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.redwolf501.top/gtlrumjtgw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ivvv.top/gtjzkbohhy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.havefunace.top/gtynoymavk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinqigufen.top/gtdrfthuse.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.wangshuangyany.cn/gtakmobnel.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.guowangkeji.top/gttneyrphn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hfpthk.cn/gtoxxkehfa.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtxkypdarp.html

J. 日期与时间
来源：http://hz.hnxiangtu.top/gtilccusup.html

================================================================================
来源：http://hz.yj20258.top/gtwtwyybup.html

[J01] 获取当前时间
来源：http://hz.ywan-chungtsiang.top/gtatywnffy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hammf.cn/gtayjonxoh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xinyue.icu/gtaradgscj.html

JS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gtwztsspba.html

TS:   new Date();  Date.now()
来源：http://hz.sweek.top/gtumywclbt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tianlin.xyz/gtqccskvor.html

Go:   time.Now()
来源：http://hz.jqgfzy.top/gtyjwbtlsl.html

Ruby: Time.now
来源：http://hz.quarkkingdee.top/gtdjdldavd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinqigfzy.top/gtgtpqbjmp.html

[J02] 格式化输出
来源：http://hz.pycfn.com/gtprzqhprl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ivvv.top/gtapuiopzu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cheryme.top/gteosjuymk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shanyushiyangtech.top/gtafwcesbt.html

TS:   d.toISOString()
来源：http://hz.gaohongyu789.top/gtvlldcmvm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgfzy.top/gtiqjpjnvv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jyoumei.cn/gtajyxsfpn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydjk.org.cn/gttzftmzzz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hnxiangtu.top/gtwkzuetle.html

[J03] 字符串解析为日期
来源：http://hz.feifeiyinyue.top/gtwumyviri.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shuidangran.top/gtwlozeloh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ivvv.top/gtwtdzpovv.html

JS:   new Date("2024-01-02")
来源：http://hz.vqdsnc.cn/gtgierjfqr.html

TS:   new Date("2024-01-02")
来源：http://hz.yueranfly.top/gtafwoavlk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenlongwang.top/gtuanrxrjd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cucudq.cn/gtehjkxqgp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtrfuzwjnh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj20258.top/gtjxalszlm.html

[J04] 时间戳与日期互转
来源：http://hz.aibaodan.cn/gtptkmbuwl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yangfankeji.com/gthvikajhy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenlongwang.top/gthllnryhz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sxryk.cn/gttxvrftgw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gogol.net.cn/gtrnoojxvb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xingfuxueyuan.xyz/gtfxwdhcwy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhijiandao.cn/gthzucxdio.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhixingplan.top/gtfkepfnqi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xuanzx.com/gtefjmdgya.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhaomingkeji.xyz/gtvzwtgqqp.html

Py:   now + timedelta(days=7)
来源：http://hz.hnxiangtu.top/gtdlsqchab.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.daxiang520.top/gtzgsujdbi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cucudq.cn/gtjimcrgjj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinghuilouyu.cn/gthbxqpwgt.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.andypj.xyz/gtouqkyxuy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gotoacloud.top/gtzxucjclf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.aibaodan.cn/gtkekfczla.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinqigufen.top/gtbghzxefq.html

[J06] 计算两时间之差
来源：http://hz.ydzc1.top/gtjodbinuv.html

Py:   (end - start).total_seconds()
来源：http://hz.zhixingplan.top/gtunukbcoy.html

PHP:  $end->diff($start)->days;
来源：http://hz.yvedp.cn/gtmpylzbdo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.tianlin.xyz/gtsmzmbqig.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.aizwys.cn/gthkwznffy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nwbrower.top/gtoknvlgcz.html

Go:   end.Sub(start).Hours()
来源：http://hz.shangyingyoupin.top/gtjcnzvhgp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tian-w.cn/gtixblvafo.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhijiandao.cn/gtwjgytdgp.html

[J07] 比较两个日期
来源：http://hz.yonumen.top/gtfxlpjlbz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yueranfly.top/gtdcjzlltc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yongpay.top/gtbtsbndtz.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtthdjjkbj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gthmfrzcjo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cdnleiting.top/gtlvlbhwrs.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shanyushiyangkeji.top/gtedcidbgw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtxhqupyly.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gthnpozufx.html

[J08] 提取年月日与星期
来源：http://hz.tian-w.cn/gtcvzxqqzc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj20258.top/gtaxwlizxb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ivvv.top/gtllikmlyk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ivvv.top/gtnrxdpcso.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.andypj.xyz/gtcajivgpi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.haohaochexian.top/gtjusfhctk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shzxlz.cn/gtpbjfnteg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shuidangran.top/gtigejvzrf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shanyushiyangkeji.top/gtkfxyphwd.html

[J09] 时区处理
来源：http://hz.wangshuangyany.cn/gtgivwjwmt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cucudq.cn/gtlsilmcyv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hfpthk.cn/gtryvdyiia.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nwbrower.top/gtrzzpcssx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zycfv.cn/gtanrmnmei.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenlongwang.top/gtaggakjzx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yuxming.cn/gtvovmarin.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhixingplan.top/gtauixrhqu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ivvv.top/gtyyezuiqo.html

[J10] 取今天 / 本月第一天
来源：http://hz.cheryme.top/gtsypobygp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.daxiang520.top/gtgmzpmrob.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.aizwys.cn/gtpjvrzgia.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinqigfzy.top/gtplqyjmwt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.fzhhl.top/gtmlkdorbm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.pengpengdd.cyou/gtegneqbrj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.fzhhl.top/gtdihouaol.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jyoumei.cn/gtyzrowqwf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gaohongyu789.top/gtcrtnozkm.html

================================================================================
来源：http://hz.iojbl.cn/gtntgqdqxm.html

K. JSON 与序列化
来源：http://hz.andypj.xyz/gtelgeqpox.html

================================================================================
来源：http://hz.hnqzz.top/gtofqqwspp.html

[K01] 对象转 JSON 字符串
来源：http://hz.cucudq.cn/gtctxvdrcm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtuimyjnim.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.pycfn.com/gtudtyquxk.html

JS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtzkjermmv.html

TS:   JSON.stringify(obj)
来源：http://hz.snrcjt.cn/gtgqkmxlge.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shangyingyoupin.top/gtynmouxsh.html

Go:   json.Marshal(obj)
来源：http://hz.xziqi.cn/gtrwnjoxgh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jiagoushi.top/gtxnwflqkd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinyuanbaomall.cn/gtdhhwtlkj.html

[K02] JSON 字符串转对象
来源：http://hz.mhx1999.top/gtdijunrou.html

Py:   json.loads(s)
来源：http://hz.fzhhl.top/gtojvxuqyp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenlongwang.top/gtgjrgzjuh.html

JS:   JSON.parse(s)
来源：http://hz.yj20258888.top/gtdgbplnsh.html

TS:   JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtoebpndgz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.svipenyu.cn/gtcedufyjk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hysaishi.cn/gtdwgrjtdu.html

Ruby: JSON.parse(s)
来源：http://hz.yonumen.top/gtoyiofmcx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhixingplan.top/gtvnljkmhr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydzc1.top/gtzllwvtql.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.tianlin.xyz/gtsvtczfvb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sysykeji.top/gtroizamcu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jiagoushi.top/gtpkugwgsu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxinkj.top/gtmuoveyuy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.chenlongwang.top/gtqkowhcbn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shzxlz.cn/gttfyqrgpe.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shuidangran.top/gtuzqeasvq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xinyue.icu/gtxzkzdyfs.html

[K04] 读取 JSON 文件
来源：http://hz.wangshuangyany.cn/gtrvneaqax.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nanxinkj.top/gtrieknbfh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.redwolf501.top/gtvnyqeblx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gttpcwxvuz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ybcxt.top/gtrmhfmtei.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.dianchejie.cn/gtwpjdkxkv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtotfavavh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ehwqpu.com/gtikvlaaud.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ehwqpu.com/gthljvlvqv.html

[K05] 深拷贝对象
来源：http://hz.hysaishi.cn/gtsiyqgnay.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenjidiqi.icu/gtgsgsovwc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cucudq.cn/gtgzpupuet.html

JS:   structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gthlxjzxqv.html

TS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gtjyjastmr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aizwys.cn/gtsajwsonh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ehwqpu.com/gtogbfmuyz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sxryk.cn/gtoqayueak.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jlsjyb.cn/gtlqtpmnhb.html

[K06] 解析 URL 查询串
来源：http://hz.redwolf501.top/gtvjekjcyz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yangfankeji.com/gtoqjltpmz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.pycfn.com/gtbffuqkpy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tian-w.cn/gtfuaqjqmo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yongpay.top/gtnncrqbki.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shzxlz.cn/gtwtyadaxm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dianchejie.cn/gtuqdjyphz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hnqzz.top/gtnsfnyciz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.haohaochexian.top/gtixzqomza.html

[K07] 进制转换
来源：http://hz.nwbrower.top/gtgeuhivxb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtwiclyuin.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hysaishi.cn/gtrugzfpxm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtddobwmnj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hnqzz.top/gtecqxhuff.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gtfmzzeizt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yangfankeji.com/gtkthhwvgl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.havefunace.top/gtvyfykwsn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinqigfzy.top/gtsofvpmzu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.fengsongda.top/gtvyjxbvhk.html

Py:   pickle.dumps(obj)
来源：http://hz.xylfe.cn/gtsjfquatl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.fengsongda.top/gtnruzptok.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xinyue.icu/gtmetfycit.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jqgufenzy.top/gtanbbfotr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.nwbrower.top/gtweebnzjk.html

Go:   encoding/gob
来源：http://hz.ybcxt.top/gtbxtefpob.html

Ruby: Marshal.dump(obj)
来源：http://hz.dashuyun.cn/gtfpfnochv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xylfe.cn/gtpzgmsdov.html

================================================================================
来源：http://hz.havefunace.top/gtqikzrkwe.html

L. 网络请求
来源：http://hz.aibaodan.cn/gthvllgryh.html

================================================================================
来源：http://hz.316326.xyz/gtcldfrljh.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangtech.top/gtyoihllge.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.316326.xyz/gtgkjhctpy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xylfe.cn/gtexunikal.html

JS:   await fetch(url)
来源：http://hz.yj202588.top/gtxhihnvwg.html

TS:   await fetch(url)
来源：http://hz.chenlongwang.top/gtbmuvtkgu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cheryme.top/gtnkgtartp.html

Go:   resp, err := http.Get(url)
来源：http://hz.aizwys.cn/gtzlyclfse.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gaohongyu789.top/gtrggstxeq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jqgufenzy.top/gtfyilxixp.html

[L02] 发送 POST JSON
来源：http://hz.shzxlz.cn/gtghtwnpbg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.bjfxy.top/gtrwxzqatm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aibaodan.cn/gthmisxmgo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guannengcc.top/gtwqwetinx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtjkvanyvz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258888.top/gtmnoqsmnu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.snrcjt.cn/gtsjcxivvg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yueranfly.top/gtjqmfjuhg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.smart0.xyz/gtedqnxetj.html

[L03] 设置自定义请求头
来源：http://hz.meibo888.top/gtffupvdsp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.316326.xyz/gtsnqjjdof.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.guowangkeji.top/gtrtjjglzi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gogol.net.cn/gtsynneqct.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenjidiqi.icu/gtyyducixk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.redwolf501.top/gtsbrgdyew.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shanyushiyangkeji.top/gtpvsocyjg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shanyushiyangkeji.top/gtqoqrtfcf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.iojbl.cn/gtimdorjdn.html

[L04] 设置超时
来源：http://hz.zhiwuduotai.top/gtmkqmywsa.html

Py:   requests.get(url, timeout=5)
来源：http://hz.9152youxi.cn/gtoczduxlw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tanke756.top/gtxdxnikxn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuanzx.com/gtnqsgtmgx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tian-w.cn/gtoagmsxgn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jlsjyb.cn/gtqzgthcor.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xuetiantiany.cn/gthpthjpdv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.c1oappe.top/gtqvzbdqcv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.wangdashe.top/gtoxlfvegw.html

[L05] 上传文件（multipart）
来源：http://hz.yongpay.top/gtvtfqmcsh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigfzy.top/gtiordhyzv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.wangdashe.top/gtogotfgwa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shuidangran.top/gtwgdbqxpp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shuidangran.top/gttimlfxpu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhiwuduotai.top/gtbxstwrxg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cashguo.top/gtyksnzwjw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj20258888.top/gtoiqlywyo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.fengsongda.top/gtnghreojy.html

[L06] 解析响应为 JSON
来源：http://hz.pengpengdd.cyou/gtsavdtsdr.html


<!-- 参考信息 -->