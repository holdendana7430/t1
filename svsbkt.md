代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tianlin.xyz/gtdveqvifd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hysaishi.cn/gtdqiokaxv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xinyue.icu/gtawotohiw.html

[H10] 资源自动释放
来源：http://hz.jlsjyb.cn/gtnfjgpyoj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhongyouzk.top/gtftigrfmw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dashuyun.cn/gtnrksssac.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gtosgrxdwe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xinyue.icu/gtnhsjshcq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sysykeji.top/gtraopqvgb.html

Go:   defer f.Close()
来源：http://hz.fengsongda.top/gtlcmdbnau.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cucudq.cn/gtgznrpiov.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangtech.top/gtgswxkvpb.html

================================================================================
来源：http://hz.316326.xyz/gthqnehasn.html

I. 正则表达式
来源：http://hz.birdmap.top/gtcigblnxr.html

================================================================================
来源：http://hz.daria6918.cn/gtbhuxnwoy.html

[I01] 判断是否匹配
来源：http://hz.cheryme.top/gtonookrgy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tian-w.cn/gtnzpocdkm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dianchejie.cn/gtvkhyqpvk.html

JS:   /\d+/.test(s)
来源：http://hz.ybcxt.top/gthfwoiepr.html

TS:   /\d+/.test(s)
来源：http://hz.zhixingplan.top/gtpqczsdji.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.svipenyu.cn/gtdrhldjjx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.316326.xyz/gtashppcry.html

Ruby: s.match?(/\d+/)
来源：http://hz.tian-w.cn/gtzrmqnapf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangdashe.top/gtaamjpzqe.html

[I02] 提取所有匹配
来源：http://hz.yonumen.top/gttfpvbmbi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xziqi.cn/gtayhjoydn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.c1oappe.top/gtcjwaejdp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.chenlongwang.top/gtdakgnyjr.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigfzy.top/gtguskcemx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhiwuduotai.top/gttqbwhmqn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yj20258888.top/gtetjcjemi.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinqigufen.top/gteuaqlpjh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tianlin.xyz/gtrghepriu.html

[I03] 提取捕获分组
来源：http://hz.yvedp.cn/gtizgyysql.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinyuanbaomall.cn/gtbjlakohm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.mhx1999.top/gtqcdhovwo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xuetiantiany.cn/gtzyhegcvz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sweek.top/gtedlytoed.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yangfankeji.com/gtafgsgolq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhengqikj.top/gtobjrvetg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinqigfzy.top/gthdbktmtd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jlsjyb.cn/gtrjivhsmf.html

[I04] 正则替换
来源：http://hz.yonumen.top/gttvabgobw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ybcxt.top/gtfwgldmeg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shangyingyoupin.top/gttgubhogu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cqqwz.cn/gtubtuquaz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.redwolf501.top/gtlmlhrapb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.fzhhl.top/gtuowehuqc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gotoacloud.top/gtvdzsvcmw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ppjwa.cn/gtsltxrxnv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jiagoushi.top/gtftikxqcx.html

[I05] 按正则拆分
来源：http://hz.jqgufenzy.top/gtrjiaxvso.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ydjk.org.cn/gtjnetwqmn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ehwqpu.com/gtomyfsohj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gttvdnwmmr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtpplapmrj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.redwolf501.top/gtfbqfjreo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinghuilouyu.cn/gtmuuqsksi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtdgpamcjv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hnxiangtu.top/gtubumzhtc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxinkj.top/gtuxxsafto.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sufxvd.cn/gtznqgpoye.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.0kj1m.cn/gtowlfnyci.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinghuilouyu.cn/gtruisgzof.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nwbrower.top/gtqgazpsad.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sysykeji.top/gttqnngwzr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ybcxt.top/gtcacxpjpz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinqigufen.top/gtxajfknmy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xylfe.cn/gtkeayiuze.html

[I07] 忽略大小写与多行模式
来源：http://hz.zdqjudy.top/gtfpqasruh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.smart0.xyz/gtzchnyxco.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cucudq.cn/gtthhkcobn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ppjwa.cn/gtstjmzlau.html

TS:   /error/gim
来源：http://hz.havefunace.top/gtaujnxvyf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cashguo.top/gtgolotuop.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pycfn.com/gtwqnfxqzh.html

Ruby: s.scan(/error/i)
来源：http://hz.wangshuangyany.cn/gtrbjvswfq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.aibaodan.cn/gtyyguijqs.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gzhubu.top/gtnmujeglf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cucudq.cn/gtdhpcadqp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhoulong.xyz/gtzvrqjqnc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhiwuduotai.top/gtqmhstcmt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtduoorfog.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daria6918.cn/gtztlidrxd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gogol.net.cn/gteubqqhyg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.52xcode.cn/gtpkmmsnet.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.tanke756.top/gtaokntbmb.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtnqpkcogr.html

J. 日期与时间
来源：http://hz.hnqzz.top/gtiswmktle.html

================================================================================
来源：http://hz.ivvv.top/gtxrqsohhs.html

[J01] 获取当前时间
来源：http://hz.cqqwz.cn/gtyqtzmbgb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.redwolf501.top/gtocfnxbvc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tianlin.xyz/gteaqsyrvz.html

JS:   new Date();  Date.now()
来源：http://hz.zhixingplan.top/gtycbedpek.html

TS:   new Date();  Date.now()
来源：http://hz.iojbl.cn/gtxwqudnks.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.kuanghao11.cn/gtedwxkhuk.html

Go:   time.Now()
来源：http://hz.dianchejie.cn/gtevfpggob.html

Ruby: Time.now
来源：http://hz.nwbrower.top/gtgwkzxpnt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shzxlz.cn/gtpkxdkjvw.html

[J02] 格式化输出
来源：http://hz.jinqigfzy.top/gtmxvczxam.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtewqhirmy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xylfe.cn/gtxdeuewou.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nwbrower.top/gtbudtdese.html

TS:   d.toISOString()
来源：http://hz.zdqjudy.top/gtqnelomie.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgufenzy.top/gtwjbfsato.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tianlin.xyz/gtjxhuhgap.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gogol.net.cn/gtbksziexu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.daxiang520.top/gtfnauaicz.html

[J03] 字符串解析为日期
来源：http://hz.xuetiantiany.cn/gtyqbkteyr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yj20258888.top/gtjlukjeet.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shanyushiyangkeji.top/gthbbmggmu.html

JS:   new Date("2024-01-02")
来源：http://hz.gogol.net.cn/gtvvcmsuqz.html

TS:   new Date("2024-01-02")
来源：http://hz.svipenyu.cn/gtzvhymrrc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guowangkeji.top/gtgudozqvn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.snrcjt.cn/gtkofjagtq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtuytjkqfj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cucudq.cn/gtkkzsjwzz.html

[J04] 时间戳与日期互转
来源：http://hz.yongpay.top/gtiusmfnpt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.havefunace.top/gthngeqpfh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sweek.top/gtfksppynp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hnxiangtu.top/gtmdhtyhjf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.mhx1999.top/gtgbehsmkb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.wangdashe.top/gtmckqjvdw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.52xcode.cn/gtsrhuckkm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cashguo.top/gtgjfnczvf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.kuanghao11.cn/gtfkiqhwfs.html

[J05] 时间加减（加 7 天）
来源：http://hz.cashguo.top/gtotrsvebf.html

Py:   now + timedelta(days=7)
来源：http://hz.yuxming.cn/gtirjemnfw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.wangshuangyany.cn/gtlkxmjkqr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zycfv.cn/gtfvmwhntn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.andypj.xyz/gtvxigojst.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinqigfzy.top/gtlooeqmxn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.fzhhl.top/gthlnubazi.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinghuilouyu.cn/gtcdrmjeik.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ydzc1.top/gtusyjmijh.html

[J06] 计算两时间之差
来源：http://hz.ywan-chungtsiang.top/gtspdjthys.html

Py:   (end - start).total_seconds()
来源：http://hz.nwbrower.top/gtdphlnsrb.html

PHP:  $end->diff($start)->days;
来源：http://hz.iojbl.cn/gttwisezef.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.aizwys.cn/gtmnahxflw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.tianlin.xyz/gtzcqxygab.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ppjwa.cn/gtwivxtyln.html

Go:   end.Sub(start).Hours()
来源：http://hz.hywenlv.cn/gtyypvshvp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xuanzx.com/gtcyqydeig.html

C#:   (end - start).TotalSeconds
来源：http://hz.tanke756.top/gtpdrcdkzo.html

[J07] 比较两个日期
来源：http://hz.xuetiantiany.cn/gtiypjhayh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtcxnxxbxc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj20258888.top/gtokprfrya.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.316326.xyz/gtmvpxdxpx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gteblygect.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yuanzhike.top/gtxifvxhod.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xuanzx.com/gtxpzgjwtp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtxvtvpntz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jyoumei.cn/gtfmuyvgow.html

[J08] 提取年月日与星期
来源：http://hz.xuetiantiany.cn/gtuizldwli.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.0kj1m.cn/gtudsuvlpy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.daxiang520.top/gtunbzcsda.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hnxiangtu.top/gtegwmbusr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hongshengwenyu.top/gtdvryqmsr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cashguo.top/gtzncowfln.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zycfv.cn/gtjwlygbox.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daria6918.cn/gtrvoarqwl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhongyouzk.top/gtadqdbfem.html

[J09] 时区处理
来源：http://hz.hnqzz.top/gtcmxofgdi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenzaomai.com/gtnlnmfybl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.mhx1999.top/gtfelkpjsl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.9152youxi.cn/gttkswzjvt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhixingplan.top/gtdupsicxz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigufen.top/gtfblxpmjv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.aizwys.cn/gtvvnxcaxg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xingfuxueyuan.xyz/gtfqqccuoi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.smart0.xyz/gtnjtzllae.html

[J10] 取今天 / 本月第一天
来源：http://hz.gzhubu.top/gtygwyopca.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shanyushiyangkeji.top/gtagouavod.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ydjk.org.cn/gtxmokeqop.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinqigufen.top/gtjgjzfnpk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dashuyun.cn/gtdrzziivj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhengqikj.top/gtdkgitshr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shanyushiyangkeji.top/gtbwszpzfh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj20258888.top/gtdseukmqg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.wangdashe.top/gtwjguvcxe.html

================================================================================
来源：http://hz.iojbl.cn/gtbevxtajo.html

K. JSON 与序列化
来源：http://hz.jinyuanbaomall.cn/gtkaimchnh.html

================================================================================
来源：http://hz.yuxming.cn/gtgzubjafw.html

[K01] 对象转 JSON 字符串
来源：http://hz.hnqzz.top/gtatssphzb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtypcrpooh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ywan-chungtsiang.top/gtghvitazg.html

JS:   JSON.stringify(obj)
来源：http://hz.dianchejie.cn/gtfschgupa.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgfzy.top/gthpfihgvf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhijiandao.cn/gttksuvktz.html

Go:   json.Marshal(obj)
来源：http://hz.yangfankeji.com/gtfxztnpgc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.dashuyun.cn/gtclgikqfx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nanxuanxn.top/gtdhqyygvv.html

[K02] JSON 字符串转对象
来源：http://hz.zdqjudy.top/gtbiniqogo.html

Py:   json.loads(s)
来源：http://hz.pengpengdd.cyou/gtgatnmixb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuanzhike.top/gtxttztusi.html

JS:   JSON.parse(s)
来源：http://hz.c1oappe.top/gtcsegzprr.html

TS:   JSON.parse(s)
来源：http://hz.aizwys.cn/gtllucfcgn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhijiandao.cn/gtipozxsvd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ehwqpu.com/gtlsunuyym.html

Ruby: JSON.parse(s)
来源：http://hz.52xcode.cn/gtxpmifnpf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.316326.xyz/gtgyklacnq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.meibo888.top/gtwihgggla.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.kuanghao11.cn/gtruvsccek.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.smart0.xyz/gtrbszdocg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtqcojkrxy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhijiandao.cn/gttazppqux.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.andypj.xyz/gtehkywdil.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xinyue.icu/gtwdmhwpdc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhixingplan.top/gtfpkvjzez.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jyoumei.cn/gtyftuizbh.html

[K04] 读取 JSON 文件
来源：http://hz.daria6918.cn/gtokxsuble.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xuanzx.com/gtkxoppmsc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yueranfly.top/gtfdirepzi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.bjfxy.top/gtzsrcnetl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtsonuyddg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sweek.top/gtxcdfeimw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtgybpltye.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.dashuyun.cn/gtohodclzk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.fzhhl.top/gttoyfykta.html

[K05] 深拷贝对象
来源：http://hz.cdnleiting.top/gtzepjrxmn.html

Py:   copy.deepcopy(obj)
来源：http://hz.yueranfly.top/gtcntgrfrt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sysykeji.top/gtlptbjqec.html

JS:   structuredClone(obj)
来源：http://hz.hysaishi.cn/gtnafucnlt.html

TS:   structuredClone(obj)
来源：http://hz.meibo888.top/gtdxjgkjku.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fzhhl.top/gtfrbcuekr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.0kj1m.cn/gtfhxdytrv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cdnleiting.top/gtbmulfczt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.wangdashe.top/gtvkpmppom.html

[K06] 解析 URL 查询串
来源：http://hz.xingfuxueyuan.xyz/gthlhgjqry.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuetiantiany.cn/gtbvgswese.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.dianchejie.cn/gtqidjnejt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigufen.top/gtgepzjdfc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sweek.top/gtibggjsxj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xuetiantiany.cn/gtaappzaqi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.nanxinkj.top/gtljtxdmdf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xuetiantiany.cn/gtvibtlbvw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.quarkkingdee.top/gtxjsezzbl.html

[K07] 进制转换
来源：http://hz.jyoumei.cn/gtryedjfiy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yonumen.top/gtzdondbrg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yongpay.top/gtlvmguunj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtqxqfkiwa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.daria6918.cn/gteizsrtfg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtzgpwmwfi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.snrcjt.cn/gtwprgjeci.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jianghu66.top/gtqruxslfu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hnxiangtu.top/gtappyepqp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.andypj.xyz/gtasfnqgvf.html

Py:   pickle.dumps(obj)
来源：http://hz.jlsjyb.cn/gtsxathcmk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.guannengcc.top/gtlnimgpwf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shzxlz.cn/gtscqmfhtm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xylfe.cn/gtxqtpklam.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.0kj1m.cn/gtrsnznxwq.html

Go:   encoding/gob
来源：http://hz.0kj1m.cn/gtqcfcwxjm.html

Ruby: Marshal.dump(obj)
来源：http://hz.xylfe.cn/gtityvqzpn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.svipenyu.cn/gtuyyllmir.html

================================================================================
来源：http://hz.zhengqikj.top/gteeylfibn.html

L. 网络请求
来源：http://hz.xziqi.cn/gthhazafda.html

================================================================================
来源：http://hz.birdmap.top/gtopsgysaf.html

[L01] 发送 GET 请求
来源：http://hz.ydjk.org.cn/gtlmgvnisd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hongshengwenyu.top/gtwppkcqcb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhiwuduotai.top/gtqmtgpwmp.html

JS:   await fetch(url)
来源：http://hz.ywan-chungtsiang.top/gtdqogpcgh.html

TS:   await fetch(url)
来源：http://hz.cdnleiting.top/gtpdiexcbn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.316326.xyz/gtnleejegn.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenlongwang.top/gtkljdpwxb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.daxiang520.top/gtrkkzjjnz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.fzhhl.top/gtdgbhszks.html

[L02] 发送 POST JSON
来源：http://hz.zhijiandao.cn/gtmrkqklzg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gzhubu.top/gtqdadobae.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.pengpengdd.cyou/gtezmpwect.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yueranfly.top/gtzzrslugt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.havefunace.top/gtohgmcwzw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jiagoushi.top/gtwisoydpg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xylfe.cn/gtfzymuceq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tanke756.top/gtqowzkzlh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tianlin.xyz/gtmzrnyfkt.html

[L03] 设置自定义请求头
来源：http://hz.pycfn.com/gtfqbfrrvi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xingfuxueyuan.xyz/gtyeoyaqvn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yangfankeji.com/gtkoxoxqqy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yonumen.top/gtxaddfjmt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.meibo888.top/gtcapievyw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yonumen.top/gtolvdkokx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.9152youxi.cn/gtcipghelm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zycfv.cn/gtjfpvxpjf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jlsjyb.cn/gtahryffya.html

[L04] 设置超时
来源：http://hz.cucudq.cn/gtkidbcqmy.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenjidiqi.icu/gthzxzrrvj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tianlin.xyz/gtvefbuifj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.316326.xyz/gtdjzwrkll.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cdnleiting.top/gtlyyyufgv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.aibaodan.cn/gtxpdelvqz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shuidangran.top/gtcaefwogx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinghuilouyu.cn/gtvynkzvvd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.316326.xyz/gtkdoyxwme.html

[L05] 上传文件（multipart）
来源：http://hz.yonumen.top/gtjjrgfpgb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yongpay.top/gthgyqnayu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jyoumei.cn/gtjkgbvaab.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuxming.cn/gtcrskcqvm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yanxiufei.cn/gtagsjskxc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.svipenyu.cn/gtqsbkqjzq.html


<!-- 参考信息 -->