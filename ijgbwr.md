代发 wailian999

================================================================================
来源：http://hz.shanyushiyangtech.top/gtvhnnnlyl.html

I. 正则表达式
来源：http://hz.hfpthk.cn/gtqsrilgxb.html

================================================================================
来源：http://hz.zdqjudy.top/gtljjcfnts.html

[I01] 判断是否匹配
来源：http://hz.sweek.top/gtgazmwskg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.nwbrower.top/gtadjjjirv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cucudq.cn/gtbcjsflit.html

JS:   /\d+/.test(s)
来源：http://hz.shanyushiyangtech.top/gtjperazaz.html

TS:   /\d+/.test(s)
来源：http://hz.gaohongyu789.top/gtectwjemc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.316326.xyz/gtxgzseizc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ppjwa.cn/gtofkclopm.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhongyouzk.top/gtplluzehn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xuanzx.com/gtrmqlygdy.html

[I02] 提取所有匹配
来源：http://hz.daxiang520.top/gtqynvqkpy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xinyue.icu/gtdrlgfjvo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.quarkkingdee.top/gtfmuzjezg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jlsjyb.cn/gttxmfacud.html

TS:   s.match(/\d+/g)
来源：http://hz.xziqi.cn/gtjcbqdrew.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hongshengwenyu.top/gtmwofmtse.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.vqdsnc.cn/gtnnawgijz.html

Ruby: s.scan(/\d+/)
来源：http://hz.smart0.xyz/gtdmquxzkd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yvedp.cn/gtlyajtnbt.html

[I03] 提取捕获分组
来源：http://hz.gzhubu.top/gtenqxnazm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jlsjyb.cn/gtllplzruj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yj20258888.top/gtymzznydg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hfpthk.cn/gtwbewunlf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ybcxt.top/gtljhydffd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gaohongyu789.top/gtqmmoexdn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxinkj.top/gthznfnaux.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinqigufen.top/gttygcfaji.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jlsjyb.cn/gtoohzqjqd.html

[I04] 正则替换
来源：http://hz.zycfv.cn/gtylsmlhog.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xinyue.icu/gthuyyvsfn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.haohaochexian.top/gtquebmzqi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gtyenmjgqc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.quarkkingdee.top/gtwjwvrppf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.mhx1999.top/gtvfcpvmxe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tanke756.top/gtrucbzqdz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinghuilouyu.cn/gtmascalbe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.quarkkingdee.top/gtpgpciqut.html

[I05] 按正则拆分
来源：http://hz.jyoumei.cn/gtpqtonrod.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.fengsongda.top/gtyxwilano.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hywenlv.cn/gtegbmbjpy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtnvwroukq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtzdeotzxr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.aizwys.cn/gtdlvgzwhx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.52xcode.cn/gtzvkfcedq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtdwcbaxmx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shzxlz.cn/gtqbaumcmf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.0kj1m.cn/gtdlcfvxwc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zdqjudy.top/gtyozdsjxw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ehwqpu.com/gtgzuczuix.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hongshengwenyu.top/gtedpdmotx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhengqikj.top/gtjmpsihfa.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.smart0.xyz/gtkzrfihtv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.meibo888.top/gtjewiilmv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhaomingkeji.xyz/gtjlroswqb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cdnleiting.top/gtovenlclx.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj202588.top/gtfsqylaxu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.9152youxi.cn/gtosgaogex.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cashguo.top/gtbpsjhmzc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sxryk.cn/gtvgindkbp.html

TS:   /error/gim
来源：http://hz.52xcode.cn/gtbvdremsz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hongshengwenyu.top/gtcbqoblni.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.dashuyun.cn/gttjhfeboe.html

Ruby: s.scan(/error/i)
来源：http://hz.jinghuilouyu.cn/gtzrecriqj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.aizwys.cn/gtlmpisxyl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hywenlv.cn/gtpffbbcfn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cashguo.top/gtuuxkpleq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yangfankeji.com/gtbaeiuitj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtxflvnkxg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ywan-chungtsiang.top/gtywhukghs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinyuanbaomall.cn/gtqpruswev.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hnqzz.top/gtfzktrowk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.daria6918.cn/gtsdfzwspx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cdnleiting.top/gttizbqdjp.html

================================================================================
来源：http://hz.zdqjudy.top/gtqsnfzeep.html

J. 日期与时间
来源：http://hz.yuanzhike.top/gtbzisdudr.html

================================================================================
来源：http://hz.mhx1999.top/gtjwkwshhd.html

[J01] 获取当前时间
来源：http://hz.pengpengdd.cyou/gtxyckbexs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.wangshuangyany.cn/gtkmssrlme.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zdqjudy.top/gtnxxbwcws.html

JS:   new Date();  Date.now()
来源：http://hz.0kj1m.cn/gtxymqvkdd.html

TS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gthfctafno.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sweek.top/gttuwpbekz.html

Go:   time.Now()
来源：http://hz.yj202588.top/gtvvpoipgi.html

Ruby: Time.now
来源：http://hz.dashuyun.cn/gtxcwgbbfe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yangfankeji.com/gtcxfkltip.html

[J02] 格式化输出
来源：http://hz.wangdashe.top/gtjhdwwgxy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xinyue.icu/gtvtcxaeci.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gzhubu.top/gteljkonwp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenzaomai.com/gtermrbhxz.html

TS:   d.toISOString()
来源：http://hz.yj202588.top/gtpdcigaqp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgfzy.top/gtlrsbfyat.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.9152youxi.cn/gtrivkqdrz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinghuilouyu.cn/gtgadqlhln.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.guowangkeji.top/gtjehebszk.html

[J03] 字符串解析为日期
来源：http://hz.ehwqpu.com/gtmdjumwoi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ivvv.top/gtsgafjrsh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xinyue.icu/gtoeqfohmf.html

JS:   new Date("2024-01-02")
来源：http://hz.jqgufenzy.top/gtrkspodzb.html

TS:   new Date("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtxdfqxrpk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nwbrower.top/gtltetmoej.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.c1oappe.top/gtugohlrbp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jqgfzy.top/gtkplhoyqd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sufxvd.cn/gtmyfcuxlc.html

[J04] 时间戳与日期互转
来源：http://hz.hfpthk.cn/gtizdvzoju.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shuidangran.top/gtqabwaxxe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jianghu66.top/gtcrigumpq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.smart0.xyz/gtjssecgng.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dianchejie.cn/gtatbbjxwa.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jqgufenzy.top/gtzfcwywpy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.smart0.xyz/gtircdkjmi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenjidiqi.icu/gtawdvyjsi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hywenlv.cn/gtcsrzqysd.html

[J05] 时间加减（加 7 天）
来源：http://hz.jyoumei.cn/gtvemqsttz.html

Py:   now + timedelta(days=7)
来源：http://hz.hywenlv.cn/gtkfsmexcj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhoulong.xyz/gtuvuoxnar.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hongshengwenyu.top/gtxfsotuqq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sufxvd.cn/gtgfsvtjci.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.dianchejie.cn/gtnvdrhicn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ydjk.org.cn/gtrtybhgcd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydjk.org.cn/gthcdotsao.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhijiandao.cn/gtjixhvmwu.html

[J06] 计算两时间之差
来源：http://hz.zhijiandao.cn/gtgehclsmp.html

Py:   (end - start).total_seconds()
来源：http://hz.ehwqpu.com/gteysoalbl.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhoulong.xyz/gtsjfbwwgz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nanxinkj.top/gtjedyzafz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj20258.top/gtfwxdgrhi.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinqigfzy.top/gtwmsoqblu.html

Go:   end.Sub(start).Hours()
来源：http://hz.aibaodan.cn/gtbctvvkse.html

Ruby: end - start                 # 返回秒数
来源：http://hz.guannengcc.top/gtwynoyxeg.html

C#:   (end - start).TotalSeconds
来源：http://hz.shanyushiyangkeji.top/gtsvwlayei.html

[J07] 比较两个日期
来源：http://hz.xinyue.icu/gtkttmkkga.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtponrlxgi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dashuyun.cn/gtbubkcxnq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ywan-chungtsiang.top/gtkaopppbd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cheryme.top/gtiprppyaq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shzxlz.cn/gtdptnfvne.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinqigfzy.top/gtozkxeejw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gtbxnswgqk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtdrrvvctx.html

[J08] 提取年月日与星期
来源：http://hz.dianchejie.cn/gteblureuf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenzaomai.com/gtmoympchf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jianghu66.top/gtppczjugj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aibaodan.cn/gtoskpufsk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.daxiang520.top/gtnhallajc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yuanzhike.top/gtilokfczy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ywan-chungtsiang.top/gtxohftpcw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yueranfly.top/gtcnthryuj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinyuanbaomall.cn/gtnazcnpvl.html

[J09] 时区处理
来源：http://hz.yj20258888.top/gthldueujy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.andypj.xyz/gtlbeiwshz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.iojbl.cn/gtgaxrjzau.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigfzy.top/gtuksoddck.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xingfuxueyuan.xyz/gtednvblnp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yuxming.cn/gtlduovkpi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sweek.top/gtsjbwsrcv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jianghu66.top/gtupgakwsw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.feifeiyinyue.top/gtqwbbnboi.html

[J10] 取今天 / 本月第一天
来源：http://hz.kuanghao11.cn/gtggewgmly.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinqigfzy.top/gtizydwopl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yanxiufei.cn/gthszdtuul.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhoulong.xyz/gtywistsbp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hfpthk.cn/gtebnofysy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jianghu66.top/gtlgwfyvfm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tian-w.cn/gtooamektd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.wangdashe.top/gtabujyfqc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.pengpengdd.cyou/gtijraftjd.html

================================================================================
来源：http://hz.gaohongyu789.top/gtpnrhhltr.html

K. JSON 与序列化
来源：http://hz.cheryme.top/gtycbvloxc.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtqdduvlfq.html

[K01] 对象转 JSON 字符串
来源：http://hz.shanyushiyangtech.top/gtxyumkoji.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sufxvd.cn/gtlepxiqfh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydjk.org.cn/gtkeeoctba.html

JS:   JSON.stringify(obj)
来源：http://hz.svipenyu.cn/gtiipwarxd.html

TS:   JSON.stringify(obj)
来源：http://hz.andypj.xyz/gtdsmovkaj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jqgfzy.top/gtsxxjshpr.html

Go:   json.Marshal(obj)
来源：http://hz.xinyue.icu/gtbjhcpqop.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhixingplan.top/gthlgfkbtq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.bjfxy.top/gtsxkdxkoc.html

[K02] JSON 字符串转对象
来源：http://hz.hnxiangtu.top/gtkqhfspqk.html

Py:   json.loads(s)
来源：http://hz.ybcxt.top/gtqpalqtue.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zycfv.cn/gtfrwknzal.html

JS:   JSON.parse(s)
来源：http://hz.jiagoushi.top/gtsbpaakhi.html

TS:   JSON.parse(s)
来源：http://hz.smart0.xyz/gtbaspzzmd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.chenzaomai.com/gtqebekizb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yanxiufei.cn/gtvcqoskcf.html

Ruby: JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtxdpsgvux.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.snrcjt.cn/gtawecfqyp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.daria6918.cn/gttntegocn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj20258888.top/gtiyphfxbt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ehwqpu.com/gtrnweipqe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gzhubu.top/gtvtzqihnl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnxiangtu.top/gttrqxklyl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dianchejie.cn/gtxlcesqtl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.316326.xyz/gtghmoqmyp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sweek.top/gtjnxtjajg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuanzhike.top/gtrrftexwg.html

[K04] 读取 JSON 文件
来源：http://hz.smart0.xyz/gtcrhbvpwl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.daria6918.cn/gtjzkqkrng.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gotoacloud.top/gtvuorgbbq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tanke756.top/gtfktalofv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xingfuxueyuan.xyz/gtdtgzuesn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ydzc1.top/gtxwbbruno.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yj20258888.top/gtijquentv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.feifeiyinyue.top/gtbnnlehcz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dashuyun.cn/gtejqlqffv.html

[K05] 深拷贝对象
来源：http://hz.c1oappe.top/gtejqhfuut.html

Py:   copy.deepcopy(obj)
来源：http://hz.ppjwa.cn/gtzcxfzmih.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cheryme.top/gtiwcexzby.html

JS:   structuredClone(obj)
来源：http://hz.jyoumei.cn/gtnpxtzkcv.html

TS:   structuredClone(obj)
来源：http://hz.jlsjyb.cn/gtmtogcknk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gzhubu.top/gtykxsjehz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jlsjyb.cn/gtceloikjt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.dashuyun.cn/gtziopwkej.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.iojbl.cn/gtcityrpuq.html

[K06] 解析 URL 查询串
来源：http://hz.iojbl.cn/gturvxsjbq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhongyouzk.top/gtmxmgpyit.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sxryk.cn/gtxcfowost.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cashguo.top/gtolzirtsf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dianchejie.cn/gtvttavryw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.gogol.net.cn/gttexguvid.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hnqzz.top/gtxlxkqodj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tianlin.xyz/gtyczwhqyi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxinkj.top/gtgwrcogip.html

[K07] 进制转换
来源：http://hz.yueranfly.top/gtmcymzdts.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gaohongyu789.top/gtkpbrlfxm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sufxvd.cn/gtzadpcnhr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtaahcewhn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gttxetsbpu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.kuanghao11.cn/gtogwfeuhj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cashguo.top/gtyjdgrfdg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shzxlz.cn/gtymcvgwik.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.316326.xyz/gtgifbvfkf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.pengpengdd.cyou/gtztmnpfko.html

Py:   pickle.dumps(obj)
来源：http://hz.gogol.net.cn/gtsktunraz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.pycfn.com/gtmigcboom.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtzsqkyidl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gaohongyu789.top/gtwufbwyyc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xingfuxueyuan.xyz/gtkcpztrcz.html

Go:   encoding/gob
来源：http://hz.xuanzx.com/gtbqmhfhdw.html

Ruby: Marshal.dump(obj)
来源：http://hz.xylfe.cn/gtgrbpnkfk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.haohaochexian.top/gtkyzevxmd.html

================================================================================
来源：http://hz.cdnleiting.top/gtmsbmjprs.html

L. 网络请求
来源：http://hz.andypj.xyz/gtghfmjsvy.html

================================================================================
来源：http://hz.sysykeji.top/gtkspwpmpe.html

[L01] 发送 GET 请求
来源：http://hz.jqgfzy.top/gtccihkqqf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gotoacloud.top/gtjtmnwtss.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.haohaochexian.top/gtuhufnikq.html

JS:   await fetch(url)
来源：http://hz.aibaodan.cn/gtrwakfbuj.html

TS:   await fetch(url)
来源：http://hz.52xcode.cn/gtrzvsmalw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yanxiufei.cn/gtymhrwcxu.html

Go:   resp, err := http.Get(url)
来源：http://hz.ywan-chungtsiang.top/gtqkhdvhwy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hammf.cn/gtmcghtblj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.pengpengdd.cyou/gtmxmwaeqe.html

[L02] 发送 POST JSON
来源：http://hz.cheryme.top/gtvvyocnyt.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xuanzx.com/gtjmpysooe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fengsongda.top/gttqmlnjfh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydjk.org.cn/gtddbjvqhz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhiwuduotai.top/gtfzrvpbem.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.quarkkingdee.top/gtkwncxrrd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.dianchejie.cn/gtlyyisome.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cdnleiting.top/gtnbigsafc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.9152youxi.cn/gtxxeyzbau.html

[L03] 设置自定义请求头
来源：http://hz.zdqjudy.top/gtomgbtfoc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nwbrower.top/gtdcloaepy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gogol.net.cn/gtarqcsyqt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.c1oappe.top/gtraeeuwnh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.iojbl.cn/gtgclcfbfi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.52xcode.cn/gttjwsrsdx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.meibo888.top/gtwrdesewk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xinyue.icu/gtuilblpup.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuxming.cn/gtdmytjgsy.html

[L04] 设置超时
来源：http://hz.tianlin.xyz/gtcuqbfmzj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xziqi.cn/gtvqstnkll.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xziqi.cn/gtdmpjafua.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenzaomai.com/gttshtavyd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtysucvusm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhoulong.xyz/gtcaaqivjz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.svipenyu.cn/gtufssyjun.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tanke756.top/gtaupuqlrh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuetiantiany.cn/gtssklrvdw.html

[L05] 上传文件（multipart）
来源：http://hz.meibo888.top/gttojsielu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sweek.top/gtgpkctwmx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yonumen.top/gtrbxvksuj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sweek.top/gtelndlygd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258.top/gttvevbyau.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shanyushiyangtech.top/gtzlpfizgt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ywan-chungtsiang.top/gtxbvlxnyp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shuidangran.top/gteufyikew.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinghuilouyu.cn/gtkzqhobra.html

[L06] 解析响应为 JSON
来源：http://hz.meibo888.top/gtocrqqtub.html

Py:   resp.json()
来源：http://hz.jyoumei.cn/gtwdhqniff.html

PHP:  json_decode($body, true);
来源：http://hz.tianlin.xyz/gtnojbyhuq.html

JS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtfrzusufu.html

TS:   await resp.json()
来源：http://hz.gogol.net.cn/gtkszuqbto.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhengqikj.top/gtdwyyjenj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.fengsongda.top/gtqemvjsrd.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ywan-chungtsiang.top/gtpottarem.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cqqwz.cn/gtpzhqbfxh.html


<!-- 参考信息 -->