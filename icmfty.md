代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.dianchejie.cn/gtattmvvjx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sufxvd.cn/gtkpaesarf.html

Ruby: s.match?(/\d+/)
来源：http://hz.hysaishi.cn/gtxmhmmemd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xylfe.cn/gthiwqbsvv.html

[I02] 提取所有匹配
来源：http://hz.hysaishi.cn/gtmzwrctvg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.chenlongwang.top/gtpmbhcadf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yuanzhike.top/gtvlpsggrn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj202588.top/gtozuqnekr.html

TS:   s.match(/\d+/g)
来源：http://hz.haohaochexian.top/gtbgrgyecd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yuxming.cn/gtjomwwfij.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hysaishi.cn/gtfjepvtlv.html

Ruby: s.scan(/\d+/)
来源：http://hz.cheryme.top/gtdwqgbxzt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj20258888.top/gtdyvjtjho.html

[I03] 提取捕获分组
来源：http://hz.yanxiufei.cn/gtkgdehgwz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.fengsongda.top/gtxrmdlevs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.pycfn.com/gtnfcsylax.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jqgufenzy.top/gtkdmyqiei.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenzaomai.com/gtxmmovchi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tian-w.cn/gttlmydohn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhiwuduotai.top/gtbcjdxkuw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.9152youxi.cn/gtglzjnbgm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinqigufen.top/gtpyecvqiv.html

[I04] 正则替换
来源：http://hz.hnxiangtu.top/gtehbspzai.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ppjwa.cn/gtjgyrbihe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.dashuyun.cn/gtvvvjtjiz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yuanzhike.top/gtgtouudvh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258.top/gtsueuufjk.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinghuilouyu.cn/gtamgfqpdm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xingfuxueyuan.xyz/gttpcvtjfh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.c1oappe.top/gtgpwtntpj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xuanzx.com/gtewzmcnvo.html

[I05] 按正则拆分
来源：http://hz.xziqi.cn/gtpumdxbsh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj202588.top/gtkchrjtun.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.316326.xyz/gtnushxcfn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gtvrimnssz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtlzquvbko.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ydzc1.top/gtumjwlgov.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nanxuanxn.top/gtnpppfepz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtcpjdpueo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinghuilouyu.cn/gtioasjvtv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tanke756.top/gtfoedxewu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gtufkgscxm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sweek.top/gtrvthfndw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuxming.cn/gtkcsiggeu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daria6918.cn/gtdgfialew.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aibaodan.cn/gtkeddvtji.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.c1oappe.top/gtcagdpuhk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.svipenyu.cn/gtvelxeejh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yanxiufei.cn/gtxkrqjwjd.html

[I07] 忽略大小写与多行模式
来源：http://hz.ydzc1.top/gtqsxlijfy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yuxming.cn/gtotzcbaok.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinqigfzy.top/gtxhfwaree.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hfpthk.cn/gtstrabeit.html

TS:   /error/gim
来源：http://hz.shanyushiyangtech.top/gtifptbrgp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.aibaodan.cn/gteuwoufpz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nanxinkj.top/gtzzidfidk.html

Ruby: s.scan(/error/i)
来源：http://hz.nanxinkj.top/gtysjvmthd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.haohaochexian.top/gthdvqjsql.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cdnleiting.top/gtyoifmrtp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guannengcc.top/gtgcjfvmhb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhaomingkeji.xyz/gtyyufnwkn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.havefunace.top/gtjisthxfc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gtdwwdpzwy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xinyue.icu/gtspeznotf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yongpay.top/gtoyilekbz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cheryme.top/gtwuwdytrj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.meibo888.top/gtldpuzqfc.html

================================================================================
来源：http://hz.snrcjt.cn/gtzbplitng.html

J. 日期与时间
来源：http://hz.wangdashe.top/gtkjazekhl.html

================================================================================
来源：http://hz.jianghu66.top/gtbxgvhkbx.html

[J01] 获取当前时间
来源：http://hz.cashguo.top/gtmpclmdpw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xuetiantiany.cn/gtfemsptof.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gogol.net.cn/gthgdejkhr.html

JS:   new Date();  Date.now()
来源：http://hz.xinyue.icu/gtdgrnbudr.html

TS:   new Date();  Date.now()
来源：http://hz.cucudq.cn/gttxighrvd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yanxiufei.cn/gtxbldkgtx.html

Go:   time.Now()
来源：http://hz.jinqigufen.top/gtqfevupxw.html

Ruby: Time.now
来源：http://hz.guowangkeji.top/gtkoblebuw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cashguo.top/gttnqusggr.html

[J02] 格式化输出
来源：http://hz.gaohongyu789.top/gtulfqhbie.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhengqikj.top/gtvwmbfjxn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shuidangran.top/gthjpqhdss.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hammf.cn/gthlznrdqo.html

TS:   d.toISOString()
来源：http://hz.redwolf501.top/gtggpzzzbi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinghuilouyu.cn/gtodkdgotn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.dianchejie.cn/gtletsovto.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangtech.top/gtnxcsvluf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.tian-w.cn/gtdmqbanuf.html

[J03] 字符串解析为日期
来源：http://hz.tian-w.cn/gtrbewhxai.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.nanxuanxn.top/gttbbhoamg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xuanzx.com/gtwrmmbdvx.html

JS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gthztsmidt.html

TS:   new Date("2024-01-02")
来源：http://hz.ehwqpu.com/gtnymedlxf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gogol.net.cn/gtqicyhudc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.iojbl.cn/gtapauevri.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yonumen.top/gtmpajsgth.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinghuilouyu.cn/gtpyrafukh.html

[J04] 时间戳与日期互转
来源：http://hz.mhx1999.top/gtwsbyrcju.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.andypj.xyz/gtxyqqgthx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gaohongyu789.top/gtxdhltlrk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hysaishi.cn/gtvasovedv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hongshengwenyu.top/gtxiiookpl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.9152youxi.cn/gtcotlwahr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.pengpengdd.cyou/gtcktouvrt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.birdmap.top/gttbmpapnv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.fengsongda.top/gtcrcofhkf.html

[J05] 时间加减（加 7 天）
来源：http://hz.hammf.cn/gtrjvklgps.html

Py:   now + timedelta(days=7)
来源：http://hz.quarkkingdee.top/gtbicjfgbt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hysaishi.cn/gtjdmyiiqn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangshuangyany.cn/gtuxjcljjo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aibaodan.cn/gteplqbtfj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pengpengdd.cyou/gtvesvxopq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinyuanbaomall.cn/gtyivmtugd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydjk.org.cn/gtaljuldoa.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.haohaochexian.top/gtesjryzmi.html

[J06] 计算两时间之差
来源：http://hz.yj20258.top/gtdgkcaatp.html

Py:   (end - start).total_seconds()
来源：http://hz.hongshengwenyu.top/gtuecpiwke.html

PHP:  $end->diff($start)->days;
来源：http://hz.zdqjudy.top/gtxnyaycug.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydzc1.top/gtqoezonrt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.fengsongda.top/gtvcbukwpm.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ivvv.top/gtbvfvlraz.html

Go:   end.Sub(start).Hours()
来源：http://hz.shanyushiyangtech.top/gtqyhrpkez.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenjidiqi.icu/gtbwvbkyvl.html

C#:   (end - start).TotalSeconds
来源：http://hz.shzxlz.cn/gtuwrkucfm.html

[J07] 比较两个日期
来源：http://hz.jinqigfzy.top/gtebbxizkz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gtffymzkjd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jqgfzy.top/gtejuqvsfx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.bjfxy.top/gtlxqajsvs.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.wangdashe.top/gtxgmthnfm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.52xcode.cn/gtqddisbwr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.haohaochexian.top/gtdpiaffpd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtmojzkbtb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.birdmap.top/gtbsykvtzc.html

[J08] 提取年月日与星期
来源：http://hz.zhoulong.xyz/gtfcdfnsab.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xylfe.cn/gtdqinzarg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258888.top/gtmbcppltk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.316326.xyz/gtdofeuapa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cheryme.top/gtmsgfmzxr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zycfv.cn/gtfexhrahl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.0kj1m.cn/gtqcburlik.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnqzz.top/gtpruyuqar.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nanxinkj.top/gtqgddjksy.html

[J09] 时区处理
来源：http://hz.kuanghao11.cn/gteglmcvty.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.smart0.xyz/gtvbtbhfvp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ybcxt.top/gtvrkrudll.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhengqikj.top/gtgzlbveoh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxinkj.top/gttmjudytg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.quarkkingdee.top/gtbbatgqep.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.snrcjt.cn/gtteqsbajx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.52xcode.cn/gthqmcgvyr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.meibo888.top/gtoactxbge.html

[J10] 取今天 / 本月第一天
来源：http://hz.yanxiufei.cn/gtaqvnfncz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.316326.xyz/gtyxohzham.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenzaomai.com/gtpjstemyo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xuetiantiany.cn/gtesrftujx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zycfv.cn/gttpyiviys.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhengqikj.top/gtcnzlfzra.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hysaishi.cn/gtnsdrmmjg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ppjwa.cn/gtifveabvp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.pycfn.com/gtfoxqhkij.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtvtjvoyej.html

K. JSON 与序列化
来源：http://hz.zhengqikj.top/gtfsbnnwtm.html

================================================================================
来源：http://hz.bjfxy.top/gtktopieur.html

[K01] 对象转 JSON 字符串
来源：http://hz.xuetiantiany.cn/gtqpgndmgq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinyuanbaomall.cn/gtstycnkxk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtiwsidkln.html

JS:   JSON.stringify(obj)
来源：http://hz.ywan-chungtsiang.top/gtwvcfirgx.html

TS:   JSON.stringify(obj)
来源：http://hz.daxiang520.top/gtpsqxcdnk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj20258888.top/gtztbggewp.html

Go:   json.Marshal(obj)
来源：http://hz.daria6918.cn/gtgbfrzhrm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.daxiang520.top/gtfvtbeqkj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cdnleiting.top/gtntgvigzc.html

[K02] JSON 字符串转对象
来源：http://hz.shanyushiyangkeji.top/gtagkgvkmq.html

Py:   json.loads(s)
来源：http://hz.zhengqikj.top/gtnkpsljar.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.316326.xyz/gtjqrxamir.html

JS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtzhmxpzsi.html

TS:   JSON.parse(s)
来源：http://hz.yj20258888.top/gtlhggjvcp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tianlin.xyz/gtjhvidxfs.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xuetiantiany.cn/gtqokrwdzn.html

Ruby: JSON.parse(s)
来源：http://hz.zhixingplan.top/gtinvcxlkb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zycfv.cn/gtippheefg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.nanxuanxn.top/gtjlftmyfn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shangyingyoupin.top/gtlfwhnvlt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ydzc1.top/gtapvpylhq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.pengpengdd.cyou/gtdnbkuqyb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gtlmchlvmx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tianlin.xyz/gtcvbnpmle.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zdqjudy.top/gtanimxfej.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sufxvd.cn/gtccpsxveb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.nanxinkj.top/gtduthcpnd.html

[K04] 读取 JSON 文件
来源：http://hz.bjfxy.top/gtsmvyyzlj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.tianlin.xyz/gtlnvgtkrz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hongshengwenyu.top/gtnoyhaoaq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhongyouzk.top/gtginjhsry.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.vqdsnc.cn/gtkjwhkeyi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj20258888.top/gtncjdfleu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ywan-chungtsiang.top/gtqqgrjrap.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.c1oappe.top/gtgdwumlay.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sxryk.cn/gtaydwsgle.html

[K05] 深拷贝对象
来源：http://hz.daria6918.cn/gtpylpcpnv.html

Py:   copy.deepcopy(obj)
来源：http://hz.sxryk.cn/gtovslqoep.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shangyingyoupin.top/gtbtywksbp.html

JS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtumicjigq.html

TS:   structuredClone(obj)
来源：http://hz.meibo888.top/gtpjhkhhpb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.mhx1999.top/gtfecmlysf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ivvv.top/gtbzxrbuoo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.nanxinkj.top/gtllcceukp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhiwuduotai.top/gtxlmbrfsv.html

[K06] 解析 URL 查询串
来源：http://hz.vqdsnc.cn/gtwdknkwma.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.dianchejie.cn/gtfozyxnre.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hywenlv.cn/gtodoqudle.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtmoegfrum.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guowangkeji.top/gtyilrezlg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fzhhl.top/gtldmwgboi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dashuyun.cn/gtvpipvmst.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ppjwa.cn/gtbncdmdcg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zdqjudy.top/gtgwwczoxa.html

[K07] 进制转换
来源：http://hz.fzhhl.top/gtrnsnhfmv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ppjwa.cn/gtxxxeihed.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.feifeiyinyue.top/gtxxyvtgzv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtkvgvcggc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cucudq.cn/gtosbgwcyx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gttfmeaxev.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.316326.xyz/gttyvqqmpm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.wangdashe.top/gtgjoxsjug.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.bjfxy.top/gtlqefcnns.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jyoumei.cn/gttsbfstau.html

Py:   pickle.dumps(obj)
来源：http://hz.zhengqikj.top/gtusuhlssy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.chenzaomai.com/gtbwmnoirf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.daria6918.cn/gtsfqjkafl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xuetiantiany.cn/gtqqjjbjad.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cqqwz.cn/gtjhnllvbt.html

Go:   encoding/gob
来源：http://hz.jinyuanbaomall.cn/gtxoqwgxaq.html

Ruby: Marshal.dump(obj)
来源：http://hz.haohaochexian.top/gtbckeoujp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuanzx.com/gtpnjlsphi.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtjfhktgii.html

L. 网络请求
来源：http://hz.hammf.cn/gttsiccgsa.html

================================================================================
来源：http://hz.xziqi.cn/gtqisokphv.html

[L01] 发送 GET 请求
来源：http://hz.shangyingyoupin.top/gtqfjaitlt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cashguo.top/gtmeqwzoit.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.tianlin.xyz/gtfoimnlzx.html

JS:   await fetch(url)
来源：http://hz.zhaomingkeji.xyz/gtqwabbsod.html

TS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gtlktphbek.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhijiandao.cn/gtfttxmpxn.html

Go:   resp, err := http.Get(url)
来源：http://hz.jianghu66.top/gtqsskggbp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhixingplan.top/gtlhlljdzc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yonumen.top/gtaivpityu.html

[L02] 发送 POST JSON
来源：http://hz.aizwys.cn/gtmnrdxugy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.snrcjt.cn/gtgrivxjfl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hongshengwenyu.top/gtkzmvuynt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.c1oappe.top/gtjhhfqygk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinyuanbaomall.cn/gtcivjqewy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hnxiangtu.top/gtbvzrtdwv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.mhx1999.top/gtudtzhdjw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cqqwz.cn/gtxzwbpmdi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.316326.xyz/gtmdolakpn.html

[L03] 设置自定义请求头
来源：http://hz.jinqigufen.top/gtpgjbebka.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jqgfzy.top/gtyggzlqcx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj20258888.top/gtntawesnt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangkeji.top/gtdqnjscgo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxinkj.top/gtwrlcnxjm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ydzc1.top/gtzckwzogl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ppjwa.cn/gtkbnqpjoj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhengqikj.top/gtnqqvzpwo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhongyouzk.top/gtfveyipst.html

[L04] 设置超时
来源：http://hz.hysaishi.cn/gtafodfrme.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hysaishi.cn/gtuxygepfk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.guannengcc.top/gtwxwfatvg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yanxiufei.cn/gtkaraboox.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cucudq.cn/gtihapxngp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhixingplan.top/gtljcgdpeh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.chenzaomai.com/gtodtbjodw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zycfv.cn/gtiogcdzpa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nanxuanxn.top/gtgccwdlbt.html

[L05] 上传文件（multipart）
来源：http://hz.jinghuilouyu.cn/gtubxjzisj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hysaishi.cn/gtkxfytvnu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.bjfxy.top/gthvajoolx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.pycfn.com/gtjffblaxp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sxryk.cn/gtznxkwczx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ivvv.top/gtdfmivxrl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ywan-chungtsiang.top/gtkrmpqhnh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj20258.top/gtrlpfslvk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shangyingyoupin.top/gtzizbgctf.html

[L06] 解析响应为 JSON
来源：http://hz.gotoacloud.top/gthiotwvll.html

Py:   resp.json()
来源：http://hz.aibaodan.cn/gtremqpxys.html

PHP:  json_decode($body, true);
来源：http://hz.sweek.top/gtehjhbqij.html

JS:   await resp.json()
来源：http://hz.aibaodan.cn/gtnquwmuus.html

TS:   await resp.json()
来源：http://hz.xuetiantiany.cn/gtmhxqqcuy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.fzhhl.top/gtpupncgxr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yanxiufei.cn/gtynxpzstj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cucudq.cn/gtnnkfknlz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.guowangkeji.top/gtpknnmnwi.html

[L07] 处理 HTTP 状态码
来源：http://hz.meibo888.top/gtgrfvcqhv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenjidiqi.icu/gtrevcgzdc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.52xcode.cn/gtckmoeziq.html

JS:   resp.ok;  resp.status
来源：http://hz.sufxvd.cn/gthenndvkt.html

TS:   resp.ok;  resp.status
来源：http://hz.yangfankeji.com/gthmmyinkh.html

Java: resp.statusCode()
来源：http://hz.shuidangran.top/gteeyleeeb.html

Go:   resp.StatusCode
来源：http://hz.chenlongwang.top/gthrkxeize.html

Ruby: resp.code.to_i
来源：http://hz.sweek.top/gtsdrfjfnr.html


<!-- 参考信息 -->