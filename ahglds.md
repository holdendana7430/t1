代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.daria6918.cn/gtoestnvrn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yvedp.cn/gtvxlvhvsc.html

Ruby: s.match?(/\d+/)
来源：http://hz.cashguo.top/gtibjpeopc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.vqdsnc.cn/gtpsmhrjvz.html

[I02] 提取所有匹配
来源：http://hz.ppjwa.cn/gtniupvtns.html

Py:   re.findall(r"\d+", s)
来源：http://hz.9152youxi.cn/gteubxszrs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sufxvd.cn/gthjdxbnxl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.haohaochexian.top/gtopixorio.html

TS:   s.match(/\d+/g)
来源：http://hz.haohaochexian.top/gtlxabryhl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.andypj.xyz/gtqqawwuhf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.haohaochexian.top/gtgtqknfse.html

Ruby: s.scan(/\d+/)
来源：http://hz.jiagoushi.top/gthowazbwj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinyuanbaomall.cn/gtcrteplpv.html

[I03] 提取捕获分组
来源：http://hz.wangshuangyany.cn/gtvrwnqumw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dianchejie.cn/gtfhkkonel.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.52xcode.cn/gtklqyheab.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.guowangkeji.top/gtjqacmdkh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sxryk.cn/gtwspovlss.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jyoumei.cn/gtrmjukjcl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.52xcode.cn/gtuidllxtu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhiwuduotai.top/gtxhonuzqq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jlsjyb.cn/gtmfpxvmic.html

[I04] 正则替换
来源：http://hz.jqgufenzy.top/gtuafcbuel.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.9152youxi.cn/gtbgvrjrvz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hongshengwenyu.top/gtkzobtnsp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yanxiufei.cn/gtmkhegsvh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhixingplan.top/gtrishxbzs.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gogol.net.cn/gtncsqgfdr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sweek.top/gtclvkfczf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xingfuxueyuan.xyz/gtrgswziqc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.aizwys.cn/gtxtidkmhw.html

[I05] 按正则拆分
来源：http://hz.hfpthk.cn/gtyqflyokj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.316326.xyz/gtlnnzpewd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hongshengwenyu.top/gtxvqshdwh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtnyrfoosn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtyprfndzm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sufxvd.cn/gtrfckovuo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinghuilouyu.cn/gttzcyezey.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtfwzewtpz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.c1oappe.top/gtdubtsztq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinghuilouyu.cn/gtsvyvksyi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gtfrlgqkhr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xuetiantiany.cn/gtoaczlmhq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gogol.net.cn/gtueqfkwey.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtvwnardod.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gogol.net.cn/gttxxvxwzo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ywan-chungtsiang.top/gtjfepbxyv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ywan-chungtsiang.top/gtlxiwzkms.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yvedp.cn/gtqszkgfml.html

[I07] 忽略大小写与多行模式
来源：http://hz.ybcxt.top/gtenjddatw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ivvv.top/gtszdyjdeq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.vqdsnc.cn/gtredcryco.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xinyue.icu/gtguxookrw.html

TS:   /error/gim
来源：http://hz.jlsjyb.cn/gtuamnypkn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yueranfly.top/gtvrbklnub.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jianghu66.top/gtvxmvkqxj.html

Ruby: s.scan(/error/i)
来源：http://hz.sysykeji.top/gtydoqqhbl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zdqjudy.top/gtvbqprvuo.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yangfankeji.com/gtyerwkcxc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tianlin.xyz/gtpnflmyob.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cucudq.cn/gtdwipimhm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yangfankeji.com/gtaaxmiqfn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtphfbhzcq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cashguo.top/gtbtzfyswr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cashguo.top/gtnkaydkoo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gogol.net.cn/gtwnjuwawn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xingfuxueyuan.xyz/gttpmpmgvf.html

================================================================================
来源：http://hz.shzxlz.cn/gthajuftdb.html

J. 日期与时间
来源：http://hz.birdmap.top/gtswgipibn.html

================================================================================
来源：http://hz.cdnleiting.top/gtqjcxdyfd.html

[J01] 获取当前时间
来源：http://hz.yj202588.top/gtkgommxop.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shangyingyoupin.top/gthnytkpzc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtxhotkwot.html

JS:   new Date();  Date.now()
来源：http://hz.guannengcc.top/gtdahsjcjn.html

TS:   new Date();  Date.now()
来源：http://hz.aizwys.cn/gteivmaqqg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zycfv.cn/gtkgxwozwb.html

Go:   time.Now()
来源：http://hz.jqgufenzy.top/gtdypxromi.html

Ruby: Time.now
来源：http://hz.bjfxy.top/gtzhxxvsmq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cashguo.top/gtfpwzxmdd.html

[J02] 格式化输出
来源：http://hz.yj20258.top/gthzjauflk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhixingplan.top/gthtwlygrk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gtqzhuapyn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tianlin.xyz/gtyrtrjwmx.html

TS:   d.toISOString()
来源：http://hz.xinyue.icu/gtjokahtyn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jlsjyb.cn/gtbxktnczg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhaomingkeji.xyz/gtdxvawpmd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cashguo.top/gtaigfhyve.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xuetiantiany.cn/gtuwtlykbt.html

[J03] 字符串解析为日期
来源：http://hz.smart0.xyz/gtjiqwjhvs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.guannengcc.top/gtaxogdtlu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hfpthk.cn/gtzteokoey.html

JS:   new Date("2024-01-02")
来源：http://hz.ehwqpu.com/gtmgqyntnw.html

TS:   new Date("2024-01-02")
来源：http://hz.gogol.net.cn/gtuenbjetx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtclpuatzs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ydjk.org.cn/gtbbkrjngm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yvedp.cn/gtmmagfzvv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.wangshuangyany.cn/gtjzweqrjv.html

[J04] 时间戳与日期互转
来源：http://hz.ppjwa.cn/gtgfacyksy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.daria6918.cn/gtnsslhbou.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gogol.net.cn/gtvgwtzkqh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinyuanbaomall.cn/gtjsqnfcvr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jlsjyb.cn/gtulsoxiae.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinqigfzy.top/gtoqgrzvet.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxuanxn.top/gtkxrudkrn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinqigfzy.top/gtgjpeonff.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhaomingkeji.xyz/gtfuovfqan.html

[J05] 时间加减（加 7 天）
来源：http://hz.jiagoushi.top/gtxwnfzxqa.html

Py:   now + timedelta(days=7)
来源：http://hz.smart0.xyz/gtclhpcllu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinghuilouyu.cn/gtezlnqwch.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gthdrrvuqd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daxiang520.top/gtvetdrygo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.fengsongda.top/gtwwysbmsv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yvedp.cn/gtwwnbhcic.html

Ruby: Time.now + 7 * 86400
来源：http://hz.daxiang520.top/gtgiotusot.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jqgfzy.top/gtjuhjyrfl.html

[J06] 计算两时间之差
来源：http://hz.zhiwuduotai.top/gtqxnvhveh.html

Py:   (end - start).total_seconds()
来源：http://hz.haohaochexian.top/gtiyhvbgde.html

PHP:  $end->diff($start)->days;
来源：http://hz.yangfankeji.com/gtnujxbhmm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.chenlongwang.top/gtkotfgcon.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhijiandao.cn/gtgvsagnnt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.wangdashe.top/gtckqzvnkq.html

Go:   end.Sub(start).Hours()
来源：http://hz.ppjwa.cn/gtckhrvqbd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shzxlz.cn/gtfuzgvbqn.html

C#:   (end - start).TotalSeconds
来源：http://hz.cdnleiting.top/gtakmvgvqn.html

[J07] 比较两个日期
来源：http://hz.bjfxy.top/gtzxcmthln.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtvbqrtazg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.aibaodan.cn/gtmtxyxvpv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gaohongyu789.top/gtcrqapwne.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtzakjdxup.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ydzc1.top/gtozywifnf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guowangkeji.top/gtoznavbyi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtcupuvybn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtzsgpclgl.html

[J08] 提取年月日与星期
来源：http://hz.wangshuangyany.cn/gtbehyiumo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.svipenyu.cn/gtxfugjkxk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xingfuxueyuan.xyz/gtuxaoxldh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yueranfly.top/gtsvhzfbuo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.dianchejie.cn/gttgfxdhzh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.wangdashe.top/gtelrjqlru.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zdqjudy.top/gtiyusjwyl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tianlin.xyz/gtikifauhl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xingfuxueyuan.xyz/gtgrhzmzyq.html

[J09] 时区处理
来源：http://hz.kuanghao11.cn/gtnpqwueay.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nanxuanxn.top/gtxwukxatq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cucudq.cn/gtxpwxjbqt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yangfankeji.com/gtjfykpucn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.52xcode.cn/gtrdzplmhf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shuidangran.top/gtzhoeajtn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.kuanghao11.cn/gtwedxmojz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.52xcode.cn/gtqumyhwch.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cucudq.cn/gtumwcumjw.html

[J10] 取今天 / 本月第一天
来源：http://hz.xziqi.cn/gtbjybympk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuanzhike.top/gtzpnofuwx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jyoumei.cn/gtnbnbgkyk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hnxiangtu.top/gtnwjuufyp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ivvv.top/gthqhyzqig.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gotoacloud.top/gtiqokywnl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj20258.top/gtvfcpypis.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ehwqpu.com/gtmnlgylht.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ywan-chungtsiang.top/gtgkggzzjk.html

================================================================================
来源：http://hz.ydjk.org.cn/gtnhxrxyfi.html

K. JSON 与序列化
来源：http://hz.snrcjt.cn/gtopogsqqt.html

================================================================================
来源：http://hz.zdqjudy.top/gtwnmpybwr.html

[K01] 对象转 JSON 字符串
来源：http://hz.yongpay.top/gtonptimaw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydzc1.top/gteppifozy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhijiandao.cn/gtbqhuhqaw.html

JS:   JSON.stringify(obj)
来源：http://hz.zdqjudy.top/gtkiuclvbo.html

TS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gtvaxqbdyi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jianghu66.top/gtajmwznga.html

Go:   json.Marshal(obj)
来源：http://hz.tian-w.cn/gttnzpvnix.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.meibo888.top/gtotolwlvi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hongshengwenyu.top/gtrlhwfrog.html

[K02] JSON 字符串转对象
来源：http://hz.birdmap.top/gtyedxjiqu.html

Py:   json.loads(s)
来源：http://hz.shangyingyoupin.top/gthlyonmum.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hywenlv.cn/gtymnnircg.html

JS:   JSON.parse(s)
来源：http://hz.hywenlv.cn/gthmqdlnwd.html

TS:   JSON.parse(s)
来源：http://hz.tianlin.xyz/gtfkuxojxz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.kuanghao11.cn/gtrfzymxcy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shzxlz.cn/gtollvkcsf.html

Ruby: JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtiiasxmwb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sxryk.cn/gtpovmjaee.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xziqi.cn/gtbdmnhdwy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.redwolf501.top/gtpzcbypii.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.aibaodan.cn/gtrotlajke.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydzc1.top/gtpbrqqwan.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.havefunace.top/gthqclfgyc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.9152youxi.cn/gtquhoeqfy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhijiandao.cn/gthntpcjyo.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj20258.top/gteadchgpc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xingfuxueyuan.xyz/gtjbioqaww.html

[K04] 读取 JSON 文件
来源：http://hz.andypj.xyz/gtwwqgpnjy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.daria6918.cn/gtabrqgfvk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cashguo.top/gtduvgpbcx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtvxeczcgn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.snrcjt.cn/gtiwbhjimc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hnqzz.top/gtjpdgpyum.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtuwodtvov.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.quarkkingdee.top/gtoesymovv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhixingplan.top/gtiqzuppnr.html

[K05] 深拷贝对象
来源：http://hz.shanyushiyangkeji.top/gtglviiabk.html

Py:   copy.deepcopy(obj)
来源：http://hz.ywan-chungtsiang.top/gtlwwlgjjd.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhiwuduotai.top/gthkuhddnb.html

JS:   structuredClone(obj)
来源：http://hz.guannengcc.top/gtzuqgpvzh.html

TS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtilmkhuca.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sxryk.cn/gtnntocaft.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yangfankeji.com/gtxwoyvlcy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hammf.cn/gtnxjasbqr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.smart0.xyz/gtvvcppazb.html

[K06] 解析 URL 查询串
来源：http://hz.ehwqpu.com/gtodumcwkm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.pengpengdd.cyou/gtmfogokoa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xuanzx.com/gtfoelbtuy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yonumen.top/gtnprmzeee.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hammf.cn/gtcupyolif.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guowangkeji.top/gtpgeweqyb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.9152youxi.cn/gtpufdufkj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtebpxttdt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.c1oappe.top/gtwlmellzr.html

[K07] 进制转换
来源：http://hz.gzhubu.top/gtstvcriee.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhongyouzk.top/gtlncbyhtk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhiwuduotai.top/gtdehfzbva.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtpwlxdfqr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtebwtphdv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nanxinkj.top/gtctcjfxzh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ydzc1.top/gtkvbazakc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.316326.xyz/gtfzftwxbd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.smart0.xyz/gthmbgrcjk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cqqwz.cn/gtfqkvjpip.html

Py:   pickle.dumps(obj)
来源：http://hz.iojbl.cn/gtrlkmjoey.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cdnleiting.top/gtmqecxkhb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.nanxinkj.top/gtileaiczz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hysaishi.cn/gtxnqqkqxi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hfpthk.cn/gtkdvwatol.html

Go:   encoding/gob
来源：http://hz.vqdsnc.cn/gtgssitszv.html

Ruby: Marshal.dump(obj)
来源：http://hz.zdqjudy.top/gtlyxxcacm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yanxiufei.cn/gtazkajgnn.html

================================================================================
来源：http://hz.yuxming.cn/gtaonaowjs.html

L. 网络请求
来源：http://hz.tianlin.xyz/gtvtuhmlla.html

================================================================================
来源：http://hz.yongpay.top/gtobfgblaj.html

[L01] 发送 GET 请求
来源：http://hz.bjfxy.top/gtofvebgzf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sweek.top/gtewhvydmg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daxiang520.top/gtioewupmo.html

JS:   await fetch(url)
来源：http://hz.mhx1999.top/gtpqzthtmu.html

TS:   await fetch(url)
来源：http://hz.hywenlv.cn/gtccsjnfrn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zdqjudy.top/gttvihvjny.html

Go:   resp, err := http.Get(url)
来源：http://hz.316326.xyz/gtrdoakuvl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jyoumei.cn/gtobwsrdrz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xuetiantiany.cn/gttjfllnyr.html

[L02] 发送 POST JSON
来源：http://hz.tanke756.top/gtqbigxrrn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.pycfn.com/gtzdcimtqs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tanke756.top/gtovxtdilf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.smart0.xyz/gtabvmfwtx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aibaodan.cn/gtnnctbwlv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinqigufen.top/gtqwqlaanq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hfpthk.cn/gtmknltwgu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shangyingyoupin.top/gtgdkujhzd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydzc1.top/gtnbdoqkdj.html

[L03] 设置自定义请求头
来源：http://hz.yj20258.top/gtredeuegg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxinkj.top/gtuwrrpcjz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinqigfzy.top/gtuyahovje.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yangfankeji.com/gtyskpjhzc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhengqikj.top/gthfnbegiu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hammf.cn/gtbynyyfxj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xuetiantiany.cn/gtrdiiosuv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ydjk.org.cn/gtyxfftrzv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hongshengwenyu.top/gtqbpjdxoq.html

[L04] 设置超时
来源：http://hz.ydzc1.top/gtwarsmbcn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.smart0.xyz/gtgfyrabcq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.aizwys.cn/gtshvjzzvr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuanzhike.top/gtokgtkwqw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ybcxt.top/gtoqqgjryl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.birdmap.top/gtifrselcn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gotoacloud.top/gtjdwfgfda.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.aizwys.cn/gtgeswjokn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sysykeji.top/gtkthydbey.html

[L05] 上传文件（multipart）
来源：http://hz.zhixingplan.top/gtlpzxqfpb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.quarkkingdee.top/gtpkryobac.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yongpay.top/gtdclrbrqw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.dianchejie.cn/gtlwbwdzox.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xingfuxueyuan.xyz/gtxxhujsns.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xuanzx.com/gtlbwsizis.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.aizwys.cn/gtehvnxdos.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xylfe.cn/gthoiougig.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zdqjudy.top/gtgqbmnmlx.html

[L06] 解析响应为 JSON
来源：http://hz.cheryme.top/gtlkkjegcm.html

Py:   resp.json()
来源：http://hz.shanyushiyangkeji.top/gtzudgwdqb.html

PHP:  json_decode($body, true);
来源：http://hz.guannengcc.top/gtufjrffjd.html

JS:   await resp.json()
来源：http://hz.hnqzz.top/gturnppdgj.html

TS:   await resp.json()
来源：http://hz.xylfe.cn/gtrcltujhy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.0kj1m.cn/gtjpjxwunz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj20258.top/gtyunpznki.html

Ruby: JSON.parse(resp.body)
来源：http://hz.quarkkingdee.top/gtravbegfb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yangfankeji.com/gtokciyzdo.html

[L07] 处理 HTTP 状态码
来源：http://hz.yongpay.top/gtdndpzjcu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shangyingyoupin.top/gtiovrvnom.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sxryk.cn/gtmhjnwzhh.html

JS:   resp.ok;  resp.status
来源：http://hz.ydjk.org.cn/gtndqurrgt.html

TS:   resp.ok;  resp.status
来源：http://hz.haohaochexian.top/gtcbygqhen.html

Java: resp.statusCode()
来源：http://hz.ybcxt.top/gthktvaspd.html

Go:   resp.StatusCode
来源：http://hz.vqdsnc.cn/gtcnrgmbnx.html

Ruby: resp.code.to_i
来源：http://hz.yj202588.top/gtmnybbgoq.html


<!-- 参考信息 -->