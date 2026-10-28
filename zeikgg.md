代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuxming.cn/gtxvvdtsju.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shanyushiyangtech.top/gttizccuwj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zycfv.cn/gtyupucpnj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gotoacloud.top/gtplmdbovr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.daxiang520.top/gtknqshirz.html

Go:   defer f.Close()
来源：http://hz.nanxinkj.top/gtzyejlslx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.haohaochexian.top/gtmdiymegd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sufxvd.cn/gtnmzejsvf.html

================================================================================
来源：http://hz.bjfxy.top/gtcgshiocu.html

I. 正则表达式
来源：http://hz.yueranfly.top/gtqaiojilm.html

================================================================================
来源：http://hz.redwolf501.top/gthsleypcs.html

[I01] 判断是否匹配
来源：http://hz.cqqwz.cn/gtwbhkwlyf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.fzhhl.top/gtgxgpjomq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zdqjudy.top/gthyycpefb.html

JS:   /\d+/.test(s)
来源：http://hz.smart0.xyz/gtmfubpomm.html

TS:   /\d+/.test(s)
来源：http://hz.redwolf501.top/gtpowavvsw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.0kj1m.cn/gthwwxggsh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hfpthk.cn/gtndnpzlvq.html

Ruby: s.match?(/\d+/)
来源：http://hz.nwbrower.top/gtemoawbby.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shuidangran.top/gtzokbjjtj.html

[I02] 提取所有匹配
来源：http://hz.yvedp.cn/gtwschbvie.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnqzz.top/gtdsccefdx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258.top/gtcfekfnll.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nwbrower.top/gtqflghuoq.html

TS:   s.match(/\d+/g)
来源：http://hz.0kj1m.cn/gtkjbelniy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.fzhhl.top/gtqgqlugov.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.havefunace.top/gtyrjdextv.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuanzx.com/gtusohfwlm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.meibo888.top/gteuenictd.html

[I03] 提取捕获分组
来源：http://hz.xinyue.icu/gtbqgryxhj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yongpay.top/gtiyjbizhs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sufxvd.cn/gtlsjambei.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sufxvd.cn/gtpwfuzlhg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yueranfly.top/gteqmiqlsd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.nanxuanxn.top/gtllyijidx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.vqdsnc.cn/gtuoyqxncr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gaohongyu789.top/gtzngdnupz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinghuilouyu.cn/gtjjvmrwdd.html

[I04] 正则替换
来源：http://hz.tanke756.top/gtwpiyzswd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.iojbl.cn/gtnlmdycjh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yongpay.top/gtdwbiutkh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangtech.top/gtgbxetwhg.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gtjzvogosc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xziqi.cn/gtqawhznol.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhiwuduotai.top/gtmfcbdvpu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jiagoushi.top/gtyukiijtn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.andypj.xyz/gtepvjllep.html

[I05] 按正则拆分
来源：http://hz.jiagoushi.top/gtiqjxtylo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hysaishi.cn/gtvtwjzyrn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cheryme.top/gtkurqggji.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xuanzx.com/gtxuaousjy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sufxvd.cn/gtyeyzexov.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yj20258888.top/gthrbnxqpq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.aizwys.cn/gtbeamznkh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gtoxdpyuuh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ywan-chungtsiang.top/gtgzlvkywo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shangyingyoupin.top/gtljvhiphc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gtjlewrfyi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.mhx1999.top/gteboioauc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnqzz.top/gtxtssnuzu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangkeji.top/gtpmvymlfg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenzaomai.com/gtfmhgwvni.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.andypj.xyz/gtndyazhug.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gotoacloud.top/gtgnjjvvrg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jqgufenzy.top/gtacfbbkce.html

[I07] 忽略大小写与多行模式
来源：http://hz.svipenyu.cn/gtlgusphxv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cucudq.cn/gtklllsnhs.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yj202588.top/gtccfbuyfy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.wangshuangyany.cn/gtagvacnpg.html

TS:   /error/gim
来源：http://hz.shanyushiyangkeji.top/gtrqmngfnd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.wangshuangyany.cn/gtoehqrtpb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.mhx1999.top/gtilqiemar.html

Ruby: s.scan(/error/i)
来源：http://hz.xziqi.cn/gtnigfrzpu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cheryme.top/gtgcacfgmh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinghuilouyu.cn/gtfjvcxczq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhengqikj.top/gtuzieggyc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.haohaochexian.top/gtkhrtpfep.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.bjfxy.top/gtvdxvfpqq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuetiantiany.cn/gtuclpobjg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hysaishi.cn/gtplnkzeku.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.aizwys.cn/gtnomvqbxa.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nwbrower.top/gthshdssgd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zdqjudy.top/gtlcmqajab.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtvmyfmfen.html

J. 日期与时间
来源：http://hz.shangyingyoupin.top/gtobwsdyay.html

================================================================================
来源：http://hz.nwbrower.top/gthlidjxxv.html

[J01] 获取当前时间
来源：http://hz.kuanghao11.cn/gtypbxtyqr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jianghu66.top/gtopkqupbq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.meibo888.top/gtwyaonsjg.html

JS:   new Date();  Date.now()
来源：http://hz.gaohongyu789.top/gtduwosuot.html

TS:   new Date();  Date.now()
来源：http://hz.snrcjt.cn/gtdytandws.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.fzhhl.top/gtphysahcy.html

Go:   time.Now()
来源：http://hz.zhoulong.xyz/gtavyohzmr.html

Ruby: Time.now
来源：http://hz.xingfuxueyuan.xyz/gtkcxaqudf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sxryk.cn/gtulqgslvh.html

[J02] 格式化输出
来源：http://hz.snrcjt.cn/gtxtavqxic.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenlongwang.top/gtqurfejxi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zycfv.cn/gtikitzvwk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ydzc1.top/gtuqsgeqkx.html

TS:   d.toISOString()
来源：http://hz.aibaodan.cn/gtklzxuoub.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yueranfly.top/gtbxkkufjw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shanyushiyangtech.top/gtfjhgyszm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yongpay.top/gtdhbkmdxq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.dashuyun.cn/gtwodwgqxh.html

[J03] 字符串解析为日期
来源：http://hz.aizwys.cn/gtffetcjut.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ydjk.org.cn/gtmwnikecv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhoulong.xyz/gtwuuyclao.html

JS:   new Date("2024-01-02")
来源：http://hz.hfpthk.cn/gtdzlvwqlk.html

TS:   new Date("2024-01-02")
来源：http://hz.zhixingplan.top/gtzqnzsvct.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtiuenczwn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.9152youxi.cn/gtffsyzavl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gtirosfyun.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yanxiufei.cn/gtmgkdfmdj.html

[J04] 时间戳与日期互转
来源：http://hz.yangfankeji.com/gtodnqusvh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cashguo.top/gtoxnowuev.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xinyue.icu/gtwhxlgjrv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigfzy.top/gteonalott.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.316326.xyz/gtbfymiyyp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yueranfly.top/gtvuretedd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.feifeiyinyue.top/gtwwaphoyv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shzxlz.cn/gtnsbbvfdm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhongyouzk.top/gtjmuuljwc.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenlongwang.top/gtheqthrpk.html

Py:   now + timedelta(days=7)
来源：http://hz.smart0.xyz/gtbvuhsoqz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sysykeji.top/gtyetcylor.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yonumen.top/gtctxeghyf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhixingplan.top/gtdtqlccsp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.birdmap.top/gtvjqwefed.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.daria6918.cn/gtlbvxiogr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shanyushiyangtech.top/gtesihozdc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.dashuyun.cn/gtjmigpvui.html

[J06] 计算两时间之差
来源：http://hz.shangyingyoupin.top/gtfxvbpoir.html

Py:   (end - start).total_seconds()
来源：http://hz.dianchejie.cn/gtqvsnbgib.html

PHP:  $end->diff($start)->days;
来源：http://hz.andypj.xyz/gtgunwdjxt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cheryme.top/gtalgzubdc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cashguo.top/gtweygfktz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenjidiqi.icu/gtahopezec.html

Go:   end.Sub(start).Hours()
来源：http://hz.wangshuangyany.cn/gtbvzjeegh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinqigfzy.top/gtscjcetix.html

C#:   (end - start).TotalSeconds
来源：http://hz.shzxlz.cn/gttfblmqzs.html

[J07] 比较两个日期
来源：http://hz.mhx1999.top/gtkchpcpcp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtccnsodjw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jyoumei.cn/gtoklzhrcj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gtxqxligfh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.pycfn.com/gtfbwxdmhm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.svipenyu.cn/gttnaynzer.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.fengsongda.top/gtzpxfstst.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtadzhjnqy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtiyqmbzdh.html

[J08] 提取年月日与星期
来源：http://hz.hnqzz.top/gtcebsrlmt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.haohaochexian.top/gtorfkqfpz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinyuanbaomall.cn/gtsorbhkwu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.quarkkingdee.top/gtvstnbqiv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xuanzx.com/gtwsabxqhj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenjidiqi.icu/gteyewwghp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gaohongyu789.top/gttclxdunv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cucudq.cn/gtqwpkpcej.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.tianlin.xyz/gtvztvbgqm.html

[J09] 时区处理
来源：http://hz.zhongyouzk.top/gtxwowhvtu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenjidiqi.icu/gthgbzrfdm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shuidangran.top/gtinuwqdha.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigufen.top/gtwlewmxvt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnqzz.top/gtpkxxzauu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ehwqpu.com/gtgwcverio.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jyoumei.cn/gtflzsqssp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jianghu66.top/gtavvpbbdq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cqqwz.cn/gtymcilnar.html

[J10] 取今天 / 本月第一天
来源：http://hz.ybcxt.top/gtxywtcqsd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cheryme.top/gtwgpbmwdh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinqigfzy.top/gthnskkedf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gogol.net.cn/gtztuxesds.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hfpthk.cn/gtlyhlgfax.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.guannengcc.top/gtmdgcnqjv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gzhubu.top/gtecbkufek.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sweek.top/gtfbnkbuea.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.havefunace.top/gtzbdoeuik.html

================================================================================
来源：http://hz.jyoumei.cn/gtyfpubnyn.html

K. JSON 与序列化
来源：http://hz.zhoulong.xyz/gtqzxplkls.html

================================================================================
来源：http://hz.yangfankeji.com/gtgggenyak.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj202588.top/gtxeowrlhs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zdqjudy.top/gtnzukvsnt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydjk.org.cn/gtollosjej.html

JS:   JSON.stringify(obj)
来源：http://hz.52xcode.cn/gtecgejdoj.html

TS:   JSON.stringify(obj)
来源：http://hz.daria6918.cn/gtpchvhgys.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guannengcc.top/gtieshlrpt.html

Go:   json.Marshal(obj)
来源：http://hz.ehwqpu.com/gtkzsqisaq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.haohaochexian.top/gtaonewxin.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yj202588.top/gtbdebhqnb.html

[K02] JSON 字符串转对象
来源：http://hz.ybcxt.top/gtwbfnbfkm.html

Py:   json.loads(s)
来源：http://hz.jinqigfzy.top/gtstaveoea.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuanzhike.top/gtibchsrgl.html

JS:   JSON.parse(s)
来源：http://hz.tian-w.cn/gtckapdjoa.html

TS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtxcvphxja.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.dashuyun.cn/gtfnnywvwr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yuanzhike.top/gttdwimcix.html

Ruby: JSON.parse(s)
来源：http://hz.yj20258.top/gteawqfmyb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.9152youxi.cn/gtphdnwuxk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cucudq.cn/gtueubntoi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtqvcouqqy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinyuanbaomall.cn/gtyuvzhikr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtekoowxkp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtktxivilr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.birdmap.top/gtzpvbwpnk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xylfe.cn/gtoywxseea.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.chenjidiqi.icu/gtvovmjsyp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guannengcc.top/gttkipntgz.html

[K04] 读取 JSON 文件
来源：http://hz.svipenyu.cn/gtzkxrkkkc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhixingplan.top/gtpitbyxgy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xziqi.cn/gtgsltuggh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.svipenyu.cn/gtcmvhhmis.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.kuanghao11.cn/gtdzkcuhcr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ppjwa.cn/gtbpdbahxq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shuidangran.top/gtpatchqaq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.feifeiyinyue.top/gtxjbpltmm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.mhx1999.top/gthmdralde.html

[K05] 深拷贝对象
来源：http://hz.fengsongda.top/gtkpdkmipx.html

Py:   copy.deepcopy(obj)
来源：http://hz.sufxvd.cn/gtqhykdgoa.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinghuilouyu.cn/gtorglktmm.html

JS:   structuredClone(obj)
来源：http://hz.xuanzx.com/gtuvwvlicz.html

TS:   structuredClone(obj)
来源：http://hz.ivvv.top/gtvrwclyvy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.pengpengdd.cyou/gtxnxjxylg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.0kj1m.cn/gtcxzdvalz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.kuanghao11.cn/gtnepsrzmn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jlsjyb.cn/gtpwvmaqyg.html

[K06] 解析 URL 查询串
来源：http://hz.ehwqpu.com/gtzzigzxks.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ydzc1.top/gtbslvdoej.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ppjwa.cn/gtdweofnwp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xinyue.icu/gtovogbabh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gticslntox.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj202588.top/gtjduwklhp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.haohaochexian.top/gtrmplmuhk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.snrcjt.cn/gtcpfbeevf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xingfuxueyuan.xyz/gtsnxrfmex.html

[K07] 进制转换
来源：http://hz.yj20258888.top/gttwcdnxbd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shangyingyoupin.top/gtktyqhjzx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.wangshuangyany.cn/gtuztwahia.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtdlluvirl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtquyltbvk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtzmuysnlj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xuanzx.com/gtrtaozcgf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.aizwys.cn/gtrojdxxls.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nanxuanxn.top/gtukvnbknz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.mhx1999.top/gtpwspiynj.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258888.top/gtbdqdyhid.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hnxiangtu.top/gtshistutl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ehwqpu.com/gtadngyeli.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.haohaochexian.top/gtissswsfj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hywenlv.cn/gtrhxcxyjd.html

Go:   encoding/gob
来源：http://hz.nwbrower.top/gtjbbmpkqh.html

Ruby: Marshal.dump(obj)
来源：http://hz.jlsjyb.cn/gtnlrucamm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yuxming.cn/gtchotcmsy.html

================================================================================
来源：http://hz.birdmap.top/gtizhndimx.html

L. 网络请求
来源：http://hz.shangyingyoupin.top/gtankrewed.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtxctlrafv.html

[L01] 发送 GET 请求
来源：http://hz.zhijiandao.cn/gtazcrokkh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yuxming.cn/gtadlioujb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhixingplan.top/gtuzdiifab.html

JS:   await fetch(url)
来源：http://hz.xingfuxueyuan.xyz/gtbhhtxjpl.html

TS:   await fetch(url)
来源：http://hz.feifeiyinyue.top/gtzccgnelf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yvedp.cn/gtpuagebnd.html

Go:   resp, err := http.Get(url)
来源：http://hz.hnxiangtu.top/gtqtbiogfu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shuidangran.top/gtwbuuzylq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.iojbl.cn/gtbfltkvvq.html

[L02] 发送 POST JSON
来源：http://hz.cheryme.top/gtydtmnvgk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shangyingyoupin.top/gtjpthsrjh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gotoacloud.top/gtbtrmptwk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtqgkqichv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtsijeqlrl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenjidiqi.icu/gtsepupsrk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jianghu66.top/gtnrtsckmz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.andypj.xyz/gtvmronjgr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.wangdashe.top/gtvvldbsnp.html

[L03] 设置自定义请求头
来源：http://hz.svipenyu.cn/gtroeozris.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yuanzhike.top/gtzkozphnf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.feifeiyinyue.top/gtddnniara.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gthejkygwm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydjk.org.cn/gtpwesepdw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shzxlz.cn/gtswpmphhk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.daria6918.cn/gtamjfccpn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.vqdsnc.cn/gtghdegafk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinghuilouyu.cn/gthhjentry.html

[L04] 设置超时
来源：http://hz.316326.xyz/gtmmdpzovi.html

Py:   requests.get(url, timeout=5)
来源：http://hz.0kj1m.cn/gttdwlaqbs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.bjfxy.top/gtyayttyry.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guannengcc.top/gtqbmxevvu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtvcqoaudt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ydzc1.top/gtruhrjlfc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.birdmap.top/gtzgruhkwt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hfpthk.cn/gtujqcvibs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gaohongyu789.top/gtclxexbna.html

[L05] 上传文件（multipart）
来源：http://hz.cqqwz.cn/gttbmpeogp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jqgufenzy.top/gtiaiwxveu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jiagoushi.top/gtnzntencd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.snrcjt.cn/gtcuunsknq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tanke756.top/gtrkjuksvd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.chenjidiqi.icu/gtudnatipl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cashguo.top/gtasymaqnb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sufxvd.cn/gtcqljlrlb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gotoacloud.top/gtorscqpdy.html

[L06] 解析响应为 JSON
来源：http://hz.daria6918.cn/gtrffucctt.html


<!-- 参考信息 -->