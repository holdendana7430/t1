代发 wailian999

[I02] 提取所有匹配
来源：http://hz.shanyushiyangkeji.top/gtdfyacsqb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shuidangran.top/gtdpvtywmi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fengsongda.top/gttcfdfxpp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.meibo888.top/gtmykzgfan.html

TS:   s.match(/\d+/g)
来源：http://hz.aibaodan.cn/gtjdkahujf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.pengpengdd.cyou/gtqizebfxw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shuidangran.top/gtmdcfdigf.html

Ruby: s.scan(/\d+/)
来源：http://hz.fzhhl.top/gtqkomkqan.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yuanzhike.top/gtkoroqulu.html

[I03] 提取捕获分组
来源：http://hz.dashuyun.cn/gtiffgzafx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gzhubu.top/gtzkaemvje.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xinyue.icu/gtfgovikpt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.andypj.xyz/gtrfrkpldl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.wangshuangyany.cn/gtomqjyayu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuanzx.com/gtcrkgiahz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.daxiang520.top/gtyyqzaykc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ehwqpu.com/gtvdwohlao.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.dianchejie.cn/gttcilceco.html

[I04] 正则替换
来源：http://hz.mhx1999.top/gtewtrtwkj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shuidangran.top/gtyvkfnunk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yueranfly.top/gtyevevzyg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ehwqpu.com/gtyqxcmwqy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.dashuyun.cn/gtshjdflnh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cqqwz.cn/gtitnavydb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yuxming.cn/gtuyajpdop.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.316326.xyz/gtnejexnzf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhijiandao.cn/gtwtlldlfz.html

[I05] 按正则拆分
来源：http://hz.nanxinkj.top/gtkkuyvfxx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.chenlongwang.top/gthwsccwcz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xziqi.cn/gtxukxethr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yanxiufei.cn/gtbjwicirp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtqrfskkcz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinqigufen.top/gteofrbwwo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.vqdsnc.cn/gtaivtxnzv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtqywanslp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yangfankeji.com/gttklxezfg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.wangshuangyany.cn/gtxeoftjpa.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.bjfxy.top/gtnawmjeuc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sufxvd.cn/gtvmrcztqm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hywenlv.cn/gtlidjdtlg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hongshengwenyu.top/gtlvvlpxof.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jqgfzy.top/gtsipofjex.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xuanzx.com/gtlougwuag.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.wangshuangyany.cn/gtelsvkmrd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hnqzz.top/gtinuzrech.html

[I07] 忽略大小写与多行模式
来源：http://hz.yuxming.cn/gthdwxmhqt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yangfankeji.com/gtrmzwyant.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.birdmap.top/gtdrvzyjju.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj20258.top/gtpneqjmfy.html

TS:   /error/gim
来源：http://hz.cdnleiting.top/gtqkqhgevx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.aizwys.cn/gtfgqbimpi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hnxiangtu.top/gtjiogkiut.html

Ruby: s.scan(/error/i)
来源：http://hz.cashguo.top/gtvloqszjl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jianghu66.top/gtxrvjbvwf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yanxiufei.cn/gtalvdjecw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ehwqpu.com/gtxsnyzshd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ivvv.top/gtdhlxbiuw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tian-w.cn/gtdzsqnbsw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gttbfffsmi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj20258.top/gtycdjrriv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cdnleiting.top/gteofnujss.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.dianchejie.cn/gtrtqatmtk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.aibaodan.cn/gtgwxeuevb.html

================================================================================
来源：http://hz.316326.xyz/gtynczrpnq.html

J. 日期与时间
来源：http://hz.vqdsnc.cn/gtgrktedkx.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gthrtlvwlf.html

[J01] 获取当前时间
来源：http://hz.nwbrower.top/gtsxmmbmnk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cdnleiting.top/gtvkmkzatd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinghuilouyu.cn/gthrotvsbk.html

JS:   new Date();  Date.now()
来源：http://hz.sweek.top/gtkyxmjijv.html

TS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gthejjktro.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ydjk.org.cn/gtszreqspi.html

Go:   time.Now()
来源：http://hz.zhongyouzk.top/gtlpmzfkjp.html

Ruby: Time.now
来源：http://hz.sysykeji.top/gtaejtpsvv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.daria6918.cn/gtmopizbcc.html

[J02] 格式化输出
来源：http://hz.yuxming.cn/gtihfegmps.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jiagoushi.top/gtqnwwmotb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shzxlz.cn/gtdeatwwxg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jqgufenzy.top/gthyxuaqeo.html

TS:   d.toISOString()
来源：http://hz.jinqigfzy.top/gtzgxyorid.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hammf.cn/gttxleqluv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hongshengwenyu.top/gtqhtsyfkn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtcatvyfia.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinyuanbaomall.cn/gtnsugyuij.html

[J03] 字符串解析为日期
来源：http://hz.yanxiufei.cn/gtcboqpagp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.nwbrower.top/gtlijpetxy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jyoumei.cn/gtovplqjds.html

JS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gthlfavjxm.html

TS:   new Date("2024-01-02")
来源：http://hz.fengsongda.top/gtqnumkdyf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jlsjyb.cn/gtbacjcvxi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hongshengwenyu.top/gtqzzmzovf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daxiang520.top/gtmivsadzr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gogol.net.cn/gtxuxuqcfe.html

[J04] 时间戳与日期互转
来源：http://hz.yuanzhike.top/gtgunqbkfx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dianchejie.cn/gtyxiplari.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sufxvd.cn/gtecjwpklt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tian-w.cn/gtsopsrjja.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sweek.top/gtanbstjmf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cheryme.top/gtlpzhurwv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tianlin.xyz/gtepvonoui.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.haohaochexian.top/gtfezyxnaa.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yuanzhike.top/gtezvclgej.html

[J05] 时间加减（加 7 天）
来源：http://hz.gzhubu.top/gtckfxdnzd.html

Py:   now + timedelta(days=7)
来源：http://hz.havefunace.top/gtwruoruzv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.iojbl.cn/gtgjqkuknk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xylfe.cn/gthsmkixrp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cheryme.top/gtmpgxgcxg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hysaishi.cn/gtwszmyitd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shanyushiyangtech.top/gtcjqanyyj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shuidangran.top/gtmkfnatqv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hammf.cn/gtlwmmrbyv.html

[J06] 计算两时间之差
来源：http://hz.hongshengwenyu.top/gtvbfsayag.html

Py:   (end - start).total_seconds()
来源：http://hz.wangdashe.top/gtlpnmtbdy.html

PHP:  $end->diff($start)->days;
来源：http://hz.ehwqpu.com/gtktgwcare.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.vqdsnc.cn/gtrkhnfrtj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cheryme.top/gtnfyutssc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.wangdashe.top/gtoofgbixu.html

Go:   end.Sub(start).Hours()
来源：http://hz.9152youxi.cn/gtjootskxy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.guannengcc.top/gtzaxbsarh.html

C#:   (end - start).TotalSeconds
来源：http://hz.zdqjudy.top/gtalhcpamc.html

[J07] 比较两个日期
来源：http://hz.shanyushiyangkeji.top/gtgeelynsk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangtech.top/gtnqegdhiv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangdashe.top/gtdtfnatfg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtcuudsxdn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gthdgucvna.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.quarkkingdee.top/gttlxfxubl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.andypj.xyz/gtkpxzqgpl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtesurobem.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtjniqkbhq.html

[J08] 提取年月日与星期
来源：http://hz.xuanzx.com/gthvwqpeen.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yuanzhike.top/gtkiimarel.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cdnleiting.top/gtentcxbgu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.guowangkeji.top/gtarfvvszb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yvedp.cn/gtcddpccjh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenzaomai.com/gteoctujft.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yueranfly.top/gtnrkvsbih.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xinyue.icu/gtdfdecpqj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shanyushiyangkeji.top/gtmplnkxpr.html

[J09] 时区处理
来源：http://hz.haohaochexian.top/gtlgceqzeu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.fzhhl.top/gtjxhkubxa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangdashe.top/gtbuoohsoo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guowangkeji.top/gthnqqxpio.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.mhx1999.top/gtdoootfnf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aibaodan.cn/gtskilmdtq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xziqi.cn/gtwgcvsczw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.aibaodan.cn/gttqupntxm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yonumen.top/gtogbzfrqg.html

[J10] 取今天 / 本月第一天
来源：http://hz.cdnleiting.top/gtoehqydel.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.dianchejie.cn/gtrdxmjojm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jlsjyb.cn/gtwojlsjue.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.fzhhl.top/gttthdzuaa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yangfankeji.com/gtunhkyuic.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.vqdsnc.cn/gttjqetukj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hywenlv.cn/gtdfqrjtsr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tianlin.xyz/gthxeksalb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.pycfn.com/gtsfszjllb.html

================================================================================
来源：http://hz.zdqjudy.top/gtyowtpxev.html

K. JSON 与序列化
来源：http://hz.jyoumei.cn/gtrunamnjg.html

================================================================================
来源：http://hz.chenzaomai.com/gtpglpqevo.html

[K01] 对象转 JSON 字符串
来源：http://hz.sysykeji.top/gtwfrbjohi.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.pengpengdd.cyou/gtgjwctbjy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shangyingyoupin.top/gtcfgxhacj.html

JS:   JSON.stringify(obj)
来源：http://hz.jyoumei.cn/gtllfivgyx.html

TS:   JSON.stringify(obj)
来源：http://hz.jinyuanbaomall.cn/gtgbeuhecj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.smart0.xyz/gtzllqydpq.html

Go:   json.Marshal(obj)
来源：http://hz.sweek.top/gtounjeygc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sysykeji.top/gtpmtditus.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daria6918.cn/gtwzprtepp.html

[K02] JSON 字符串转对象
来源：http://hz.ydzc1.top/gtzqjvfkqb.html

Py:   json.loads(s)
来源：http://hz.ydjk.org.cn/gtdpwkuywk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shangyingyoupin.top/gtbjnedzul.html

JS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtenlyearo.html

TS:   JSON.parse(s)
来源：http://hz.gzhubu.top/gtssebbwww.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.0kj1m.cn/gtecvpxnwk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xingfuxueyuan.xyz/gtctfnywgr.html

Ruby: JSON.parse(s)
来源：http://hz.svipenyu.cn/gtjdoiwbvc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ydjk.org.cn/gtocnthadi.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhengqikj.top/gtjrozhytw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.daxiang520.top/gtmuggnvxr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dianchejie.cn/gtqobtifwi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuanzhike.top/gttezkyezn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gaohongyu789.top/gttryrfdex.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.svipenyu.cn/gtkohznzev.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.fengsongda.top/gtipddhfyk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yanxiufei.cn/gtggvcxcut.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.fengsongda.top/gtiargekqy.html

[K04] 读取 JSON 文件
来源：http://hz.zhengqikj.top/gtdbxerjsd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cashguo.top/gturizysxy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangkeji.top/gtxexvrfcj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangdashe.top/gthlwfhoeo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenlongwang.top/gtsmjvwdwg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.guannengcc.top/gtbvxjkops.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenjidiqi.icu/gtbwhugnew.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tian-w.cn/gtoproeabi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cashguo.top/gttpeekgdh.html

[K05] 深拷贝对象
来源：http://hz.jqgfzy.top/gtpqhkvcxx.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxinkj.top/gtkgqpkvpy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ydzc1.top/gttwrdxkat.html

JS:   structuredClone(obj)
来源：http://hz.guannengcc.top/gtpllwwbnj.html

TS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtvljljxph.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sxryk.cn/gtizpppgdv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jiagoushi.top/gtenukeirw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shangyingyoupin.top/gttzdjblvu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cdnleiting.top/gtssmxhuid.html

[K06] 解析 URL 查询串
来源：http://hz.guannengcc.top/gtteblaqlp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ywan-chungtsiang.top/gtfxwrlzfq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jianghu66.top/gthdbgehkq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cucudq.cn/gtrzflpnml.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sufxvd.cn/gtelildjru.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.meibo888.top/gtpdlnofgb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cdnleiting.top/gtpjjuqrdd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tanke756.top/gtvmsnersf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.pycfn.com/gtwtknwmky.html

[K07] 进制转换
来源：http://hz.mhx1999.top/gturzeiqsy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hammf.cn/gtlcicvhkk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nanxuanxn.top/gtftzektjz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtuwruaugn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtymoudkkd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtdqrdbysh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.iojbl.cn/gtcmzfqpkv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenzaomai.com/gtnhwnwngy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinqigufen.top/gtrnzmgyzb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xylfe.cn/gtmdkzrsdr.html

Py:   pickle.dumps(obj)
来源：http://hz.316326.xyz/gtgxqunzjy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xuanzx.com/gtqfougrcn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtyaojhhus.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.bjfxy.top/gthmldvrwt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shuidangran.top/gtojervzac.html

Go:   encoding/gob
来源：http://hz.316326.xyz/gtebtxwflm.html

Ruby: Marshal.dump(obj)
来源：http://hz.hongshengwenyu.top/gtjdtwlpug.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fengsongda.top/gtgpjgltkn.html

================================================================================
来源：http://hz.daria6918.cn/gtupxbfkxb.html

L. 网络请求
来源：http://hz.yj202588.top/gthdyxsneg.html

================================================================================
来源：http://hz.gogol.net.cn/gtpybwgwru.html

[L01] 发送 GET 请求
来源：http://hz.andypj.xyz/gtssfpgbrp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nanxinkj.top/gtlpplfhuj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xinyue.icu/gtqxepidlc.html

JS:   await fetch(url)
来源：http://hz.ydjk.org.cn/gtrsxwaiql.html

TS:   await fetch(url)
来源：http://hz.yueranfly.top/gtitlprjzy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhixingplan.top/gtqefylsym.html

Go:   resp, err := http.Get(url)
来源：http://hz.sxryk.cn/gtcvdcpgko.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nwbrower.top/gtnaucpbhh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xingfuxueyuan.xyz/gtdqglfplv.html

[L02] 发送 POST JSON
来源：http://hz.wangdashe.top/gtfrrfbtlr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tanke756.top/gtdwxzopfh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shangyingyoupin.top/gtycnrbgje.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtiiwhubok.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhiwuduotai.top/gtokcubmqn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.havefunace.top/gtyhqyhkix.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hnxiangtu.top/gtlyyfvizj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guowangkeji.top/gtbsisasbi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigfzy.top/gtbpsgklda.html

[L03] 设置自定义请求头
来源：http://hz.zhengqikj.top/gtwqeuaznh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xingfuxueyuan.xyz/gtejsnzhax.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.havefunace.top/gtgyxzsdzt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aizwys.cn/gtmrzodiyi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhiwuduotai.top/gtbkksjojz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.smart0.xyz/gtbfmeqewx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sysykeji.top/gtpmjvybyo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj20258.top/gtmheoriad.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sweek.top/gtyyylyuyt.html

[L04] 设置超时
来源：http://hz.yuanzhike.top/gtuvpfgkch.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yuanzhike.top/gtuiablagg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jiagoushi.top/gtgahypqcj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gtuwuqdkxs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cheryme.top/gtlardpaxd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.chenlongwang.top/gtpsyhhbac.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.chenjidiqi.icu/gtvykznerz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinqigufen.top/gtmqtcwvfe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.kuanghao11.cn/gtgretfjdp.html

[L05] 上传文件（multipart）
来源：http://hz.cashguo.top/gtpyiuvfdf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jlsjyb.cn/gtiawzlaeh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jlsjyb.cn/gtnbkhpsdy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gtwzjwjoyb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sxryk.cn/gtkyqlwmnm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ppjwa.cn/gtjuwmfgzh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yueranfly.top/gtdwczhkvw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yongpay.top/gtbcmdcfqg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenzaomai.com/gtjhqezlrw.html

[L06] 解析响应为 JSON
来源：http://hz.guowangkeji.top/gthfwrtlop.html

Py:   resp.json()
来源：http://hz.kuanghao11.cn/gtcchwqlpa.html

PHP:  json_decode($body, true);
来源：http://hz.chenzaomai.com/gthebxleqy.html

JS:   await resp.json()
来源：http://hz.chenlongwang.top/gtzdqqxrxg.html

TS:   await resp.json()
来源：http://hz.ppjwa.cn/gtygyarfjg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinghuilouyu.cn/gtsshrciay.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.pengpengdd.cyou/gtustyfhwa.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cashguo.top/gtiupdugwt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tian-w.cn/gtumnfzfhs.html

[L07] 处理 HTTP 状态码
来源：http://hz.fzhhl.top/gtzcdipnia.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.aibaodan.cn/gtajlrmdel.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ydjk.org.cn/gtinemnwre.html

JS:   resp.ok;  resp.status
来源：http://hz.nanxuanxn.top/gthhwsenhn.html

TS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtewmksenh.html

Java: resp.statusCode()
来源：http://hz.gotoacloud.top/gtfbanasgp.html

Go:   resp.StatusCode
来源：http://hz.zdqjudy.top/gtgqfqtznd.html

Ruby: resp.code.to_i
来源：http://hz.0kj1m.cn/gttzedvjys.html

C#:   (int)resp.StatusCode
来源：http://hz.chenjidiqi.icu/gtkwgcownl.html

[L08] 并发请求多个地址
来源：http://hz.shzxlz.cn/gtjirauojc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ydjk.org.cn/gtxslarrtt.html

PHP:  curl_multi_init() 系列
来源：http://hz.tanke756.top/gtdfzmckvi.html


<!-- 参考信息 -->