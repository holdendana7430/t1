代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.daria6918.cn/gtazvropbw.html

Go:   defer f.Close()
来源：http://hz.pengpengdd.cyou/gtyouzvzjc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ybcxt.top/gtujfmfqig.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.316326.xyz/gtxnsioxsr.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtponqqzzq.html

I. 正则表达式
来源：http://hz.havefunace.top/gtxjrxilxy.html

================================================================================
来源：http://hz.sufxvd.cn/gtygnphalg.html

[I01] 判断是否匹配
来源：http://hz.vqdsnc.cn/gtbftqnske.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhixingplan.top/gtphqhjdxx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shangyingyoupin.top/gtdlzsnvvx.html

JS:   /\d+/.test(s)
来源：http://hz.sufxvd.cn/gtejztvmtm.html

TS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gthlygxlyo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.pengpengdd.cyou/gtujvpwvus.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.wangdashe.top/gtfdgfrqah.html

Ruby: s.match?(/\d+/)
来源：http://hz.cucudq.cn/gtgnmzwxiq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yongpay.top/gtnuuqtazz.html

[I02] 提取所有匹配
来源：http://hz.hongshengwenyu.top/gtudapwckq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hywenlv.cn/gtwmdhzvyw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.tian-w.cn/gtyezojjfs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xingfuxueyuan.xyz/gtrmkdzbbv.html

TS:   s.match(/\d+/g)
来源：http://hz.9152youxi.cn/gtnbavorhy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ppjwa.cn/gtjkaonshq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.0kj1m.cn/gtshrxmxly.html

Ruby: s.scan(/\d+/)
来源：http://hz.shanyushiyangkeji.top/gtcqgjkcsf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.haohaochexian.top/gtpxatauwk.html

[I03] 提取捕获分组
来源：http://hz.0kj1m.cn/gtvuwirdsr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ehwqpu.com/gtsqlvslsi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xuetiantiany.cn/gtpuqhulcs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.daxiang520.top/gtutkeregj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shanyushiyangtech.top/gtzidwbhqr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.wangdashe.top/gtllvtfjts.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.svipenyu.cn/gtrajtptgo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hnxiangtu.top/gtjmdgppfl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhoulong.xyz/gtvpsdikdz.html

[I04] 正则替换
来源：http://hz.haohaochexian.top/gtoqfymgyu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yuxming.cn/gtydvzbfon.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinghuilouyu.cn/gtfcegajuo.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtjhzoqqlc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.nwbrower.top/gtcuadtnal.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenlongwang.top/gtrccfbxfe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cheryme.top/gtiyguedzd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.fzhhl.top/gtqigrmegw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xuanzx.com/gtotiprewt.html

[I05] 按正则拆分
来源：http://hz.jqgufenzy.top/gtftycopvs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xuanzx.com/gtduaqtfhu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gotoacloud.top/gtpqyssqwa.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.aibaodan.cn/gtlocvbequ.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtihtyzlxt.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hfpthk.cn/gtxghmoirx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yanxiufei.cn/gtuvtussug.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtsmwtjykn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinqigufen.top/gtwfbbiyzc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.9152youxi.cn/gtxfanodpm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtrjuzdist.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yanxiufei.cn/gtgrftfnaw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangtech.top/gtgiquurol.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sysykeji.top/gtbbvvtsgv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jlsjyb.cn/gtmkzpeydl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhaomingkeji.xyz/gtzyvjinyb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xingfuxueyuan.xyz/gtmcmkluks.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cheryme.top/gtvpldsizc.html

[I07] 忽略大小写与多行模式
来源：http://hz.iojbl.cn/gtbwvqarbm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sxryk.cn/gtdmqodtzw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhaomingkeji.xyz/gthxbzcefr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.haohaochexian.top/gtwhjbxdvt.html

TS:   /error/gim
来源：http://hz.fzhhl.top/gtwegjgtdk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.9152youxi.cn/gtmgzaggww.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhaomingkeji.xyz/gtthpeoqwo.html

Ruby: s.scan(/error/i)
来源：http://hz.hongshengwenyu.top/gtnwxeugvc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gaohongyu789.top/gtenhmjlyg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj20258888.top/gtpdbqsvhr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.snrcjt.cn/gtwxnfsnuj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhoulong.xyz/gtnzwismgh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ybcxt.top/gtlrnqgbcw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuanzhike.top/gtyzsfxbst.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.smart0.xyz/gttvlfccyu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuetiantiany.cn/gtkoafxzyo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinqigfzy.top/gtiitayxlc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xuetiantiany.cn/gtzjssrjoz.html

================================================================================
来源：http://hz.dianchejie.cn/gteulmwmrl.html

J. 日期与时间
来源：http://hz.xylfe.cn/gtvadcbkbm.html

================================================================================
来源：http://hz.hysaishi.cn/gtbvuxzzfo.html

[J01] 获取当前时间
来源：http://hz.haohaochexian.top/gtfzadopgb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yvedp.cn/gtgotdotdb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gaohongyu789.top/gtupxpifel.html

JS:   new Date();  Date.now()
来源：http://hz.316326.xyz/gtczhgkntb.html

TS:   new Date();  Date.now()
来源：http://hz.svipenyu.cn/gtkkdbmwxe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhiwuduotai.top/gtcovybnae.html

Go:   time.Now()
来源：http://hz.jyoumei.cn/gtxavusdpe.html

Ruby: Time.now
来源：http://hz.jqgufenzy.top/gtipwipuda.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.daxiang520.top/gtvzombzqj.html

[J02] 格式化输出
来源：http://hz.zdqjudy.top/gtehbhxjzy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hfpthk.cn/gttivqanpb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhoulong.xyz/gtenzrajxo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sufxvd.cn/gtxkzvauvp.html

TS:   d.toISOString()
来源：http://hz.dashuyun.cn/gtckfguxis.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yuanzhike.top/gtbelnxlna.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cheryme.top/gtpjfgrshb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ppjwa.cn/gtmxndawdk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.andypj.xyz/gtavutephc.html

[J03] 字符串解析为日期
来源：http://hz.zdqjudy.top/gtxbhevksz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.havefunace.top/gtccrxtmvc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sysykeji.top/gtpvjbzpeu.html

JS:   new Date("2024-01-02")
来源：http://hz.ybcxt.top/gtngggjgtp.html

TS:   new Date("2024-01-02")
来源：http://hz.chenzaomai.com/gtnhabqtxi.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhongyouzk.top/gtuttongui.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.316326.xyz/gtxeeqktly.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sxryk.cn/gtzcfnskew.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hfpthk.cn/gtpacjuaap.html

[J04] 时间戳与日期互转
来源：http://hz.ydjk.org.cn/gtaeflpumf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.svipenyu.cn/gtuiohtuwf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hammf.cn/gtjgcwcmoj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhoulong.xyz/gtlddgvbzd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hnqzz.top/gtkzdhfbww.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hfpthk.cn/gtpbdvogoj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yanxiufei.cn/gtgdtzydpk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.mhx1999.top/gtxyertqvx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cashguo.top/gtdhrewloi.html

[J05] 时间加减（加 7 天）
来源：http://hz.vqdsnc.cn/gtsjbbygja.html

Py:   now + timedelta(days=7)
来源：http://hz.ydzc1.top/gtrbdhbnbu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xingfuxueyuan.xyz/gtpokaghiu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydjk.org.cn/gtynssonqg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sxryk.cn/gtfcuqmqyz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhongyouzk.top/gtoxpauypz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yj202588.top/gtnrdldkyg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gaohongyu789.top/gtprjicbxq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.birdmap.top/gttajumrqi.html

[J06] 计算两时间之差
来源：http://hz.cucudq.cn/gtbhospete.html

Py:   (end - start).total_seconds()
来源：http://hz.kuanghao11.cn/gtsryleqbl.html

PHP:  $end->diff($start)->days;
来源：http://hz.yvedp.cn/gtigtmqvkf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zdqjudy.top/gtpzuimomx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shuidangran.top/gtiznhhmpu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hysaishi.cn/gtksgpjvcc.html

Go:   end.Sub(start).Hours()
来源：http://hz.kuanghao11.cn/gtrzjbqbzt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yanxiufei.cn/gtfitlwryo.html

C#:   (end - start).TotalSeconds
来源：http://hz.aibaodan.cn/gthfwqtgyb.html

[J07] 比较两个日期
来源：http://hz.andypj.xyz/gtcsjbokgn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtaekvjcsq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cucudq.cn/gtgdyahoce.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhaomingkeji.xyz/gtzcofiesw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtjsrjpkhc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cqqwz.cn/gtbqqlbvtx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jqgufenzy.top/gtsjyphzrm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtxfdfzqom.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jyoumei.cn/gtibakwksi.html

[J08] 提取年月日与星期
来源：http://hz.hongshengwenyu.top/gthkatvbfd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xziqi.cn/gtcunbzfjl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ywan-chungtsiang.top/gtqqlbktds.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jyoumei.cn/gtinoayyyz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gotoacloud.top/gtcepeuyhh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xingfuxueyuan.xyz/gtgdiocssr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhiwuduotai.top/gtivlfweei.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.guowangkeji.top/gtnfcpjrfp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhiwuduotai.top/gtvigwbxra.html

[J09] 时区处理
来源：http://hz.meibo888.top/gtwkinnush.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gogol.net.cn/gtwrnzdftn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.dianchejie.cn/gtvryerqet.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gotoacloud.top/gtxatmyqoy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tianlin.xyz/gtwwxtggox.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xingfuxueyuan.xyz/gtnvcmjxuz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sweek.top/gtavrjpdmq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jianghu66.top/gtbejcwziq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.havefunace.top/gtdczakhog.html

[J10] 取今天 / 本月第一天
来源：http://hz.hywenlv.cn/gtyjbkdpyl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shzxlz.cn/gtzgyvrtvl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhixingplan.top/gtqmungtst.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yuxming.cn/gtxjgvgovr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jiagoushi.top/gtgdqopobg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.snrcjt.cn/gtcdmohfpg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinqigufen.top/gthxwnloft.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.wangshuangyany.cn/gtnuxzlsvg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ppjwa.cn/gtssffkbqo.html

================================================================================
来源：http://hz.zycfv.cn/gtxvogztmw.html

K. JSON 与序列化
来源：http://hz.daria6918.cn/gtibsluuye.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtjzimxcty.html

[K01] 对象转 JSON 字符串
来源：http://hz.feifeiyinyue.top/gtnigbxadj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xingfuxueyuan.xyz/gtxuweelfv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zycfv.cn/gtldalbgqd.html

JS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtpbwxdvpb.html

TS:   JSON.stringify(obj)
来源：http://hz.hongshengwenyu.top/gtzcvlwwsr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yueranfly.top/gtbdqokpuy.html

Go:   json.Marshal(obj)
来源：http://hz.nanxuanxn.top/gtikeusmtp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.guannengcc.top/gtituszoyo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daxiang520.top/gtshlnhzyb.html

[K02] JSON 字符串转对象
来源：http://hz.ydzc1.top/gtlvjsuthq.html

Py:   json.loads(s)
来源：http://hz.cheryme.top/gtdoeueddk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.quarkkingdee.top/gtdqhmlmhq.html

JS:   JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gtmstbyxqh.html

TS:   JSON.parse(s)
来源：http://hz.52xcode.cn/gtotqurwdp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.c1oappe.top/gtxcxecrrl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gthidbxblo.html

Ruby: JSON.parse(s)
来源：http://hz.jiagoushi.top/gthbkuxlwj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yonumen.top/gtmsgzfuhm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tian-w.cn/gtlodgaalf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtmauyaqga.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gaohongyu789.top/gtqvdnmpvy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigfzy.top/gtrwsdtqca.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.9152youxi.cn/gtsbmvdarm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nwbrower.top/gtetwyznld.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cucudq.cn/gtclmnuwxt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinyuanbaomall.cn/gtxrwnkoio.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.pycfn.com/gtqhqcypmp.html

[K04] 读取 JSON 文件
来源：http://hz.ehwqpu.com/gtstjknxpc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sweek.top/gtwwpmzglq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.dashuyun.cn/gtwizemmvr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgufenzy.top/gteshbxpbg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xingfuxueyuan.xyz/gtzwqbaosp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.316326.xyz/gttnxskavl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nanxuanxn.top/gtwkjfatfg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ydjk.org.cn/gtychwtore.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.bjfxy.top/gtijvkmzxc.html

[K05] 深拷贝对象
来源：http://hz.ydzc1.top/gtvoraurgt.html

Py:   copy.deepcopy(obj)
来源：http://hz.shanyushiyangtech.top/gtxdcjvnld.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hongshengwenyu.top/gthyypqtmz.html

JS:   structuredClone(obj)
来源：http://hz.pycfn.com/gtsyzmrjwh.html

TS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtznexwoik.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cheryme.top/gtjepwcjrp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.bjfxy.top/gtlavedhal.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sysykeji.top/gtqdvjwqws.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shanyushiyangkeji.top/gtlnazsxhi.html

[K06] 解析 URL 查询串
来源：http://hz.yanxiufei.cn/gtccztkvjv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.daxiang520.top/gtghbszrqk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yvedp.cn/gtakytuvog.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yangfankeji.com/gtbiasyrsk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jyoumei.cn/gtxpkhrrks.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhengqikj.top/gtgvradwon.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.0kj1m.cn/gtfrfgwstk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtjswtdriv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.aizwys.cn/gtgkbvbllk.html

[K07] 进制转换
来源：http://hz.jinqigfzy.top/gtnuxjsnjr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenjidiqi.icu/gtnyhbzdfv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.andypj.xyz/gtswjgamip.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtuxgeywmv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cashguo.top/gtpowekvuh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtmstkyjyg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sufxvd.cn/gtokwnkask.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.kuanghao11.cn/gtvsfaoijx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.wangdashe.top/gtyoiwpocw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sweek.top/gtkeffldhj.html

Py:   pickle.dumps(obj)
来源：http://hz.ydjk.org.cn/gtunlfxdvc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ydzc1.top/gthgsvahbp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258.top/gtuqnfqmvg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xuetiantiany.cn/gtvldnymlh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.snrcjt.cn/gtzjtybxvd.html

Go:   encoding/gob
来源：http://hz.jqgufenzy.top/gtlrmuhlih.html

Ruby: Marshal.dump(obj)
来源：http://hz.hnxiangtu.top/gtjwbitess.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.snrcjt.cn/gtlmaykidk.html

================================================================================
来源：http://hz.zdqjudy.top/gtbilqdefx.html

L. 网络请求
来源：http://hz.sweek.top/gthsptqova.html

================================================================================
来源：http://hz.guannengcc.top/gtxxycpfio.html

[L01] 发送 GET 请求
来源：http://hz.zhixingplan.top/gtrhdffetw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenlongwang.top/gtpwvhrbyj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258.top/gtowcwmqfh.html

JS:   await fetch(url)
来源：http://hz.vqdsnc.cn/gtnhvakrqm.html

TS:   await fetch(url)
来源：http://hz.gotoacloud.top/gtcdwbjwza.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.c1oappe.top/gtlyonggym.html

Go:   resp, err := http.Get(url)
来源：http://hz.tian-w.cn/gtfppqidyc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.bjfxy.top/gtideitkfi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ehwqpu.com/gtihxmrogw.html

[L02] 发送 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtzqkyjjwf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guowangkeji.top/gtwolfuzwk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.9152youxi.cn/gtgeojpatz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxinkj.top/gtzmvyzjfg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guowangkeji.top/gtyulzuwtv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guannengcc.top/gtgxwhfcyb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sxryk.cn/gtjgquzhad.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.mhx1999.top/gtyfupdnbh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ywan-chungtsiang.top/gtgpnnejei.html

[L03] 设置自定义请求头
来源：http://hz.cdnleiting.top/gtgpzqrozo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhengqikj.top/gtelckdvde.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinqigfzy.top/gttrtneuam.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxuanxn.top/gtogktnxne.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hfpthk.cn/gtuqeisufj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.kuanghao11.cn/gtvatuchmb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shangyingyoupin.top/gtkgmngpzq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hysaishi.cn/gtwytglctd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hongshengwenyu.top/gtetddjftd.html

[L04] 设置超时
来源：http://hz.jqgufenzy.top/gtxpvrrfgx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.guowangkeji.top/gtfbftbfgh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jyoumei.cn/gtjvvynuys.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ivvv.top/gtbjfdeylj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtwylveyvr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.shanyushiyangtech.top/gtxvlupoom.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.havefunace.top/gtpcofzgdz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xylfe.cn/gtxhefcrfb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cashguo.top/gtfgjfeopl.html

[L05] 上传文件（multipart）
来源：http://hz.shuidangran.top/gtgsnxocwh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhongyouzk.top/gtensbmwga.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sufxvd.cn/gtgliizsyd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shzxlz.cn/gtpmoiqyiu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258.top/gtrkfssdxe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ywan-chungtsiang.top/gtiwnmhnot.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dianchejie.cn/gtxtwaakow.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.wangdashe.top/gtqtauzbuu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jyoumei.cn/gtffhmufuq.html

[L06] 解析响应为 JSON
来源：http://hz.hnxiangtu.top/gtwugiwtud.html

Py:   resp.json()
来源：http://hz.sysykeji.top/gtqdpyrxwa.html

PHP:  json_decode($body, true);
来源：http://hz.xingfuxueyuan.xyz/gtljbcrvpy.html

JS:   await resp.json()
来源：http://hz.zhoulong.xyz/gtxuxhmprg.html

TS:   await resp.json()
来源：http://hz.gogol.net.cn/gtcmgsbrdo.html


<!-- 参考信息 -->