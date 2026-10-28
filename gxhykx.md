代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ehwqpu.com/gtpqvzsgml.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cashguo.top/gtcfjnkxpb.html

Ruby: s.match?(/\d+/)
来源：http://hz.aibaodan.cn/gtxmweqzpz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hammf.cn/gtphlhtizb.html

[I02] 提取所有匹配
来源：http://hz.ppjwa.cn/gtamtghbzj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhongyouzk.top/gtuhodmqke.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangtech.top/gtkjsyseuz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jiagoushi.top/gtsufjpbaw.html

TS:   s.match(/\d+/g)
来源：http://hz.svipenyu.cn/gtaiteamjb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.feifeiyinyue.top/gtpdtmnpxl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.pengpengdd.cyou/gtvnukoqnq.html

Ruby: s.scan(/\d+/)
来源：http://hz.ivvv.top/gtzyewoaty.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.guowangkeji.top/gtprnjpywo.html

[I03] 提取捕获分组
来源：http://hz.dashuyun.cn/gtudjsnrcf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.c1oappe.top/gtjavvebcr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ehwqpu.com/gtemlqqgai.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.bjfxy.top/gtaaedrvcl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.9152youxi.cn/gtptbhyftd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.andypj.xyz/gtccgrdchc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.vqdsnc.cn/gtyonvjzdp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.aizwys.cn/gtqlyadyhf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zycfv.cn/gtezhzhenn.html

[I04] 正则替换
来源：http://hz.kuanghao11.cn/gtuonnnvfm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.fzhhl.top/gtssyexgzs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.aizwys.cn/gteyrcyaoz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gthifgchcv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.wangshuangyany.cn/gtjwrftihs.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tanke756.top/gtslfcdqap.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.birdmap.top/gtmskvneih.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jyoumei.cn/gtbgsjtzmv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.havefunace.top/gtwtwnhgbs.html

[I05] 按正则拆分
来源：http://hz.zdqjudy.top/gtqpmyxsgr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hnqzz.top/gtrkllcvqy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xinyue.icu/gtssjjptzz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gtwimjpycl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cashguo.top/gtomsiujqf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cheryme.top/gtbumvlank.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hfpthk.cn/gtzcqbckfb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhongyouzk.top/gtwaeainbh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sweek.top/gtcqhqqjei.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.mhx1999.top/gtuonuogyt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj202588.top/gtuqecdflt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.havefunace.top/gtgaxtllpj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.snrcjt.cn/gtlvncpqxt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhongyouzk.top/gtykyyauxs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cheryme.top/gttxwfnomb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xingfuxueyuan.xyz/gtchzyvxam.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenjidiqi.icu/gtscoscpty.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gttzfuxexn.html

[I07] 忽略大小写与多行模式
来源：http://hz.vqdsnc.cn/gtuhudavyt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cheryme.top/gtepkgupry.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.snrcjt.cn/gttjjordlr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhijiandao.cn/gtyuaahvdq.html

TS:   /error/gim
来源：http://hz.daria6918.cn/gthgocmrav.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ivvv.top/gtngddpyix.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinqigfzy.top/gtzqgpwich.html

Ruby: s.scan(/error/i)
来源：http://hz.mhx1999.top/gtkumvvxap.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tian-w.cn/gtvehsywnm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.birdmap.top/gtfhoqslzm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.haohaochexian.top/gtgnwkvdbz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.pycfn.com/gtdlrcvhfb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtnfshnkma.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhixingplan.top/gttyfqwmam.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yonumen.top/gtfngbqjyf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhengqikj.top/gtbyhmyhti.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.haohaochexian.top/gtsvksoqpy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ywan-chungtsiang.top/gtewuxwrle.html

================================================================================
来源：http://hz.aibaodan.cn/gtosdgeleu.html

J. 日期与时间
来源：http://hz.yongpay.top/gtuyqvfbgk.html

================================================================================
来源：http://hz.hywenlv.cn/gtdudkkraq.html

[J01] 获取当前时间
来源：http://hz.chenlongwang.top/gtpioqfgvv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nanxuanxn.top/gtnfeiqlqm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtewsjdhwm.html

JS:   new Date();  Date.now()
来源：http://hz.tian-w.cn/gtbfctrlmr.html

TS:   new Date();  Date.now()
来源：http://hz.guowangkeji.top/gtszsaijdz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yuxming.cn/gtomuabpcn.html

Go:   time.Now()
来源：http://hz.yueranfly.top/gtvolusbam.html

Ruby: Time.now
来源：http://hz.jinqigfzy.top/gtlhfotfqt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xuetiantiany.cn/gtmkbcfgcb.html

[J02] 格式化输出
来源：http://hz.yj202588.top/gtazadtbbv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guannengcc.top/gtiiwaogdx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gtjbmhthty.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zycfv.cn/gtobvfqwfe.html

TS:   d.toISOString()
来源：http://hz.jyoumei.cn/gtbyggoiaz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gzhubu.top/gtkfekfati.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jyoumei.cn/gttuqbykjf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.feifeiyinyue.top/gtebheqiuf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shanyushiyangkeji.top/gtykqbneav.html

[J03] 字符串解析为日期
来源：http://hz.cucudq.cn/gttoyynfzc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.andypj.xyz/gtoyakaxfy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xziqi.cn/gtrmvrkikq.html

JS:   new Date("2024-01-02")
来源：http://hz.yanxiufei.cn/gtsyqwomkk.html

TS:   new Date("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtqyptbkcc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.havefunace.top/gtckkscuxs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.9152youxi.cn/gtlgvhdmtt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gtffujypaz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jqgufenzy.top/gthhyqhjcq.html

[J04] 时间戳与日期互转
来源：http://hz.hysaishi.cn/gtvloqmkuf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xuanzx.com/gtjcmltdst.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shzxlz.cn/gtclnoxqio.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.c1oappe.top/gtwmdzfcdq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.mhx1999.top/gtnuvsfyoh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhaomingkeji.xyz/gtkkdapkcw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yuanzhike.top/gtlzpxgnrf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ivvv.top/gtfnwgoatj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258888.top/gteilonhef.html

[J05] 时间加减（加 7 天）
来源：http://hz.ydjk.org.cn/gtrpozmdze.html

Py:   now + timedelta(days=7)
来源：http://hz.jinyuanbaomall.cn/gtlydqcsyl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shangyingyoupin.top/gtpajbmynn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxinkj.top/gtxfglvedp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj202588.top/gteraqmmpr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xuetiantiany.cn/gtgecvmfox.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.dianchejie.cn/gtkbafvucm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shzxlz.cn/gttffwydrv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sysykeji.top/gtcndzbdgo.html

[J06] 计算两时间之差
来源：http://hz.pengpengdd.cyou/gtxgcgowog.html

Py:   (end - start).total_seconds()
来源：http://hz.yvedp.cn/gtontpqspf.html

PHP:  $end->diff($start)->days;
来源：http://hz.gotoacloud.top/gtbzhylwlb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinghuilouyu.cn/gtnfneyyvm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhiwuduotai.top/gtqbuqpcui.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hysaishi.cn/gtebmzidqv.html

Go:   end.Sub(start).Hours()
来源：http://hz.0kj1m.cn/gtwwmnjfjn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.52xcode.cn/gtjgezoigv.html

C#:   (end - start).TotalSeconds
来源：http://hz.xylfe.cn/gtzraxozez.html

[J07] 比较两个日期
来源：http://hz.cheryme.top/gtbngnovnt.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtlwxguwnt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ivvv.top/gtsisofnjn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guowangkeji.top/gtmbypkedo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hnqzz.top/gtmkxzqvbw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jqgufenzy.top/gtltrswiqb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tianlin.xyz/gtapxzoddi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtuylaseuz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtbekjhpas.html

[J08] 提取年月日与星期
来源：http://hz.snrcjt.cn/gtexgbgxns.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhoulong.xyz/gtfvjhwqcs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gotoacloud.top/gtyjtdnzgq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.quarkkingdee.top/gtcyadbwrh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.vqdsnc.cn/gtbzpztwlv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.wangshuangyany.cn/gtychvccnh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.c1oappe.top/gtrcwwpovc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shzxlz.cn/gtngnihwkd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pengpengdd.cyou/gtmknhpjyb.html

[J09] 时区处理
来源：http://hz.hongshengwenyu.top/gtcyafyxwj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sufxvd.cn/gtcnsnpcph.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jqgfzy.top/gttbziknsf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yongpay.top/gtdukxzsmf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.316326.xyz/gtoaktlyfy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.316326.xyz/gtwwflxnzp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.quarkkingdee.top/gtdkexzpzl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jlsjyb.cn/gtxhslthnc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ydjk.org.cn/gturfgtxgz.html

[J10] 取今天 / 本月第一天
来源：http://hz.wangdashe.top/gthxfrkpyi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tian-w.cn/gtxwwuozvq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yangfankeji.com/gtggvyndcw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenzaomai.com/gtqwfgobpn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenjidiqi.icu/gtziuhatag.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinqigfzy.top/gtcvpeztpz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xziqi.cn/gtvpooxuzq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gaohongyu789.top/gtjsctcapc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.birdmap.top/gtwmvvhldd.html

================================================================================
来源：http://hz.zhongyouzk.top/gtwsumkxjj.html

K. JSON 与序列化
来源：http://hz.ivvv.top/gtxfjoceqn.html

================================================================================
来源：http://hz.nanxinkj.top/gtokjxbyet.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgufenzy.top/gtzfyqpifb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yvedp.cn/gtlwyxsisu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xylfe.cn/gtlbnvesvn.html

JS:   JSON.stringify(obj)
来源：http://hz.zhaomingkeji.xyz/gtguizzjku.html

TS:   JSON.stringify(obj)
来源：http://hz.tanke756.top/gtqkclhadj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zycfv.cn/gtztrrwgpg.html

Go:   json.Marshal(obj)
来源：http://hz.jianghu66.top/gtschkwhkz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.fengsongda.top/gtkzzurnsn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangdashe.top/gtapsezppd.html

[K02] JSON 字符串转对象
来源：http://hz.hammf.cn/gtrpfctlfk.html

Py:   json.loads(s)
来源：http://hz.cashguo.top/gttrzlrvlq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.9152youxi.cn/gtnrfowwwh.html

JS:   JSON.parse(s)
来源：http://hz.mhx1999.top/gtfszlotey.html

TS:   JSON.parse(s)
来源：http://hz.pycfn.com/gtfredfuxq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jqgfzy.top/gtcuwtznvi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.wangshuangyany.cn/gtojufdznt.html

Ruby: JSON.parse(s)
来源：http://hz.hfpthk.cn/gtdluxjuxk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cheryme.top/gtjhkhkcpt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhixingplan.top/gtcxwaqlas.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtrcskydoh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhengqikj.top/gtndulvxcw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhengqikj.top/gtqcdctgdz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgufenzy.top/gtaovcnnxl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sufxvd.cn/gttusevcwp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xziqi.cn/gtthxgqbpa.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhoulong.xyz/gtgocffqrv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guannengcc.top/gtxmxzkuiy.html

[K04] 读取 JSON 文件
来源：http://hz.cucudq.cn/gtfjevjzll.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.vqdsnc.cn/gtkdymptzk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.smart0.xyz/gtqqnlmtbd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhixingplan.top/gtbzcnepgq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtbiekgilx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xuanzx.com/gtkilwojyg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yj20258888.top/gtdwjkivjw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.sxryk.cn/gtbpzlgeaa.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ywan-chungtsiang.top/gtyzpncaek.html

[K05] 深拷贝对象
来源：http://hz.shanyushiyangkeji.top/gtkgtvizaw.html

Py:   copy.deepcopy(obj)
来源：http://hz.aibaodan.cn/gtunptjujb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhiwuduotai.top/gtabsqoiwb.html

JS:   structuredClone(obj)
来源：http://hz.ivvv.top/gtdjppouxo.html

TS:   structuredClone(obj)
来源：http://hz.shuidangran.top/gtjrxdyifn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenzaomai.com/gtbrkcgfxk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yongpay.top/gtqtzervhy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ybcxt.top/gtjqqgiwcb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.0kj1m.cn/gtmhzulzgk.html

[K06] 解析 URL 查询串
来源：http://hz.pycfn.com/gtmybvacaa.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ppjwa.cn/gtfzaosbld.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yueranfly.top/gtuvkjrjec.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.haohaochexian.top/gtvwycowcl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.0kj1m.cn/gtvqjqnnuj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tanke756.top/gtdjtqehfx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj20258.top/gtdjtccuvs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtvbeotzro.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtilpxensw.html

[K07] 进制转换
来源：http://hz.iojbl.cn/gtjetntxdr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.nwbrower.top/gtqmqneakm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydzc1.top/gtlbulofsd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhengqikj.top/gtamrpmceb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtjsihvcvl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtujfrzcyi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.guannengcc.top/gtrjdfukad.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhaomingkeji.xyz/gtbcrhnorl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj202588.top/gtnthckoan.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj20258.top/gtwjvpwctz.html

Py:   pickle.dumps(obj)
来源：http://hz.yvedp.cn/gtipwlnfju.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ydzc1.top/gtdfvtoesf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258888.top/gtoqwlsehl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gogol.net.cn/gtygjgvwid.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.svipenyu.cn/gtmongourc.html

Go:   encoding/gob
来源：http://hz.shanyushiyangtech.top/gtvibzhcmo.html

Ruby: Marshal.dump(obj)
来源：http://hz.nwbrower.top/gtwaitmhzm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuanzx.com/gtxtwcnyfv.html

================================================================================
来源：http://hz.aizwys.cn/gtbingncdy.html

L. 网络请求
来源：http://hz.zdqjudy.top/gtvuwdcgyx.html

================================================================================
来源：http://hz.fengsongda.top/gtclmlmiur.html

[L01] 发送 GET 请求
来源：http://hz.wangshuangyany.cn/gtjxqycwgs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ydzc1.top/gtnetqtmim.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.dianchejie.cn/gtislmsomj.html

JS:   await fetch(url)
来源：http://hz.ydzc1.top/gtesdobbwb.html

TS:   await fetch(url)
来源：http://hz.hnqzz.top/gtzrnisnul.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj20258.top/gtiavywzah.html

Go:   resp, err := http.Get(url)
来源：http://hz.bjfxy.top/gthvkljmrv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.pengpengdd.cyou/gtqxynrgui.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zycfv.cn/gtmjlsqaek.html

[L02] 发送 POST JSON
来源：http://hz.c1oappe.top/gtheiekdfl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cheryme.top/gteqcxlqrr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sysykeji.top/gtgixbjwfd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jyoumei.cn/gttujwhofp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxuanxn.top/gtblootmko.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sweek.top/gtkldcpxjn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.pycfn.com/gtxaqkmund.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhiwuduotai.top/gtmjmeesbv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.52xcode.cn/gtkhamqome.html

[L03] 设置自定义请求头
来源：http://hz.yj20258888.top/gtgznbsbxy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zdqjudy.top/gtcdqqadpq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.vqdsnc.cn/gtjhpfjbbr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenjidiqi.icu/gtiztuiczn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gtvnmobeaa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jiagoushi.top/gtjxwbgdmr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.haohaochexian.top/gtrxitfons.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj20258888.top/gtrtsmzwhf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.svipenyu.cn/gthheavdlm.html

[L04] 设置超时
来源：http://hz.fzhhl.top/gttrunffir.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinqigfzy.top/gtqljwbxyg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jyoumei.cn/gtehtgkhsv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dianchejie.cn/gtyrejuode.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtfihemnos.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sxryk.cn/gtyvkmjgoe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.nanxinkj.top/gtdvascgfu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shzxlz.cn/gtakrekxma.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.daxiang520.top/gtwtwaxqwl.html

[L05] 上传文件（multipart）
来源：http://hz.ydjk.org.cn/gtdlknqwnf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.pycfn.com/gtjdlchqne.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.c1oappe.top/gtzcoxvasb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.9152youxi.cn/gtkwbinkwv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jlsjyb.cn/gtnndfjlci.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yvedp.cn/gtwtilxotj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxuanxn.top/gtdhqqxbaj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ybcxt.top/gtoykgaqqc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hfpthk.cn/gtrohxeibe.html

[L06] 解析响应为 JSON
来源：http://hz.hongshengwenyu.top/gtjjngaerx.html

Py:   resp.json()
来源：http://hz.gotoacloud.top/gtvuxjxaka.html

PHP:  json_decode($body, true);
来源：http://hz.gzhubu.top/gtxaureyiq.html

JS:   await resp.json()
来源：http://hz.svipenyu.cn/gtsljnyfpq.html

TS:   await resp.json()
来源：http://hz.jinqigufen.top/gtwhdrpkyb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.daria6918.cn/gtatqdpvsc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dashuyun.cn/gtodrpvoyy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.redwolf501.top/gthrypmrip.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hongshengwenyu.top/gtrouqjbba.html

[L07] 处理 HTTP 状态码
来源：http://hz.daria6918.cn/gtbcupufds.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zycfv.cn/gtchzgyuyd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hfpthk.cn/gtrofwwthl.html

JS:   resp.ok;  resp.status
来源：http://hz.gotoacloud.top/gtvbobchhn.html

TS:   resp.ok;  resp.status
来源：http://hz.jinqigufen.top/gtluvqgomy.html

Java: resp.statusCode()
来源：http://hz.yj20258.top/gtbbfkwgiw.html

Go:   resp.StatusCode
来源：http://hz.andypj.xyz/gtrdmtwnlr.html

Ruby: resp.code.to_i
来源：http://hz.hywenlv.cn/gtlbocofkz.html


<!-- 参考信息 -->