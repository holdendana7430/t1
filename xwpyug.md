代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jiagoushi.top/gtqqcnkhpk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.tanke756.top/gtzejgxvir.html

JS:   /\d+/.test(s)
来源：http://hz.yonumen.top/gtoylpywvz.html

TS:   /\d+/.test(s)
来源：http://hz.daxiang520.top/gtapnoshyz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yvedp.cn/gtrjvrpeue.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zdqjudy.top/gtvbdhmclg.html

Ruby: s.match?(/\d+/)
来源：http://hz.snrcjt.cn/gtrgtcgpnr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangshuangyany.cn/gtuhwwtgzn.html

[I02] 提取所有匹配
来源：http://hz.nwbrower.top/gtjkfriylu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhijiandao.cn/gtpdxyndpr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hammf.cn/gtiywtnmiq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.pengpengdd.cyou/gtwbpgqotu.html

TS:   s.match(/\d+/g)
来源：http://hz.yuxming.cn/gtrrdyzmsa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.nanxinkj.top/gtviaeblzh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hfpthk.cn/gtylixnhdx.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj202588.top/gtwehoxwhk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xingfuxueyuan.xyz/gteoavkmjp.html

[I03] 提取捕获分组
来源：http://hz.9152youxi.cn/gtnbegnwww.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xylfe.cn/gteesqkkgt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.haohaochexian.top/gtqitdllgf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pycfn.com/gtlxhrwiau.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.andypj.xyz/gtdcpeycsz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.smart0.xyz/gtemextgfe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.guowangkeji.top/gttvgmtcmo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cqqwz.cn/gtfmermhhz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shuidangran.top/gtfdhksbsm.html

[I04] 正则替换
来源：http://hz.yuxming.cn/gtmwfvsazg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.9152youxi.cn/gtifjfmlod.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.c1oappe.top/gtymnialrq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.feifeiyinyue.top/gtljwlvyso.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigfzy.top/gtdljrbgke.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dashuyun.cn/gttzuywpkb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jiagoushi.top/gtgmmymgcg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ppjwa.cn/gtuhfepyil.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.snrcjt.cn/gtgnvzpgmr.html

[I05] 按正则拆分
来源：http://hz.birdmap.top/gtmcvmzwas.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yangfankeji.com/gthkuisayf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xziqi.cn/gtcmdpngbr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yangfankeji.com/gtxiirpdwq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.guannengcc.top/gtjvvzlwgx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.c1oappe.top/gtmyyfxcpi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhaomingkeji.xyz/gtzgjprrqg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gtxvdovlkz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.meibo888.top/gtscjvejfr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.quarkkingdee.top/gtlintxkve.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hywenlv.cn/gttphmcoah.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gaohongyu789.top/gtpmnelbhq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yangfankeji.com/gthxcgqgki.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jianghu66.top/gtokjrpygy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sufxvd.cn/gtzzouprta.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.mhx1999.top/gtberpylqf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.tianlin.xyz/gtfcgcwfgq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.redwolf501.top/gtmspkzsag.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigfzy.top/gtoqigmrhp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zdqjudy.top/gtdtuxhfvu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hongshengwenyu.top/gtglcoanhu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.wangshuangyany.cn/gtoxlluwea.html

TS:   /error/gim
来源：http://hz.gaohongyu789.top/gtxrcdxezq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yuxming.cn/gtgvzvriwg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xuanzx.com/gtvzxgubnt.html

Ruby: s.scan(/error/i)
来源：http://hz.hammf.cn/gtwyidsnbt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenzaomai.com/gtreqvhvug.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.tianlin.xyz/gtnrxdjfiu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jlsjyb.cn/gtnupuyjhf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shanyushiyangkeji.top/gtazlvfhdh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yongpay.top/gthxjamkjg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258.top/gtdptmkqul.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daria6918.cn/gtbozhqstj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yuanzhike.top/gtwvwfimpb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zycfv.cn/gthzjjtvyj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.snrcjt.cn/gtggfetdbd.html

================================================================================
来源：http://hz.yuxming.cn/gtktjdokid.html

J. 日期与时间
来源：http://hz.jinqigfzy.top/gtzhqwvnhl.html

================================================================================
来源：http://hz.kuanghao11.cn/gtnkcsdtll.html

[J01] 获取当前时间
来源：http://hz.chenjidiqi.icu/gtkdlycgnx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.smart0.xyz/gtlxorwhvx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.pycfn.com/gtbqizajyv.html

JS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gtdbhwbcmx.html

TS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtpajcovse.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gzhubu.top/gtmtxeejjb.html

Go:   time.Now()
来源：http://hz.jinqigufen.top/gtdbsgjubw.html

Ruby: Time.now
来源：http://hz.cucudq.cn/gtaizjbqqr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yongpay.top/gtvmqtfdtc.html

[J02] 格式化输出
来源：http://hz.zhongyouzk.top/gtbttuqluv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenlongwang.top/gtofzgzxbb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gaohongyu789.top/gtmcqickeo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.vqdsnc.cn/gtrvffutct.html

TS:   d.toISOString()
来源：http://hz.cucudq.cn/gtdxvhidjf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yangfankeji.com/gtsrdddhzw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sufxvd.cn/gtgdelwntb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jiagoushi.top/gtbbkkvpnv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zycfv.cn/gtwvecpqcf.html

[J03] 字符串解析为日期
来源：http://hz.jinqigfzy.top/gtivmqbids.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xinyue.icu/gtuseqydmu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jlsjyb.cn/gtnwxbqdsz.html

JS:   new Date("2024-01-02")
来源：http://hz.yj20258888.top/gtaaaybetn.html

TS:   new Date("2024-01-02")
来源：http://hz.zhongyouzk.top/gtnfelkrjg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tianlin.xyz/gtxtbioxlq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yuanzhike.top/gtbkuuqrpm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtdwinvqrv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jiagoushi.top/gtnfyunmuu.html

[J04] 时间戳与日期互转
来源：http://hz.c1oappe.top/gtbxsjhjpz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nanxinkj.top/gtuhpsqxtb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinghuilouyu.cn/gtwywxuybv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hfpthk.cn/gtmglwdzzg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cheryme.top/gtbppudeyl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhoulong.xyz/gtivbgkzrq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cheryme.top/gtbqerifzw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tanke756.top/gtyxlaruyb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.daria6918.cn/gtgwmtzntu.html

[J05] 时间加减（加 7 天）
来源：http://hz.svipenyu.cn/gtygjcysve.html

Py:   now + timedelta(days=7)
来源：http://hz.yongpay.top/gtyfjlbahh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tian-w.cn/gtqpyjxorh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhaomingkeji.xyz/gtdgqznqyv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zycfv.cn/gtcqdfrzex.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhaomingkeji.xyz/gtctjzfoct.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xinyue.icu/gtmvoosxso.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tian-w.cn/gtgsaxmtkm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ehwqpu.com/gtgdcgibeu.html

[J06] 计算两时间之差
来源：http://hz.cashguo.top/gtjedzjqpd.html

Py:   (end - start).total_seconds()
来源：http://hz.chenzaomai.com/gtklyenhov.html

PHP:  $end->diff($start)->days;
来源：http://hz.316326.xyz/gthvzrddzo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yuanzhike.top/gtmqxmhisu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigufen.top/gtjfrhlrin.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.dashuyun.cn/gtchzkxwgy.html

Go:   end.Sub(start).Hours()
来源：http://hz.cheryme.top/gtsucthyag.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgufenzy.top/gtzhlenhfb.html

C#:   (end - start).TotalSeconds
来源：http://hz.jianghu66.top/gtsdtmreuk.html

[J07] 比较两个日期
来源：http://hz.cdnleiting.top/gtmbmplblp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtqvbwlyxg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.svipenyu.cn/gthmrphhxh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sufxvd.cn/gtlfyqfype.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtjavtrhwp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxuanxn.top/gtmfhisxij.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guannengcc.top/gtbnijddus.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtfgwefyxz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtsyfwoujj.html

[J08] 提取年月日与星期
来源：http://hz.xylfe.cn/gtbxznmtdw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.wangshuangyany.cn/gtfyvvqkex.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tian-w.cn/gtxhqvzwnh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.mhx1999.top/gtuoqyboeu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nanxuanxn.top/gtzehwuozw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daria6918.cn/gtontndbqe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhongyouzk.top/gtaqtgirnx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yuanzhike.top/gtervionzv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yongpay.top/gtdxnyscgw.html

[J09] 时区处理
来源：http://hz.yj20258.top/gtpewxuqya.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hywenlv.cn/gtwddxwbma.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenlongwang.top/gtwhugeyhd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.redwolf501.top/gtvzlupmgd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.redwolf501.top/gtfnnommzs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wangdashe.top/gtqhhttcvf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nwbrower.top/gtppgifcrp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yuanzhike.top/gtxciuqatz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xziqi.cn/gtdfvttijl.html

[J10] 取今天 / 本月第一天
来源：http://hz.havefunace.top/gtifvmxbou.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yueranfly.top/gtitoxecfp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.guannengcc.top/gtqtyfdfjv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxuanxn.top/gtaayeimxk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shuidangran.top/gtlzdemjie.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tanke756.top/gtbrzutrap.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.fengsongda.top/gtszvrtnnb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sweek.top/gtmijguayg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yuanzhike.top/gtcyszcsnr.html

================================================================================
来源：http://hz.bjfxy.top/gtyvfjowgx.html

K. JSON 与序列化
来源：http://hz.smart0.xyz/gtaaazermj.html

================================================================================
来源：http://hz.guannengcc.top/gtdvsprxzt.html

[K01] 对象转 JSON 字符串
来源：http://hz.52xcode.cn/gtgohgjith.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydzc1.top/gtzswtsemr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gtrejjfoui.html

JS:   JSON.stringify(obj)
来源：http://hz.xingfuxueyuan.xyz/gtvultuolc.html

TS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtfploihch.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shuidangran.top/gtfvrqqplm.html

Go:   json.Marshal(obj)
来源：http://hz.birdmap.top/gtwtdvzxfn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj20258888.top/gtrcrwatgy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gotoacloud.top/gtpkgnwhjf.html

[K02] JSON 字符串转对象
来源：http://hz.dashuyun.cn/gtxgttgkop.html

Py:   json.loads(s)
来源：http://hz.zycfv.cn/gtgkqikmfl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ywan-chungtsiang.top/gteaxlcfsv.html

JS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtnxraydns.html

TS:   JSON.parse(s)
来源：http://hz.zdqjudy.top/gtqagcpsjw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnxiangtu.top/gtsvlbswwe.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.feifeiyinyue.top/gtscujptse.html

Ruby: JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtujgwmdis.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shangyingyoupin.top/gtwkycddqv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhoulong.xyz/gticntudmx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnqzz.top/gtjmyrwbqa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.guannengcc.top/gtfsxqflbj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gtlbdxynsn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xylfe.cn/gtiqhpyzyn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cashguo.top/gtopoxhrqf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cucudq.cn/gtsnwcjtfo.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tianlin.xyz/gtneotwlla.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhixingplan.top/gtcfdkzbfb.html

[K04] 读取 JSON 文件
来源：http://hz.jiagoushi.top/gtwjripoft.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.guowangkeji.top/gtfjmziyqg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj20258888.top/gtazcjhhdi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtkofnmruo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgfzy.top/gtbnkuwsdm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hywenlv.cn/gtoyslujjo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.tanke756.top/gtcnsrqftm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ivvv.top/gtmqclsuhv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sysykeji.top/gtjenjyjng.html

[K05] 深拷贝对象
来源：http://hz.fengsongda.top/gtzkddwmrn.html

Py:   copy.deepcopy(obj)
来源：http://hz.gotoacloud.top/gttbfszyum.html

PHP:  unserialize(serialize($obj));
来源：http://hz.guannengcc.top/gtpsvkrbvt.html

JS:   structuredClone(obj)
来源：http://hz.vqdsnc.cn/gtimtkqqea.html

TS:   structuredClone(obj)
来源：http://hz.hfpthk.cn/gtrohmgtxg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinyuanbaomall.cn/gtzrprffho.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xylfe.cn/gtaylyilap.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.havefunace.top/gtwhikgzny.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.daxiang520.top/gtgnzhadhz.html

[K06] 解析 URL 查询串
来源：http://hz.wangshuangyany.cn/gtnzwoyeep.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.mhx1999.top/gthyrnqkto.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hnqzz.top/gtmldsfmlq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.iojbl.cn/gtbpfypvyu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yueranfly.top/gtxlvedhfz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hnqzz.top/gtfxikyevh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gtmizipgwm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aizwys.cn/gtrfqqytzr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sufxvd.cn/gtxtjywdep.html

[K07] 进制转换
来源：http://hz.wangdashe.top/gtzmnnjzfe.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yanxiufei.cn/gtojvxeskb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tian-w.cn/gtyqceydub.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gttphfdunt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtagszvlcw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtzigzuior.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xuanzx.com/gtdtnkzjnt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daria6918.cn/gtggyzahft.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenjidiqi.icu/gtqavbbqib.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.redwolf501.top/gtzczwcvvb.html

Py:   pickle.dumps(obj)
来源：http://hz.bjfxy.top/gtvcgsstfo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shanyushiyangtech.top/gtrkfojhxx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gtzbjzbibj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.wangshuangyany.cn/gttuulnmep.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ydzc1.top/gtzawkxipl.html

Go:   encoding/gob
来源：http://hz.sufxvd.cn/gtrebwpvgz.html

Ruby: Marshal.dump(obj)
来源：http://hz.yuanzhike.top/gtisvjmkaq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.feifeiyinyue.top/gtbajpbyum.html

================================================================================
来源：http://hz.nwbrower.top/gtdwrgdrzn.html

L. 网络请求
来源：http://hz.pengpengdd.cyou/gtfjvjpvql.html

================================================================================
来源：http://hz.tanke756.top/gtzvzczkni.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangtech.top/gtukyvlnyc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.bjfxy.top/gtinlpdwmu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gotoacloud.top/gtngtyzcsx.html

JS:   await fetch(url)
来源：http://hz.shzxlz.cn/gtirdlzref.html

TS:   await fetch(url)
来源：http://hz.cucudq.cn/gtlimqvhaq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gotoacloud.top/gtmoazyujp.html

Go:   resp, err := http.Get(url)
来源：http://hz.c1oappe.top/gtqxiwvbwe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.smart0.xyz/gtkxeoqwnd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hywenlv.cn/gtlvlcrucf.html

[L02] 发送 POST JSON
来源：http://hz.fengsongda.top/gtrylupndo.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.smart0.xyz/gtelfuwjta.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuanzx.com/gtyxewllic.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtxhckmurp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.meibo888.top/gtagwgyvvl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cucudq.cn/gtofkfwzjo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ppjwa.cn/gtlkfpxrjd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gzhubu.top/gtanvvojbh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jqgufenzy.top/gtfmjifqho.html

[L03] 设置自定义请求头
来源：http://hz.kuanghao11.cn/gtcdowgauj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sufxvd.cn/gtinowpqun.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zdqjudy.top/gtrhuqpdkr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangshuangyany.cn/gtmgowrhjt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigufen.top/gtlphmdswg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhijiandao.cn/gtehqzwciu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.wangdashe.top/gtoxhbxikz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xinyue.icu/gtkzbxfomf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yj20258888.top/gtzomubjmn.html

[L04] 设置超时
来源：http://hz.yvedp.cn/gtbrtqpupl.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydzc1.top/gtshdrsdge.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xziqi.cn/gttkecviaw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cheryme.top/gtsweqsxeu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinyuanbaomall.cn/gtgyzdfbib.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.havefunace.top/gtoyskzdbb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cucudq.cn/gtykhsmkad.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinqigufen.top/gtrvkupvbc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sysykeji.top/gtnwfbohbe.html

[L05] 上传文件（multipart）
来源：http://hz.zdqjudy.top/gtqkonrkos.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xingfuxueyuan.xyz/gtdljcfewf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.chenjidiqi.icu/gtytwwgaxs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gtnycznshv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shzxlz.cn/gtdykkmnee.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ppjwa.cn/gtlodjckyb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.daxiang520.top/gtqyoyipgd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigufen.top/gtnwwlcjdb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zdqjudy.top/gtiuidmeoo.html

[L06] 解析响应为 JSON
来源：http://hz.ydjk.org.cn/gtuaaietit.html

Py:   resp.json()
来源：http://hz.cheryme.top/gtdmmnmeuz.html

PHP:  json_decode($body, true);
来源：http://hz.sxryk.cn/gtvavxgtxu.html

JS:   await resp.json()
来源：http://hz.zhengqikj.top/gtguhttxqc.html

TS:   await resp.json()
来源：http://hz.aibaodan.cn/gtlczwmfjk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zdqjudy.top/gtstyllcxt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.smart0.xyz/gtgmvnhujn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cqqwz.cn/gtueedswrv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ehwqpu.com/gtdifhcczm.html

[L07] 处理 HTTP 状态码
来源：http://hz.jyoumei.cn/gteflqrkcv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj20258888.top/gttrzlbnyq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinyuanbaomall.cn/gteviisdid.html

JS:   resp.ok;  resp.status
来源：http://hz.gaohongyu789.top/gtdqatzszr.html


<!-- 参考信息 -->