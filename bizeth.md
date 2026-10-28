代发 wailian999

[I02] 提取所有匹配
来源：http://hz.jianghu66.top/gtifffimvu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yongpay.top/gtenzqojbr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258888.top/gtqnuykend.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xziqi.cn/gtqskhxtyd.html

TS:   s.match(/\d+/g)
来源：http://hz.meibo888.top/gtngygxeob.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sufxvd.cn/gtnjipsizv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cdnleiting.top/gtuabpketw.html

Ruby: s.scan(/\d+/)
来源：http://hz.gotoacloud.top/gtcntuxmoy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.pycfn.com/gtfdjusjjl.html

[I03] 提取捕获分组
来源：http://hz.zycfv.cn/gtfmjolxjj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhoulong.xyz/gtasjdcszn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jlsjyb.cn/gtjbnxgnbz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.kuanghao11.cn/gtvrsutrob.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hnxiangtu.top/gthltksbkr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenjidiqi.icu/gtxcpzsvta.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.52xcode.cn/gtlzurwmqe.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jqgufenzy.top/gtesdvzlcn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.mhx1999.top/gterdqeaxc.html

[I04] 正则替换
来源：http://hz.jiagoushi.top/gtqoiptdgm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zycfv.cn/gtizdyfhul.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cheryme.top/gtycuqmfmm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhaomingkeji.xyz/gtunhsxweq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.tian-w.cn/gtjdfsuwyt.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.smart0.xyz/gtmxscobsl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.kuanghao11.cn/gtxazpccdv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tianlin.xyz/gtvrstcyzl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhijiandao.cn/gtidouyymm.html

[I05] 按正则拆分
来源：http://hz.jinqigfzy.top/gthyheexup.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yonumen.top/gtbthqxqwi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhijiandao.cn/gtjgrhxdrt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtrawqsqug.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.redwolf501.top/gtnevhcizh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.kuanghao11.cn/gtjptnqbfl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shzxlz.cn/gtpiadipfm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtwygtoojb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yj20258.top/gtvwgpbcic.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.dashuyun.cn/gtodkzfcks.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gtcqcasrqp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zycfv.cn/gtyviseaiw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guowangkeji.top/gtahufgvvn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guannengcc.top/gtepyvgorp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.bjfxy.top/gtkmkueefg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shuidangran.top/gthzdsdqdo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.c1oappe.top/gtsjezwajc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hfpthk.cn/gtkmiyfoem.html

[I07] 忽略大小写与多行模式
来源：http://hz.chenjidiqi.icu/gtqigyivuj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gzhubu.top/gteinotxxw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xingfuxueyuan.xyz/gtsyzoxywc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ivvv.top/gtlnucekap.html

TS:   /error/gim
来源：http://hz.jinqigfzy.top/gtvehlpzal.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.aizwys.cn/gtyonpcvbt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinqigufen.top/gtmgkmprja.html

Ruby: s.scan(/error/i)
来源：http://hz.shanyushiyangkeji.top/gtlqojwqkj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tanke756.top/gtiqwjzsiq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhoulong.xyz/gtcemdfyym.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.havefunace.top/gtaloadxth.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhijiandao.cn/gtbfavovcp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jyoumei.cn/gtjbapfzix.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.mhx1999.top/gtndxjyevn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ybcxt.top/gtjjikcprn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cucudq.cn/gtkzutqbch.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sufxvd.cn/gtmmmsjood.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gzhubu.top/gtpczqawxh.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gthnaxegcd.html

J. 日期与时间
来源：http://hz.gogol.net.cn/gtfrbjoojb.html

================================================================================
来源：http://hz.sufxvd.cn/gtajvydpcl.html

[J01] 获取当前时间
来源：http://hz.yongpay.top/gtnypalhjl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.havefunace.top/gtdcinfkxk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hfpthk.cn/gtynvnjako.html

JS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtghofbujg.html

TS:   new Date();  Date.now()
来源：http://hz.jianghu66.top/gtilescyfh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yvedp.cn/gtmckyatdi.html

Go:   time.Now()
来源：http://hz.wangshuangyany.cn/gtwffgxedd.html

Ruby: Time.now
来源：http://hz.sysykeji.top/gtxtpeeewi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenjidiqi.icu/gtfawqsdnq.html

[J02] 格式化输出
来源：http://hz.zhixingplan.top/gtantidgtz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sweek.top/gtrxkapjzb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ywan-chungtsiang.top/gtojdizrjh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daxiang520.top/gtcavdasoj.html

TS:   d.toISOString()
来源：http://hz.hfpthk.cn/gtplvzohht.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.smart0.xyz/gtnhlbvadu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinqigfzy.top/gthigonkhu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gtyoixqbnr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.aizwys.cn/gtmixdhrig.html

[J03] 字符串解析为日期
来源：http://hz.quarkkingdee.top/gtwyadqbde.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shzxlz.cn/gtgbpgqjmr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.svipenyu.cn/gtiwaggioi.html

JS:   new Date("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtysrcwpwb.html

TS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gtxyqtftdv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.316326.xyz/gtcetvzxpm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.andypj.xyz/gtpzbwefcz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ybcxt.top/gtojqtflrb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.snrcjt.cn/gtxkddlnsy.html

[J04] 时间戳与日期互转
来源：http://hz.iojbl.cn/gtcttlbyqn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhijiandao.cn/gtilumceeq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yj202588.top/gtfccodacz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gzhubu.top/gtoasolbdl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.meibo888.top/gtyrwopqbn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jianghu66.top/gtqermuuoq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ywan-chungtsiang.top/gtzawxjnqs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hywenlv.cn/gtwyinbiyh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ybcxt.top/gtafjvdeex.html

[J05] 时间加减（加 7 天）
来源：http://hz.yuxming.cn/gtfvcsvoin.html

Py:   now + timedelta(days=7)
来源：http://hz.yuanzhike.top/gtjyeelkpo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shanyushiyangtech.top/gtyyoyopiq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gtwoolahab.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aizwys.cn/gticwsopkt.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aibaodan.cn/gtpgicwgqf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sysykeji.top/gtzibbfbsq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tanke756.top/gtdlpysiue.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinghuilouyu.cn/gtrlwitbug.html

[J06] 计算两时间之差
来源：http://hz.xziqi.cn/gtdjktjxwz.html

Py:   (end - start).total_seconds()
来源：http://hz.tanke756.top/gtelgftklh.html

PHP:  $end->diff($start)->days;
来源：http://hz.hnqzz.top/gtrbenflsf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jiagoushi.top/gtchsbwfud.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.9152youxi.cn/gtminrlncf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hammf.cn/gtgpadqrna.html

Go:   end.Sub(start).Hours()
来源：http://hz.xylfe.cn/gtdtuppibf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinghuilouyu.cn/gtdibcovod.html

C#:   (end - start).TotalSeconds
来源：http://hz.guowangkeji.top/gtixbhuyay.html

[J07] 比较两个日期
来源：http://hz.0kj1m.cn/gtraxfdvwj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gtrakmjind.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj20258.top/gtkkfcmdpl.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ppjwa.cn/gthpewmcfv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.316326.xyz/gthmvyscsa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cqqwz.cn/gtevelweps.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guannengcc.top/gthriffcho.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtnbjgtltq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtorkjgkbz.html

[J08] 提取年月日与星期
来源：http://hz.fzhhl.top/gtmivdiiqp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinghuilouyu.cn/gtuhwljfqe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.mhx1999.top/gtbsstrneo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.0kj1m.cn/gtftoiwkpr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tianlin.xyz/gtgkjhbgbz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.feifeiyinyue.top/gtvttzsifl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gotoacloud.top/gtdrlrisux.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sufxvd.cn/gtwfybzqpo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nanxuanxn.top/gtqgsgynzf.html

[J09] 时区处理
来源：http://hz.chenlongwang.top/gtqdokpumk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cqqwz.cn/gtcaxwulev.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenjidiqi.icu/gtommvaazs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cucudq.cn/gtcxqdqsgp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnqzz.top/gthxmupfly.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.andypj.xyz/gtwiyrovmf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.aibaodan.cn/gtzgvrjuhv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.52xcode.cn/gtwibzuwzq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhaomingkeji.xyz/gtebqcukme.html

[J10] 取今天 / 本月第一天
来源：http://hz.yuxming.cn/gtcowmtxvk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.dashuyun.cn/gtjbfztrjv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.svipenyu.cn/gtsjeobtsv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj20258.top/gtidxxgzqv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zdqjudy.top/gtpyrxgypf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xinyue.icu/gtvclktcmp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ydjk.org.cn/gtrxrlzzel.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jianghu66.top/gtebjjikbc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tanke756.top/gtglnoeepl.html

================================================================================
来源：http://hz.birdmap.top/gtxtidwnbl.html

K. JSON 与序列化
来源：http://hz.tanke756.top/gteabbvuwt.html

================================================================================
来源：http://hz.ybcxt.top/gtgsmmeodj.html

[K01] 对象转 JSON 字符串
来源：http://hz.pengpengdd.cyou/gtxsmqwntn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yueranfly.top/gtgvynfuwo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hfpthk.cn/gtsutsfhwh.html

JS:   JSON.stringify(obj)
来源：http://hz.hongshengwenyu.top/gtkxkeadtb.html

TS:   JSON.stringify(obj)
来源：http://hz.cdnleiting.top/gtfxhwmghy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yvedp.cn/gtphxeftur.html

Go:   json.Marshal(obj)
来源：http://hz.jinyuanbaomall.cn/gtecssdzze.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yvedp.cn/gtzlthoqqm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigufen.top/gthhbctoyn.html

[K02] JSON 字符串转对象
来源：http://hz.jinyuanbaomall.cn/gtygrzigvy.html

Py:   json.loads(s)
来源：http://hz.yangfankeji.com/gtpeayddzo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hywenlv.cn/gtxlljnvak.html

JS:   JSON.parse(s)
来源：http://hz.jianghu66.top/gtxhuiiztt.html

TS:   JSON.parse(s)
来源：http://hz.zdqjudy.top/gtubyciwia.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hammf.cn/gtxuhbdews.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ybcxt.top/gtuwohxrfe.html

Ruby: JSON.parse(s)
来源：http://hz.hywenlv.cn/gtcbqpswcr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hongshengwenyu.top/gtcmydbjhh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yangfankeji.com/gtoqhlswzd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hongshengwenyu.top/gtdqimfzro.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gteeyfdpfk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ivvv.top/gtzovjcunr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.fengsongda.top/gtqeudsvxu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.0kj1m.cn/gtvuusdyfu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinyuanbaomall.cn/gtojbeckpd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ywan-chungtsiang.top/gtvqfykdai.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigufen.top/gthlcfyfox.html

[K04] 读取 JSON 文件
来源：http://hz.xylfe.cn/gtljnwmbay.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.c1oappe.top/gtktzmupym.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.aibaodan.cn/gtmolipiol.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtibwqwqvt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258.top/gtjkluxjto.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sysykeji.top/gtywwfazwe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.tian-w.cn/gtxrnpinxp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yueranfly.top/gtbcoaeamz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yonumen.top/gtlbwbzovd.html

[K05] 深拷贝对象
来源：http://hz.xuetiantiany.cn/gthdkqgtcv.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnxiangtu.top/gthhzqoekb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gzhubu.top/gtbjuugbnf.html

JS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtgtukibgz.html

TS:   structuredClone(obj)
来源：http://hz.yj20258.top/gtwpvgunnb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.guowangkeji.top/gtzoedhwcg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.daxiang520.top/gtvinuulwe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gogol.net.cn/gtbqxgnhuj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yuxming.cn/gtvpszhsvo.html

[K06] 解析 URL 查询串
来源：http://hz.cdnleiting.top/gtzwnpbksh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgufenzy.top/gtkarzthkj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yongpay.top/gtkkaoslxu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhijiandao.cn/gtfstcijjh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhixingplan.top/gtkgbwwfcf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.redwolf501.top/gtvlbyikzt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.wangdashe.top/gtbdppvjxh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.0kj1m.cn/gteprktzzp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yongpay.top/gthnebuhlx.html

[K07] 进制转换
来源：http://hz.wangdashe.top/gtgpkqzicr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhongyouzk.top/gtoruodpyo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ehwqpu.com/gtfiziwgtx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtigtcgumo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gteknkqvgb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.c1oappe.top/gtyynmctzk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zycfv.cn/gtxvufheca.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.316326.xyz/gtxnbyovsi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuanzx.com/gtyylsmmcy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zdqjudy.top/gtjwanrtzt.html

Py:   pickle.dumps(obj)
来源：http://hz.svipenyu.cn/gtzswyzgxh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.iojbl.cn/gtxtckmkjm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zdqjudy.top/gtymhkseby.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.nanxuanxn.top/gtyfgitedh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yvedp.cn/gtmaqqjkty.html

Go:   encoding/gob
来源：http://hz.yj202588.top/gtxbgmcxwo.html

Ruby: Marshal.dump(obj)
来源：http://hz.daxiang520.top/gtmpioyuno.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sxryk.cn/gtjlwhzggj.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtidwfgvhm.html

L. 网络请求
来源：http://hz.snrcjt.cn/gtrbnikjva.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtiroletcq.html

[L01] 发送 GET 请求
来源：http://hz.gaohongyu789.top/gtlpdcnugh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gaohongyu789.top/gtlggbyqgg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yanxiufei.cn/gtmlweqhgc.html

JS:   await fetch(url)
来源：http://hz.redwolf501.top/gtwyjrymkd.html

TS:   await fetch(url)
来源：http://hz.jinyuanbaomall.cn/gtzoqyceuu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhiwuduotai.top/gtzwpptwfl.html

Go:   resp, err := http.Get(url)
来源：http://hz.andypj.xyz/gtgdsjdvng.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhoulong.xyz/gtpgwojfnz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ppjwa.cn/gtnxiwimto.html

[L02] 发送 POST JSON
来源：http://hz.sxryk.cn/gtgkyjxdkv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhaomingkeji.xyz/gtlzszrhkz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhijiandao.cn/gtdwpmuqbh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zdqjudy.top/gtrruwmoyy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.vqdsnc.cn/gtqboxlcgm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.havefunace.top/gtqlldzdph.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.aizwys.cn/gtbsllxllu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhiwuduotai.top/gtmwuwiumm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yangfankeji.com/gtxhbbhykg.html

[L03] 设置自定义请求头
来源：http://hz.ybcxt.top/gtptdoamnn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hammf.cn/gtdusesufk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hnqzz.top/gtdzeruhtj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gtocxakxpc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hammf.cn/gtturijzbj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhaomingkeji.xyz/gtkoqolhtt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.pengpengdd.cyou/gtwgawrdek.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.aizwys.cn/gtriqnrkkm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuxming.cn/gtcidgwvut.html

[L04] 设置超时
来源：http://hz.havefunace.top/gtoamdsbhu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhaomingkeji.xyz/gtmhlheudf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.chenjidiqi.icu/gtflyegeor.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gtumgevavf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sxryk.cn/gtfuefznhi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.redwolf501.top/gttreecard.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sweek.top/gtmzcsydcq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.bjfxy.top/gtnebrnmhs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yangfankeji.com/gtjdbdpqqi.html

[L05] 上传文件（multipart）
来源：http://hz.smart0.xyz/gtpolvkdte.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shuidangran.top/gtcirivrdo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hfpthk.cn/gtqqjnfnoa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shzxlz.cn/gtjzybuvat.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cheryme.top/gtenwyzufi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gotoacloud.top/gteietymyy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hfpthk.cn/gttdgkoqer.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pengpengdd.cyou/gtqkpuxtee.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yongpay.top/gtyyxxdeel.html

[L06] 解析响应为 JSON
来源：http://hz.zhongyouzk.top/gtsywazkmf.html

Py:   resp.json()
来源：http://hz.ivvv.top/gtisavdcye.html

PHP:  json_decode($body, true);
来源：http://hz.sxryk.cn/gtlnlszeip.html

JS:   await resp.json()
来源：http://hz.zhaomingkeji.xyz/gtyhawyhjp.html

TS:   await resp.json()
来源：http://hz.chenlongwang.top/gtezydokwn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.snrcjt.cn/gtssmhxjwv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.daxiang520.top/gtzutoyngt.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhaomingkeji.xyz/gtwvtwpimw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.wangdashe.top/gthagtmdhz.html

[L07] 处理 HTTP 状态码
来源：http://hz.nwbrower.top/gttaxdgrif.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xingfuxueyuan.xyz/gtsifnqssp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gaohongyu789.top/gtooxtxgor.html

JS:   resp.ok;  resp.status
来源：http://hz.xuanzx.com/gtpvnvszrx.html

TS:   resp.ok;  resp.status
来源：http://hz.aibaodan.cn/gtjcupoups.html

Java: resp.statusCode()
来源：http://hz.wangshuangyany.cn/gtpyknypwt.html

Go:   resp.StatusCode
来源：http://hz.ivvv.top/gtmbejljkf.html

Ruby: resp.code.to_i
来源：http://hz.sxryk.cn/gtqhhipklr.html

C#:   (int)resp.StatusCode
来源：http://hz.shanyushiyangtech.top/gtbsvpaxco.html

[L08] 并发请求多个地址
来源：http://hz.gaohongyu789.top/gtaausekfa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jyoumei.cn/gtyukiunve.html

PHP:  curl_multi_init() 系列
来源：http://hz.hnxiangtu.top/gttitgerrv.html


<!-- 参考信息 -->