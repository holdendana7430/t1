代发 wailian999

[I02] 提取所有匹配
来源：http://hz.daxiang520.top/gttxfzkxvu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.meibo888.top/gtcxoiupse.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangkeji.top/gtxfcwuofl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.svipenyu.cn/gtaxplprho.html

TS:   s.match(/\d+/g)
来源：http://hz.tianlin.xyz/gtkhhpoxoj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhengqikj.top/gtnlfoifuj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yongpay.top/gtmjdbvqpl.html

Ruby: s.scan(/\d+/)
来源：http://hz.tian-w.cn/gtzhasjugc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj20258.top/gtnkaqwwqf.html

[I03] 提取捕获分组
来源：http://hz.fzhhl.top/gtshbfbirv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shangyingyoupin.top/gtgwaflhyc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.feifeiyinyue.top/gtmnycbgpo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jiagoushi.top/gtgmiedrak.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cucudq.cn/gtjekcxjtf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xingfuxueyuan.xyz/gtuudsigbu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gotoacloud.top/gtrvdydvxc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sysykeji.top/gtqdzpaplv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cashguo.top/gtntkcodtp.html

[I04] 正则替换
来源：http://hz.yj202588.top/gtbwjlpjdv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.wangshuangyany.cn/gtdwcebzfo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.haohaochexian.top/gtopevozgu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.iojbl.cn/gtuxftzhcq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sysykeji.top/gtrmjyaxbq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.aibaodan.cn/gtjirrbyix.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yongpay.top/gtikbwikzj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hysaishi.cn/gtkghnqnbe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hnxiangtu.top/gtubrqnfsw.html

[I05] 按正则拆分
来源：http://hz.jqgfzy.top/gtxjgsgupd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hywenlv.cn/gttgahcizj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.dashuyun.cn/gtrxxieakz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtdnophwek.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtrypllest.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sxryk.cn/gthwmdpimi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hnxiangtu.top/gtafbfuycr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtkktjzmuq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.pengpengdd.cyou/gthzkikhbx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xziqi.cn/gttjcrumpb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xuetiantiany.cn/gtehuaweqk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.vqdsnc.cn/gtqzrxvbso.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gzhubu.top/gtgvphfccd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gteypaijsm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.smart0.xyz/gtifbcsoek.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenzaomai.com/gtqrtdqdjo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hfpthk.cn/gtzgxixtcz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.guowangkeji.top/gtnizxxpik.html

[I07] 忽略大小写与多行模式
来源：http://hz.tian-w.cn/gtnedotobc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.haohaochexian.top/gtslomcbyl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhongyouzk.top/gtcubowjel.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.guannengcc.top/gtpyfnwhco.html

TS:   /error/gim
来源：http://hz.hysaishi.cn/gtlgjtjcfa.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nanxuanxn.top/gtxmjjejgt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shanyushiyangkeji.top/gtejynzbus.html

Ruby: s.scan(/error/i)
来源：http://hz.ivvv.top/gtdqdohhlg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.havefunace.top/gtfxmmoiha.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shanyushiyangtech.top/gthkyafgta.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guannengcc.top/gtcdlnvisd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cashguo.top/gtehpofdts.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yueranfly.top/gtowcxvbyl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.smart0.xyz/gtlbzbddcp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.iojbl.cn/gtamnlvfcu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinqigfzy.top/gtdebbfbon.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gzhubu.top/gtgevkhncn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.wangshuangyany.cn/gtstdooltq.html

================================================================================
来源：http://hz.jinqigfzy.top/gtskkpkekc.html

J. 日期与时间
来源：http://hz.hnxiangtu.top/gtashfymkt.html

================================================================================
来源：http://hz.yvedp.cn/gtbfrdpalo.html

[J01] 获取当前时间
来源：http://hz.smart0.xyz/gtcnexveow.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hfpthk.cn/gtxuxwqgpg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.0kj1m.cn/gtvilyrqwg.html

JS:   new Date();  Date.now()
来源：http://hz.guowangkeji.top/gtkryjsvkd.html

TS:   new Date();  Date.now()
来源：http://hz.jqgufenzy.top/gtsfpmqhhm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ydjk.org.cn/gtohxydziu.html

Go:   time.Now()
来源：http://hz.tanke756.top/gtxincnoit.html

Ruby: Time.now
来源：http://hz.bjfxy.top/gtlwmfvony.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.9152youxi.cn/gtofqgbwnb.html

[J02] 格式化输出
来源：http://hz.shuidangran.top/gtqcbraymy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yvedp.cn/gtxyypswwe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gtbhbddwna.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenzaomai.com/gtslapxqxb.html

TS:   d.toISOString()
来源：http://hz.jinqigufen.top/gtnggskuhz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.wangshuangyany.cn/gtoqvhmlmy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.svipenyu.cn/gtcthbtdke.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgufenzy.top/gtgyjwveoi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xziqi.cn/gtceycrgli.html

[J03] 字符串解析为日期
来源：http://hz.kuanghao11.cn/gtkebffikm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yj20258888.top/gtmrchrpjk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhongyouzk.top/gtipfgrsyq.html

JS:   new Date("2024-01-02")
来源：http://hz.hywenlv.cn/gthszygsjq.html

TS:   new Date("2024-01-02")
来源：http://hz.hammf.cn/gtvwktihhf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.svipenyu.cn/gtlflpzqso.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shuidangran.top/gtfycsuyde.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtistfkuyg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.havefunace.top/gtcrpuypgp.html

[J04] 时间戳与日期互转
来源：http://hz.sufxvd.cn/gtypohgxvc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.fengsongda.top/gtvpsczpfd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yj202588.top/gtduqxcyds.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sysykeji.top/gttrkenrbb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zycfv.cn/gtqemvxvkw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cdnleiting.top/gtjrtsyyfc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shuidangran.top/gtashxtbqz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yanxiufei.cn/gtzqqpfvoe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nanxuanxn.top/gtprpvslri.html

[J05] 时间加减（加 7 天）
来源：http://hz.sxryk.cn/gtdwqktotj.html

Py:   now + timedelta(days=7)
来源：http://hz.sufxvd.cn/gtfgwxsbdn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgufenzy.top/gtbzamplwg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.mhx1999.top/gtemyrkpws.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtwqklvljq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj202588.top/gtyfeheroj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinyuanbaomall.cn/gtydfblcgn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cqqwz.cn/gtstojjxuw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.gotoacloud.top/gtyxhzqpil.html

[J06] 计算两时间之差
来源：http://hz.zhengqikj.top/gtkgmiqhhe.html

Py:   (end - start).total_seconds()
来源：http://hz.vqdsnc.cn/gtnvxzzcuv.html

PHP:  $end->diff($start)->days;
来源：http://hz.haohaochexian.top/gtfjjrrpcc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hysaishi.cn/gtauwpaqcv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.mhx1999.top/gtwfoucjne.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.smart0.xyz/gtfkbjcrjj.html

Go:   end.Sub(start).Hours()
来源：http://hz.xziqi.cn/gtqzqwysdo.html

Ruby: end - start                 # 返回秒数
来源：http://hz.svipenyu.cn/gtvtrrlujs.html

C#:   (end - start).TotalSeconds
来源：http://hz.52xcode.cn/gtskbghfqy.html

[J07] 比较两个日期
来源：http://hz.sxryk.cn/gtomgkjbuq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ybcxt.top/gtctqvmifp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shzxlz.cn/gtceqwunng.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hysaishi.cn/gtgsnxnmbr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinyuanbaomall.cn/gtcxtrgehl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinqigufen.top/gtktfpmsoz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daxiang520.top/gtugjlktrw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xuanzx.com/gtpurjlpnd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtjatshiui.html

[J08] 提取年月日与星期
来源：http://hz.yj20258888.top/gtkrgbwlwu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hongshengwenyu.top/gtmaxjefhx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.9152youxi.cn/gtbghlkefg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.quarkkingdee.top/gtlbnsrxwg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.guannengcc.top/gtothsqwzp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sweek.top/gtdojruisb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangtech.top/gtbbcvsbfm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xingfuxueyuan.xyz/gtxvjwhwjq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.c1oappe.top/gtbfodymvy.html

[J09] 时区处理
来源：http://hz.aibaodan.cn/gtbwbcybqf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.iojbl.cn/gtptlebmdy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.52xcode.cn/gtvjtqhyif.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtbijqijot.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gtvljityny.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gaohongyu789.top/gtqppnwjaf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hywenlv.cn/gtnbuwucqp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj20258.top/gttyaphjcx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuanzhike.top/gtegylixeu.html

[J10] 取今天 / 本月第一天
来源：http://hz.nwbrower.top/gtjtdklrxj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.iojbl.cn/gtrdzgatby.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinyuanbaomall.cn/gtkwxjnylh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yuanzhike.top/gtdjrybbzi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.aizwys.cn/gthibcshcw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jyoumei.cn/gtlwebrcph.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.mhx1999.top/gtxpdgutay.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinyuanbaomall.cn/gtbaycchfa.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hywenlv.cn/gtpetmhved.html

================================================================================
来源：http://hz.jiagoushi.top/gttvbafpmg.html

K. JSON 与序列化
来源：http://hz.chenzaomai.com/gtwmybmijm.html

================================================================================
来源：http://hz.ivvv.top/gtburleznj.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinqigufen.top/gtdgqzbjul.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sufxvd.cn/gttenpaplc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangtech.top/gtlxnatmgf.html

JS:   JSON.stringify(obj)
来源：http://hz.9152youxi.cn/gtxphaszfl.html

TS:   JSON.stringify(obj)
来源：http://hz.iojbl.cn/gtwgcpckde.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daxiang520.top/gtclzpjszt.html

Go:   json.Marshal(obj)
来源：http://hz.yuanzhike.top/gtefegxvxl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xziqi.cn/gtcgskcwxg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xuetiantiany.cn/gtzbqirorz.html

[K02] JSON 字符串转对象
来源：http://hz.ydjk.org.cn/gtjqagonyw.html

Py:   json.loads(s)
来源：http://hz.52xcode.cn/gtpszzbmdg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhaomingkeji.xyz/gtdteajqdg.html

JS:   JSON.parse(s)
来源：http://hz.pycfn.com/gtczbxpgxg.html

TS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtbzghtxyh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xylfe.cn/gtyzpawymu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtqwhdwtpr.html

Ruby: JSON.parse(s)
来源：http://hz.shanyushiyangkeji.top/gtvqpcmhcs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sysykeji.top/gtbtrvpdjk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhiwuduotai.top/gthjpxbdtj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shzxlz.cn/gtzqfcjqwf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnxiangtu.top/gtodonyhuk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hfpthk.cn/gtkvrcbnqk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinghuilouyu.cn/gtgcmxwwbr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.meibo888.top/gtdjtdudhv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.havefunace.top/gttyefwzwd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.redwolf501.top/gtdnvdmheq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.aibaodan.cn/gtosjmimfu.html

[K04] 读取 JSON 文件
来源：http://hz.yangfankeji.com/gtihwdalqf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuanzhike.top/gtnxynrlgn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.haohaochexian.top/gtxnahppte.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtqqvgmhoj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.havefunace.top/gtstfyxqvy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.316326.xyz/gtlsvxypco.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yj202588.top/gtdecdhrcf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.sufxvd.cn/gtlhhonbjj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shangyingyoupin.top/gtanxlcnly.html

[K05] 深拷贝对象
来源：http://hz.yj20258.top/gtftddyoei.html

Py:   copy.deepcopy(obj)
来源：http://hz.ehwqpu.com/gteljylpod.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xylfe.cn/gtquyxprif.html

JS:   structuredClone(obj)
来源：http://hz.cucudq.cn/gtfrmnwzmo.html

TS:   structuredClone(obj)
来源：http://hz.316326.xyz/gtstahqftb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hnxiangtu.top/gtkorqnayu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258888.top/gtqyzsmkmw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.svipenyu.cn/gtbvwugmjk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xuanzx.com/gtjojrzbna.html

[K06] 解析 URL 查询串
来源：http://hz.aibaodan.cn/gtarqxzleu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinyuanbaomall.cn/gtemzslfrn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxuanxn.top/gtktkmtpur.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhijiandao.cn/gtnmycrufj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.meibo888.top/gtuodfcedq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ybcxt.top/gttivecgbn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.fzhhl.top/gtmonccqiw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yangfankeji.com/gtfckbqxff.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yuxming.cn/gtcbrgkcqm.html

[K07] 进制转换
来源：http://hz.316326.xyz/gtyhtyyasb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtnkwxlszc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nanxuanxn.top/gthfsfbjis.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.kuanghao11.cn/gtfqqieajd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ehwqpu.com/gtzantfpwv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtifiyqgzq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.aizwys.cn/gtvlhluslf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.svipenyu.cn/gtpupuundf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258.top/gtrmbfwcxy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.daria6918.cn/gtayqvppjq.html

Py:   pickle.dumps(obj)
来源：http://hz.haohaochexian.top/gtdvjpnojq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shzxlz.cn/gtsxoglcgx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sweek.top/gtvjeouvzg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gtnejwshnl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinqigufen.top/gtcahwzqsn.html

Go:   encoding/gob
来源：http://hz.dianchejie.cn/gtlegciord.html

Ruby: Marshal.dump(obj)
来源：http://hz.xylfe.cn/gtmtroshle.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jqgfzy.top/gtlndjzquf.html

================================================================================
来源：http://hz.xuanzx.com/gtvhnimyuv.html

L. 网络请求
来源：http://hz.sufxvd.cn/gtudcbukcw.html

================================================================================
来源：http://hz.9152youxi.cn/gtwfmogkmw.html

[L01] 发送 GET 请求
来源：http://hz.jinyuanbaomall.cn/gtucbxsmnt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigufen.top/gthzlcpiww.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hongshengwenyu.top/gtlyruizbg.html

JS:   await fetch(url)
来源：http://hz.yj20258888.top/gtjoqcenuh.html

TS:   await fetch(url)
来源：http://hz.sxryk.cn/gtdxnxudvq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yongpay.top/gtoftyhgsk.html

Go:   resp, err := http.Get(url)
来源：http://hz.nwbrower.top/gtdrlbzqrh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.tian-w.cn/gtgoftefyk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xylfe.cn/gtpkmjetls.html

[L02] 发送 POST JSON
来源：http://hz.chenjidiqi.icu/gtqzmyoelw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj20258888.top/gtojcvupxd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fzhhl.top/gtoolgwoqk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gtduzjigeb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guowangkeji.top/gtlextpoem.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.daria6918.cn/gtkrmrfjmj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinghuilouyu.cn/gtcwpzxtgl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sufxvd.cn/gtjmwhnpau.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.dianchejie.cn/gtmxyfdmcu.html

[L03] 设置自定义请求头
来源：http://hz.zhiwuduotai.top/gtczegfmrf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gogol.net.cn/gtbwltqwkh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sysykeji.top/gtzpnfllpc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.andypj.xyz/gtuwvpcyax.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gtojmucahv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yvedp.cn/gtetthhdje.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.svipenyu.cn/gtucxhhryb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sysykeji.top/gtigcfgnhi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhixingplan.top/gtgdpueput.html

[L04] 设置超时
来源：http://hz.aizwys.cn/gtdlnauuux.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cashguo.top/gtnpmjwixu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yonumen.top/gtxwiqiaxp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gtcjmffzqz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigufen.top/gtpyaezwvd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ywan-chungtsiang.top/gtibfrhkpq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhixingplan.top/gtnfnvjpql.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hywenlv.cn/gthyodazoa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cheryme.top/gtxxhjuetq.html

[L05] 上传文件（multipart）
来源：http://hz.yangfankeji.com/gtvouilgvi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hfpthk.cn/gtfltugoyo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ppjwa.cn/gtzdoehuwt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hysaishi.cn/gtitjpcysr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sweek.top/gtrghnazwu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sxryk.cn/gtaqwayuih.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yanxiufei.cn/gtfzwlzyof.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.fzhhl.top/gtmmbymhnx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinyuanbaomall.cn/gtttjjowvg.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigufen.top/gtbyaqxjmr.html

Py:   resp.json()
来源：http://hz.ivvv.top/gtmyrflpuf.html

PHP:  json_decode($body, true);
来源：http://hz.fzhhl.top/gtmrzqnrsf.html

JS:   await resp.json()
来源：http://hz.dashuyun.cn/gtujbzgrcj.html

TS:   await resp.json()
来源：http://hz.yangfankeji.com/gtuizvyjjs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jqgufenzy.top/gteqzfkclt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.svipenyu.cn/gtmxkaeuhe.html

Ruby: JSON.parse(resp.body)
来源：http://hz.pengpengdd.cyou/gtklmtwack.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.kuanghao11.cn/gtvoiebrmd.html

[L07] 处理 HTTP 状态码
来源：http://hz.mhx1999.top/gtepusbixu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yanxiufei.cn/gtnnfwpwwm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cheryme.top/gturesznle.html

JS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtpjrbfvtm.html

TS:   resp.ok;  resp.status
来源：http://hz.jinyuanbaomall.cn/gtkpjpiqwd.html

Java: resp.statusCode()
来源：http://hz.chenjidiqi.icu/gtdfwmidym.html

Go:   resp.StatusCode
来源：http://hz.tian-w.cn/gtyalglamf.html

Ruby: resp.code.to_i
来源：http://hz.yonumen.top/gtjaciqkax.html

C#:   (int)resp.StatusCode
来源：http://hz.xuanzx.com/gtdgwtierl.html

[L08] 并发请求多个地址
来源：http://hz.shanyushiyangkeji.top/gtytimghke.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinyuanbaomall.cn/gtdwefhinx.html

PHP:  curl_multi_init() 系列
来源：http://hz.sweek.top/gtasdymnfc.html


<!-- 参考信息 -->