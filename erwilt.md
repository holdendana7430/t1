代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.0kj1m.cn/gtewqxmtee.html

Go:   defer f.Close()
来源：http://hz.yongpay.top/gtwthliebc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yanxiufei.cn/gtaodifsay.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sysykeji.top/gthqisdnoz.html

================================================================================
来源：http://hz.aizwys.cn/gthpifbzka.html

I. 正则表达式
来源：http://hz.jianghu66.top/gtcwnyeczg.html

================================================================================
来源：http://hz.zhoulong.xyz/gtxjqbabcq.html

[I01] 判断是否匹配
来源：http://hz.jinyuanbaomall.cn/gtxaltomye.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gzhubu.top/gtidjyzgei.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.0kj1m.cn/gtmjrmxtar.html

JS:   /\d+/.test(s)
来源：http://hz.cheryme.top/gtmdgvuwkm.html

TS:   /\d+/.test(s)
来源：http://hz.zhongyouzk.top/gtvfpveckb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.andypj.xyz/gtbnrfgfug.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jiagoushi.top/gtirsjmuuz.html

Ruby: s.match?(/\d+/)
来源：http://hz.shanyushiyangtech.top/gtzyxrhvwr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangshuangyany.cn/gtqpsetrgk.html

[I02] 提取所有匹配
来源：http://hz.smart0.xyz/gtnryygubi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hfpthk.cn/gtlxbxcpfn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jqgfzy.top/gthkdxgqan.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nanxinkj.top/gtlspoekfo.html

TS:   s.match(/\d+/g)
来源：http://hz.havefunace.top/gttwxmtdlk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.pengpengdd.cyou/gthnatohck.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.feifeiyinyue.top/gtvjzxlqdu.html

Ruby: s.scan(/\d+/)
来源：http://hz.316326.xyz/gtecnxwiht.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hammf.cn/gtcgtangen.html

[I03] 提取捕获分组
来源：http://hz.feifeiyinyue.top/gtuhexoiyz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dashuyun.cn/gtawegfxax.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.svipenyu.cn/gtdvaixgjy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pengpengdd.cyou/gtygspcrdk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ydzc1.top/gtcfzlftul.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinghuilouyu.cn/gtxcfqhyei.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cdnleiting.top/gtbyyehvoz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.fzhhl.top/gthtezmbqz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zycfv.cn/gtdfrrvmxr.html

[I04] 正则替换
来源：http://hz.jyoumei.cn/gtspaotsvg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.wangshuangyany.cn/gtyoeyddfd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nwbrower.top/gtgldflrpl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gaohongyu789.top/gtocnjrmuv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cashguo.top/gtdndegwkc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guannengcc.top/gtqbtxqlch.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jqgfzy.top/gtglmdkqjh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.guowangkeji.top/gtmscppqcw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yongpay.top/gttjxvnosg.html

[I05] 按正则拆分
来源：http://hz.0kj1m.cn/gttmaztzjp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ybcxt.top/gtcekhqfug.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hywenlv.cn/gtotstxqqh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.pycfn.com/gtzdkhrjya.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtspweovqa.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zycfv.cn/gthcbvvexr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hysaishi.cn/gtlxgmuyym.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gtjdxfmqax.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ehwqpu.com/gtdzqpqlhr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cqqwz.cn/gttucupsrz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tanke756.top/gtghvrlbrm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hysaishi.cn/gtfmbewutq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxinkj.top/gtnqiiolkz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuxming.cn/gtmlssjvgg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.guannengcc.top/gtazwrtnwc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ppjwa.cn/gtzfjrahgr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.andypj.xyz/gtncjzndxd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hnxiangtu.top/gttrhclkdr.html

[I07] 忽略大小写与多行模式
来源：http://hz.zycfv.cn/gtvrjeqvah.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jianghu66.top/gtwygcszzq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.bjfxy.top/gtzwgpgvmg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nwbrower.top/gtzdjwsrak.html

TS:   /error/gim
来源：http://hz.nanxuanxn.top/gtqdemtcgo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yj202588.top/gtlvhbwqdb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shuidangran.top/gtqfogbzje.html

Ruby: s.scan(/error/i)
来源：http://hz.xinyue.icu/gtsbebsbks.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hnqzz.top/gtrgtfpfvy.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinghuilouyu.cn/gtymxenhzs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.meibo888.top/gttkjzsuwe.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sufxvd.cn/gtwadtpgpe.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhiwuduotai.top/gtmclntaqr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnxiangtu.top/gtgbncvkiu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.52xcode.cn/gtqlhjhrox.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.fzhhl.top/gtgkdrqwbj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cheryme.top/gtuqwtzlyc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daria6918.cn/gtkxkhoale.html

================================================================================
来源：http://hz.ivvv.top/gtsihxdnfc.html

J. 日期与时间
来源：http://hz.smart0.xyz/gtwkfodkiv.html

================================================================================
来源：http://hz.havefunace.top/gtepyvypqb.html

[J01] 获取当前时间
来源：http://hz.dianchejie.cn/gtiyrirpnk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.9152youxi.cn/gtazwdrszu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gtffnhebaw.html

JS:   new Date();  Date.now()
来源：http://hz.aizwys.cn/gtgwsycjrj.html

TS:   new Date();  Date.now()
来源：http://hz.xinyue.icu/gtwspvlqwv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cashguo.top/gtpbxvyeqm.html

Go:   time.Now()
来源：http://hz.zhiwuduotai.top/gtmvlgnihg.html

Ruby: Time.now
来源：http://hz.hywenlv.cn/gtohczqfrd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zdqjudy.top/gtoipneqav.html

[J02] 格式化输出
来源：http://hz.guowangkeji.top/gtzrlczpbk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuxming.cn/gtfyarbdsz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zdqjudy.top/gtchlcttoa.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.kuanghao11.cn/gtujpmnrcj.html

TS:   d.toISOString()
来源：http://hz.gaohongyu789.top/gtpuffqalm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnxiangtu.top/gtrykgmfjl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yj20258.top/gtwhextuok.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tanke756.top/gtvilwokrq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hammf.cn/gtoivqikdn.html

[J03] 字符串解析为日期
来源：http://hz.dianchejie.cn/gtmooyentm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.c1oappe.top/gtrxriabdi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj20258.top/gtqhhamdpe.html

JS:   new Date("2024-01-02")
来源：http://hz.daxiang520.top/gtfhmqnbcr.html

TS:   new Date("2024-01-02")
来源：http://hz.hywenlv.cn/gtoxhibaqv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtslqtzgvf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.aibaodan.cn/gtaayxsmwo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gotoacloud.top/gtvxpcdsfp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gotoacloud.top/gtqqevhmvc.html

[J04] 时间戳与日期互转
来源：http://hz.ybcxt.top/gtjgwbbqdq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhiwuduotai.top/gtwdbcygzd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xylfe.cn/gtnndfqnwt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.andypj.xyz/gtvezdeqht.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.havefunace.top/gthwdsldcm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yanxiufei.cn/gtupbjllim.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xuetiantiany.cn/gtltymtqcq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.316326.xyz/gtaplcdqaj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yueranfly.top/gtsmaomswv.html

[J05] 时间加减（加 7 天）
来源：http://hz.nwbrower.top/gtgzzvdjif.html

Py:   now + timedelta(days=7)
来源：http://hz.bjfxy.top/gtcdthxuta.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.9152youxi.cn/gtvrbnmspu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pycfn.com/gtjxduvbkh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhongyouzk.top/gtznkrsuaf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuxming.cn/gtgwfadoho.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.9152youxi.cn/gtnetmndnc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hongshengwenyu.top/gtzzcgtbuh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jianghu66.top/gtulalvzgl.html

[J06] 计算两时间之差
来源：http://hz.c1oappe.top/gtthghnlxo.html

Py:   (end - start).total_seconds()
来源：http://hz.yuxming.cn/gtwrfuqksb.html

PHP:  $end->diff($start)->days;
来源：http://hz.sxryk.cn/gtmbjglewt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.mhx1999.top/gtkwtxmjpf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.vqdsnc.cn/gtrzjbwoeb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.mhx1999.top/gtfimifjxm.html

Go:   end.Sub(start).Hours()
来源：http://hz.sufxvd.cn/gtvoqspuua.html

Ruby: end - start                 # 返回秒数
来源：http://hz.wangshuangyany.cn/gtaipzygwy.html

C#:   (end - start).TotalSeconds
来源：http://hz.hywenlv.cn/gtljxiuydt.html

[J07] 比较两个日期
来源：http://hz.smart0.xyz/gteropanvj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gtfbodcihy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tian-w.cn/gtpmbdtrhd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangtech.top/gtxyntqmnh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhoulong.xyz/gthgmoiels.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhongyouzk.top/gtsughbhhb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nanxuanxn.top/gtfvxxlrux.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gtrkuxetut.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtqjderffc.html

[J08] 提取年月日与星期
来源：http://hz.shangyingyoupin.top/gtjzslucop.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jqgfzy.top/gtrpzasqql.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jlsjyb.cn/gtqprbnjvy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xinyue.icu/gtaefipuac.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgfzy.top/gtoibbmoaw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.feifeiyinyue.top/gthflgvmmb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gaohongyu789.top/gtyizvdzbb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258888.top/gtoygbjtnx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jiagoushi.top/gtkbdmkxfd.html

[J09] 时区处理
来源：http://hz.daxiang520.top/gtqtcmnzoo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.dashuyun.cn/gtvonqslzl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cqqwz.cn/gtfdpduklt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtqqfmxdkl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cheryme.top/gtkoenogin.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hnqzz.top/gtsgpiqfdm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gogol.net.cn/gtxmdkhwyg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.andypj.xyz/gtewbuobgq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.52xcode.cn/gtrtiavjdn.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhijiandao.cn/gtagffleyq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xziqi.cn/gtlkruzfkz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ydjk.org.cn/gtrfgdtirf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aibaodan.cn/gtocoqcwuq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ppjwa.cn/gtyffprkmi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cqqwz.cn/gtcamlwtor.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenzaomai.com/gtqgqndote.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jlsjyb.cn/gtyedqgwbp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj20258.top/gtalzdsdbd.html

================================================================================
来源：http://hz.yj20258.top/gteumszsiy.html

K. JSON 与序列化
来源：http://hz.hongshengwenyu.top/gtpesyczea.html

================================================================================
来源：http://hz.shuidangran.top/gtdtyvhaxv.html

[K01] 对象转 JSON 字符串
来源：http://hz.52xcode.cn/gtozklwlgq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigfzy.top/gtvhbdsdtt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gtqijnteou.html

JS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gtlxvgituu.html

TS:   JSON.stringify(obj)
来源：http://hz.smart0.xyz/gtmchqqpfu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shuidangran.top/gtctgfsjfy.html

Go:   json.Marshal(obj)
来源：http://hz.xylfe.cn/gtcowpkyxz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.smart0.xyz/gtkapimjwe.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xuetiantiany.cn/gtbmdcjdzd.html

[K02] JSON 字符串转对象
来源：http://hz.pycfn.com/gtggucntij.html

Py:   json.loads(s)
来源：http://hz.fengsongda.top/gtpjvggiqj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tianlin.xyz/gttxxuglvh.html

JS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtdehagmfz.html

TS:   JSON.parse(s)
来源：http://hz.tian-w.cn/gtqpgdqmob.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnqzz.top/gtesmuswaz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ybcxt.top/gtdtffnzqy.html

Ruby: JSON.parse(s)
来源：http://hz.9152youxi.cn/gtinvpeudv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.iojbl.cn/gtaxwkiltg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jqgufenzy.top/gtswnejipe.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.guowangkeji.top/gtsrunojer.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hfpthk.cn/gtqcxctyby.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.daria6918.cn/gtqblptzhe.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.meibo888.top/gtdabnuhag.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.aibaodan.cn/gtlycmdyth.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.feifeiyinyue.top/gtsvvsfkuu.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.pycfn.com/gtsvfqswce.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gotoacloud.top/gtmtymlmfs.html

[K04] 读取 JSON 文件
来源：http://hz.smart0.xyz/gtwpingtnf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ybcxt.top/gtckykwuzd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.pengpengdd.cyou/gtwqkrysao.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.svipenyu.cn/gtilpvziid.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yvedp.cn/gtsxafxldk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yangfankeji.com/gtiixwqbye.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.dashuyun.cn/gtqzxsfsqf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nwbrower.top/gtngikjzmq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shzxlz.cn/gtbvipuhoy.html

[K05] 深拷贝对象
来源：http://hz.zhijiandao.cn/gtslschxbd.html

Py:   copy.deepcopy(obj)
来源：http://hz.dianchejie.cn/gttltdryrj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj202588.top/gtzujeihoh.html

JS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gtatakppoo.html

TS:   structuredClone(obj)
来源：http://hz.shangyingyoupin.top/gtrsxvoevl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.nwbrower.top/gtisgmgfhr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.mhx1999.top/gtjyjetlnk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jlsjyb.cn/gtrgsdtuwx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jlsjyb.cn/gtxkhmgjbn.html

[K06] 解析 URL 查询串
来源：http://hz.yj202588.top/gtyvbdqxbi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.guannengcc.top/gtyqjwrewj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhixingplan.top/gtajopsijl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yanxiufei.cn/gtjoolpcwx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tianlin.xyz/gtldqvszhl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenzaomai.com/gtlgfdqgxl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tian-w.cn/gtkuqydefc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shanyushiyangtech.top/gttogqatwu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.feifeiyinyue.top/gtqjbounks.html

[K07] 进制转换
来源：http://hz.jqgufenzy.top/gtygywdchn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.nanxinkj.top/gtfrynngwk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xingfuxueyuan.xyz/gtfrhvjcqn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtxwvogiry.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtcpoapzcy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtlqervgfq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.havefunace.top/gtfxeklbib.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shanyushiyangkeji.top/gtcqoclxxp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sysykeji.top/gtkxaqyrpp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj20258888.top/gtgcuwtujt.html

Py:   pickle.dumps(obj)
来源：http://hz.ybcxt.top/gtttwvdugi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xziqi.cn/gtmqwllbab.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gtnyrivcks.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtrvcaggsv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jiagoushi.top/gtlorejlpi.html

Go:   encoding/gob
来源：http://hz.chenlongwang.top/gtceutjbms.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhongyouzk.top/gtclwnxwny.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gzhubu.top/gtxofukkai.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtccuksnuy.html

L. 网络请求
来源：http://hz.tanke756.top/gtwhdjmaab.html

================================================================================
来源：http://hz.gogol.net.cn/gtqagghqco.html

[L01] 发送 GET 请求
来源：http://hz.yj202588.top/gtzyegeqqz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yj202588.top/gtfznsmupy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gaohongyu789.top/gtbfahqnld.html

JS:   await fetch(url)
来源：http://hz.ybcxt.top/gtfmzhmkwu.html

TS:   await fetch(url)
来源：http://hz.52xcode.cn/gtvpeycdvh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.tian-w.cn/gtdkmdtrfq.html

Go:   resp, err := http.Get(url)
来源：http://hz.yj20258888.top/gtgypmoygp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.wangdashe.top/gtwnrhyapm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xuetiantiany.cn/gtirimmqxj.html

[L02] 发送 POST JSON
来源：http://hz.nwbrower.top/gtbjmihzfd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.birdmap.top/gtemnfxlhs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sufxvd.cn/gtztzrwsva.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hysaishi.cn/gtzarhdzwv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jyoumei.cn/gtnhyfsrgh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhiwuduotai.top/gtqekbkoku.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hongshengwenyu.top/gtrgnjsymy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shuidangran.top/gtgiiwxvqx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yonumen.top/gtdkvnwuja.html

[L03] 设置自定义请求头
来源：http://hz.jqgufenzy.top/gttbynhbty.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhijiandao.cn/gtvxteflra.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xuetiantiany.cn/gtijhyxlqa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aibaodan.cn/gtzyhdqhqy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.quarkkingdee.top/gtevganwkx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj20258.top/gtkauduzhe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zycfv.cn/gtayxjqeit.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tianlin.xyz/gtjtnqyedj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sxryk.cn/gtjdvjsjgm.html

[L04] 设置超时
来源：http://hz.andypj.xyz/gtnklesdfa.html

Py:   requests.get(url, timeout=5)
来源：http://hz.guannengcc.top/gtdlxidimt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.kuanghao11.cn/gtwymgxpet.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.quarkkingdee.top/gtzssvtfpd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jlsjyb.cn/gtsctgyhsa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.daria6918.cn/gtnlsozjxd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gaohongyu789.top/gtiarvllxf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yangfankeji.com/gtowhohvcx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.fengsongda.top/gtwlpiznza.html

[L05] 上传文件（multipart）
来源：http://hz.smart0.xyz/gtcrwfbwbc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.haohaochexian.top/gtrhktmpeo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhixingplan.top/gtkbhkcehh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sysykeji.top/gtgfkdcyrd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinghuilouyu.cn/gtiipmolwh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.aibaodan.cn/gtzilapeuw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yj20258.top/gtqddzvdwg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ehwqpu.com/gtwlmletgr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.bjfxy.top/gtyupkxeca.html

[L06] 解析响应为 JSON
来源：http://hz.zhixingplan.top/gtbpiailfe.html

Py:   resp.json()
来源：http://hz.wangdashe.top/gtfshkkvhn.html

PHP:  json_decode($body, true);
来源：http://hz.nanxinkj.top/gteuewxsvb.html

JS:   await resp.json()
来源：http://hz.hnqzz.top/gtxkmtymjg.html

TS:   await resp.json()
来源：http://hz.hysaishi.cn/gtnrouhwew.html


<!-- 参考信息 -->