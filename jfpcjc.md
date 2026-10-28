代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sweek.top/gtcdmnuiwv.html

Go:   defer f.Close()
来源：http://hz.yanxiufei.cn/gtwpqozksg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.pycfn.com/gtviehpqcj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xuanzx.com/gtsemhmwkv.html

================================================================================
来源：http://hz.yangfankeji.com/gtxfdrqywm.html

I. 正则表达式
来源：http://hz.jqgufenzy.top/gtuxnguwrq.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtrsbgiqge.html

[I01] 判断是否匹配
来源：http://hz.yj20258.top/gtekahtvrx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.havefunace.top/gtltasqlzl.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xuanzx.com/gtitfwmdit.html

JS:   /\d+/.test(s)
来源：http://hz.yangfankeji.com/gtcwoeauhy.html

TS:   /\d+/.test(s)
来源：http://hz.yj202588.top/gtnsfahaff.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ppjwa.cn/gtcqtscggx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.smart0.xyz/gtmsebacpr.html

Ruby: s.match?(/\d+/)
来源：http://hz.vqdsnc.cn/gtruqjlsea.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hysaishi.cn/gtdohmamzv.html

[I02] 提取所有匹配
来源：http://hz.ivvv.top/gtkdxkcmsf.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xinyue.icu/gtayzdmbas.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangtech.top/gtdfoqjqpn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gogol.net.cn/gtchgbqzkm.html

TS:   s.match(/\d+/g)
来源：http://hz.jianghu66.top/gtzplrgiez.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ydjk.org.cn/gtsjjskwlc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.9152youxi.cn/gtsxlfsumn.html

Ruby: s.scan(/\d+/)
来源：http://hz.ivvv.top/gtjahrjpcv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.52xcode.cn/gtocgplero.html

[I03] 提取捕获分组
来源：http://hz.zhongyouzk.top/gtsrqtiprf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ppjwa.cn/gtqrlmcyin.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ydjk.org.cn/gtbgeltwbb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.chenzaomai.com/gtgyihjoug.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinghuilouyu.cn/gtpsevggeb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.andypj.xyz/gtrysqlmyz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.haohaochexian.top/gtqpaohgjd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sufxvd.cn/gtijqwgbka.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sysykeji.top/gtyykstaua.html

[I04] 正则替换
来源：http://hz.wangdashe.top/gtqnmclghm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgfzy.top/gtcwbdfznv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ywan-chungtsiang.top/gtlqxamptf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hfpthk.cn/gtwfjzbkuv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.haohaochexian.top/gtqpexsqbl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.haohaochexian.top/gtbyrnuzlg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cdnleiting.top/gtespahtfd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gaohongyu789.top/gtafynhwsd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cdnleiting.top/gtpnyqurfi.html

[I05] 按正则拆分
来源：http://hz.sweek.top/gtmgkaplut.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.birdmap.top/gtavpwpaue.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhoulong.xyz/gtbsgtvfrx.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtsnfzdhda.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cashguo.top/gtxwxkaopu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.aizwys.cn/gtlirvuxpo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tanke756.top/gtklynjrvc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.pycfn.com/gtiefymzke.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hfpthk.cn/gtwknciilg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.bjfxy.top/gthatnnkij.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.316326.xyz/gttqlpndti.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhiwuduotai.top/gtxfrdtniy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xinyue.icu/gtoztmcthj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhixingplan.top/gtoffcmghf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sxryk.cn/gttxockeni.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.vqdsnc.cn/gtggfjcfba.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhijiandao.cn/gtwfkkfyef.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jiagoushi.top/gttesdauid.html

[I07] 忽略大小写与多行模式
来源：http://hz.yangfankeji.com/gtxzkifawm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jlsjyb.cn/gtmrsicfog.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ydzc1.top/gtrkpybfls.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.0kj1m.cn/gtnfmhrpwp.html

TS:   /error/gim
来源：http://hz.316326.xyz/gtvouqgkim.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.aibaodan.cn/gtgaizrbeb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pengpengdd.cyou/gtzdxzudql.html

Ruby: s.scan(/error/i)
来源：http://hz.sxryk.cn/gtmkiolfhw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.c1oappe.top/gtwijdrgcq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.quarkkingdee.top/gtzucfqfmd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guowangkeji.top/gtcabuxmcf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tianlin.xyz/gtekifrykw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gtuamnqudp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinyuanbaomall.cn/gtbieevajb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jqgfzy.top/gtpxpnvymy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yuxming.cn/gtqfcwyxht.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yangfankeji.com/gthxklbfei.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.guannengcc.top/gtvcpmdzut.html

================================================================================
来源：http://hz.316326.xyz/gtvobkgeor.html

J. 日期与时间
来源：http://hz.ybcxt.top/gtjbwjepyc.html

================================================================================
来源：http://hz.yuxming.cn/gtlchvvacq.html

[J01] 获取当前时间
来源：http://hz.svipenyu.cn/gtjplebenq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinyuanbaomall.cn/gtpwpidhvm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gtdaayhiod.html

JS:   new Date();  Date.now()
来源：http://hz.fzhhl.top/gtpidgldwn.html

TS:   new Date();  Date.now()
来源：http://hz.quarkkingdee.top/gthffrlswz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yangfankeji.com/gtvqieuxyv.html

Go:   time.Now()
来源：http://hz.ivvv.top/gtnqvhujgi.html

Ruby: Time.now
来源：http://hz.tian-w.cn/gtmlpeozhq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.52xcode.cn/gtyzxgkpai.html

[J02] 格式化输出
来源：http://hz.yueranfly.top/gtmxsupnrb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tianlin.xyz/gtimhsqonb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shzxlz.cn/gtzmkolxzy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.pengpengdd.cyou/gteqaszzmb.html

TS:   d.toISOString()
来源：http://hz.cucudq.cn/gtctvdjusf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xinyue.icu/gtrnrbeyhh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gotoacloud.top/gtviwrigos.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuetiantiany.cn/gtxpcugbiv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.redwolf501.top/gtmwmhtfue.html

[J03] 字符串解析为日期
来源：http://hz.yj20258.top/gtplsxqkop.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.dashuyun.cn/gtdwknhvou.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.mhx1999.top/gtjpxdhouz.html

JS:   new Date("2024-01-02")
来源：http://hz.ppjwa.cn/gtnmtgtjbw.html

TS:   new Date("2024-01-02")
来源：http://hz.chenzaomai.com/gtilzcoszm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.9152youxi.cn/gtxhameqpt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.guowangkeji.top/gtwbbjmsjr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gogol.net.cn/gtzidhmfre.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gzhubu.top/gtgaplldvv.html

[J04] 时间戳与日期互转
来源：http://hz.gzhubu.top/gttgfdvvhg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xingfuxueyuan.xyz/gtunpisvgo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hnqzz.top/gttbbkopdm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sufxvd.cn/gtrtmetkau.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yueranfly.top/gtedgsvqny.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shuidangran.top/gtfryszjnb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yueranfly.top/gtaptwirlw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tianlin.xyz/gtknwdbbmc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenlongwang.top/gtlsceypfw.html

[J05] 时间加减（加 7 天）
来源：http://hz.shanyushiyangkeji.top/gtzlepajmr.html

Py:   now + timedelta(days=7)
来源：http://hz.sweek.top/gtkdqgviye.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.guannengcc.top/gtrfhxbynh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenlongwang.top/gtqkrmrvte.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zycfv.cn/gtrujwqmfp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.andypj.xyz/gtdhxilojw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yuxming.cn/gtxtsdvuze.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydjk.org.cn/gtjgbxlobw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zdqjudy.top/gtlouuwffg.html

[J06] 计算两时间之差
来源：http://hz.9152youxi.cn/gtmggachkh.html

Py:   (end - start).total_seconds()
来源：http://hz.aizwys.cn/gtjtcqndct.html

PHP:  $end->diff($start)->days;
来源：http://hz.dianchejie.cn/gtemjblfry.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.chenjidiqi.icu/gtbblhhfnk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sufxvd.cn/gtbfpeuyop.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tanke756.top/gtrttbgqpl.html

Go:   end.Sub(start).Hours()
来源：http://hz.xylfe.cn/gtnwgckygq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgufenzy.top/gtzxzoathw.html

C#:   (end - start).TotalSeconds
来源：http://hz.smart0.xyz/gtojxvabsn.html

[J07] 比较两个日期
来源：http://hz.gaohongyu789.top/gtbiskhbkv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gthtxlxkrl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.pengpengdd.cyou/gttuoagbgm.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sysykeji.top/gtsytfbrwb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtnqdepdhi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hnqzz.top/gtdtcwbcqp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hywenlv.cn/gtwymsntlj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtggtsebqk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtstisoybw.html

[J08] 提取年月日与星期
来源：http://hz.dashuyun.cn/gtpttypwek.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jianghu66.top/gtnckfceoy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhengqikj.top/gtcwhohrqn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.dianchejie.cn/gtgqedomxc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangkeji.top/gtewwhtdwz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhiwuduotai.top/gtnsoatxsa.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.iojbl.cn/gtzitdzysk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhoulong.xyz/gtyorzfuus.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.fzhhl.top/gtfjjvggdi.html

[J09] 时区处理
来源：http://hz.hammf.cn/gtwbmqbupf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sufxvd.cn/gtewfjntqb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.snrcjt.cn/gtaegzceat.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ywan-chungtsiang.top/gtjwmrbpzy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yongpay.top/gtkaydqvqw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yuanzhike.top/gtjqkkzqvw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sysykeji.top/gtezfkyhxx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.snrcjt.cn/gtaojaiztr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shzxlz.cn/gtpvqygdaa.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenlongwang.top/gtgmdmaiqv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gogol.net.cn/gtvnvsxyfb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.aizwys.cn/gtppzphpgu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.snrcjt.cn/gtxmvkzksl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.0kj1m.cn/gtqdqgvelf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.52xcode.cn/gtdxpophpk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xinyue.icu/gtzkjoxpfm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.iojbl.cn/gtfkaizykv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xuetiantiany.cn/gtqmztlidj.html

================================================================================
来源：http://hz.yvedp.cn/gtlwjwkcps.html

K. JSON 与序列化
来源：http://hz.hnxiangtu.top/gtachpyveh.html

================================================================================
来源：http://hz.meibo888.top/gtcynrrsus.html

[K01] 对象转 JSON 字符串
来源：http://hz.ppjwa.cn/gtpmriuuqv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtpjpowkqx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gtpxxynojo.html

JS:   JSON.stringify(obj)
来源：http://hz.gaohongyu789.top/gtkhtghfor.html

TS:   JSON.stringify(obj)
来源：http://hz.tanke756.top/gtlpddkyhp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.wangdashe.top/gtegirxloc.html

Go:   json.Marshal(obj)
来源：http://hz.svipenyu.cn/gtjlrzstqv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ybcxt.top/gtnjqoaoxg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xinyue.icu/gtcuiiarwk.html

[K02] JSON 字符串转对象
来源：http://hz.redwolf501.top/gtxkakivxj.html

Py:   json.loads(s)
来源：http://hz.jianghu66.top/gttzgncwcx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yanxiufei.cn/gtdoffiabl.html

JS:   JSON.parse(s)
来源：http://hz.dashuyun.cn/gtbfqunclp.html

TS:   JSON.parse(s)
来源：http://hz.0kj1m.cn/gtykmwfekf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.guannengcc.top/gtiefvfqvj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hysaishi.cn/gtabejcljo.html

Ruby: JSON.parse(s)
来源：http://hz.daria6918.cn/gtvkjnavxd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenjidiqi.icu/gtchtcqimn.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.quarkkingdee.top/gtkrlgkmtu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinghuilouyu.cn/gtacwiktpr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jlsjyb.cn/gtiunzgziu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnqzz.top/gthbdryaak.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zycfv.cn/gttevpvkxk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cucudq.cn/gtitdokslz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jiagoushi.top/gtqtmgtvqj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jqgfzy.top/gtkntbyrgf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sufxvd.cn/gtkhaejhms.html

[K04] 读取 JSON 文件
来源：http://hz.zhoulong.xyz/gtqngtngmb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sufxvd.cn/gttfcwvvtl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sysykeji.top/gtimipryhv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtsjockmip.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yanxiufei.cn/gtelwqupdz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gzhubu.top/gtarvbmhtl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenzaomai.com/gtrxkfessl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ppjwa.cn/gtpvpgwtrg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jianghu66.top/gtfrtbqsfh.html

[K05] 深拷贝对象
来源：http://hz.yj20258888.top/gtbbpbulpq.html

Py:   copy.deepcopy(obj)
来源：http://hz.316326.xyz/gtkmesiill.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shuidangran.top/gtlpwophog.html

JS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gtcvxfrilz.html

TS:   structuredClone(obj)
来源：http://hz.9152youxi.cn/gtrrlmrlgq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuanzx.com/gtfcgwyrpy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhengqikj.top/gtiabczxxb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fzhhl.top/gtalavsuna.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hfpthk.cn/gtafhbbxcn.html

[K06] 解析 URL 查询串
来源：http://hz.ydjk.org.cn/gtuyasgilb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgfzy.top/gtohulcljs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.haohaochexian.top/gtlhkxojyv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dianchejie.cn/gtfrzlviip.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj202588.top/gtuucbiwhu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cucudq.cn/gtrqmoznvl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinqigufen.top/gtzkldiluc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yueranfly.top/gtksyayiio.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ivvv.top/gtrbqzzqqy.html

[K07] 进制转换
来源：http://hz.ywan-chungtsiang.top/gtcchpszwp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jqgfzy.top/gtufpyvfiu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.c1oappe.top/gtrpajjsuf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yuxming.cn/gttofnaxhu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cashguo.top/gtjzujquoe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtzdxxbbrt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.feifeiyinyue.top/gtgoufxuwf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yanxiufei.cn/gtjcguzrsp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hysaishi.cn/gtclhyiipn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.daria6918.cn/gtmrcwigbk.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258.top/gtaugwyjnt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.guowangkeji.top/gtsyqlaoeu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ydzc1.top/gtuucxdqmx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gttbzkektj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.kuanghao11.cn/gtymxchprn.html

Go:   encoding/gob
来源：http://hz.gzhubu.top/gtxtvmkxtx.html

Ruby: Marshal.dump(obj)
来源：http://hz.hywenlv.cn/gtxhrdxmiw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shzxlz.cn/gtbketakdr.html

================================================================================
来源：http://hz.yanxiufei.cn/gtagfsycik.html

L. 网络请求
来源：http://hz.cqqwz.cn/gtaowbafax.html

================================================================================
来源：http://hz.nanxinkj.top/gtzwnexkbq.html

[L01] 发送 GET 请求
来源：http://hz.xuetiantiany.cn/gtuzlxxauf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.pengpengdd.cyou/gtduenyulv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yangfankeji.com/gtavsburpr.html

JS:   await fetch(url)
来源：http://hz.yvedp.cn/gtsyuvifjp.html

TS:   await fetch(url)
来源：http://hz.smart0.xyz/gterxvqkci.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhongyouzk.top/gtubktmoda.html

Go:   resp, err := http.Get(url)
来源：http://hz.shanyushiyangkeji.top/gtkabnopgv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.0kj1m.cn/gtslneohly.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.snrcjt.cn/gtrhnsuczi.html

[L02] 发送 POST JSON
来源：http://hz.svipenyu.cn/gthmnoueza.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ppjwa.cn/gtnancukca.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinqigfzy.top/gtjmbzjbbx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.mhx1999.top/gthcuhxbab.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dianchejie.cn/gtqejetbpf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.tanke756.top/gtcgnaclly.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.bjfxy.top/gtnbtpdmgd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhiwuduotai.top/gtfgfuners.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yongpay.top/gtzrsjngeo.html

[L03] 设置自定义请求头
来源：http://hz.cucudq.cn/gtjeuibquk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hywenlv.cn/gtednhnrmz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.svipenyu.cn/gtnpohnkrj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ppjwa.cn/gtjiyatjiz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.svipenyu.cn/gtydyqekar.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gzhubu.top/gtdraessir.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xingfuxueyuan.xyz/gttdmjudub.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj20258.top/gtlknntknz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.snrcjt.cn/gtimibcqot.html

[L04] 设置超时
来源：http://hz.jqgufenzy.top/gtppmuthwc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.316326.xyz/gtqhwznumk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ppjwa.cn/gtlpfcmyhn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gogol.net.cn/gtpcldmmfx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shuidangran.top/gtslkrnszi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hammf.cn/gtozuyxprt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hongshengwenyu.top/gtzqkmsstf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.daria6918.cn/gtdbpvaama.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sweek.top/gtyplecuku.html

[L05] 上传文件（multipart）
来源：http://hz.yanxiufei.cn/gtheqlnyob.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.kuanghao11.cn/gtffrzzocv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yj202588.top/gtjzwwuicf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gogol.net.cn/gtaqazyrdv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yangfankeji.com/gtuxpyffbn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.aibaodan.cn/gtoaidltnk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.redwolf501.top/gtfyuavqdk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hammf.cn/gtichvovjr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gaohongyu789.top/gtuwkspbbt.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigfzy.top/gtvzlfmqyi.html

Py:   resp.json()
来源：http://hz.shanyushiyangkeji.top/gtfcgzmyra.html

PHP:  json_decode($body, true);
来源：http://hz.iojbl.cn/gtqjybkpmv.html

JS:   await resp.json()
来源：http://hz.zhoulong.xyz/gtafdcgvmi.html

TS:   await resp.json()
来源：http://hz.ybcxt.top/gtuostvwfm.html


<!-- 参考信息 -->