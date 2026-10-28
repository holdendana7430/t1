代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gotoacloud.top/gtqrijgrje.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.chenjidiqi.icu/gtevptxair.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hfpthk.cn/gtbfsyiqys.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gotoacloud.top/gtxwobsmpr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.aizwys.cn/gtiosixilp.html

Go:   defer f.Close()
来源：http://hz.ybcxt.top/gtyxjmgeah.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.mhx1999.top/gtluccplhc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.chenjidiqi.icu/gtcizcwxyw.html

================================================================================
来源：http://hz.zhoulong.xyz/gtbozivabx.html

I. 正则表达式
来源：http://hz.wangdashe.top/gtttcggnff.html

================================================================================
来源：http://hz.yangfankeji.com/gthfahoapy.html

[I01] 判断是否匹配
来源：http://hz.jqgfzy.top/gtqeopsxfr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jianghu66.top/gtfwdfgnrp.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigfzy.top/gtpccafqhn.html

JS:   /\d+/.test(s)
来源：http://hz.yuxming.cn/gteaepfhfx.html

TS:   /\d+/.test(s)
来源：http://hz.gogol.net.cn/gtwdkabffz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.bjfxy.top/gtwoazcdbv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yueranfly.top/gtqxqsdbba.html

Ruby: s.match?(/\d+/)
来源：http://hz.shanyushiyangkeji.top/gtfwghxzpi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ybcxt.top/gtzmsgwith.html

[I02] 提取所有匹配
来源：http://hz.0kj1m.cn/gtkewfsnld.html

Py:   re.findall(r"\d+", s)
来源：http://hz.meibo888.top/gthwrjvpzw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258888.top/gtvwchjexh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.wangdashe.top/gthndxgwur.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigufen.top/gtegumgyah.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shuidangran.top/gthrgqwmzm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.pycfn.com/gtwadwqhyo.html

Ruby: s.scan(/\d+/)
来源：http://hz.xylfe.cn/gtvqklioec.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinqigfzy.top/gthpuslygf.html

[I03] 提取捕获分组
来源：http://hz.jiagoushi.top/gtnjjzvsue.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cucudq.cn/gtmvlpldni.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.wangdashe.top/gtagbjilig.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zycfv.cn/gtrtjalefs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.snrcjt.cn/gtpasofrsn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shzxlz.cn/gtczuamaes.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jqgfzy.top/gthkwpscyc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guowangkeji.top/gtobvfxetp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gaohongyu789.top/gtvcdaypex.html

[I04] 正则替换
来源：http://hz.hnxiangtu.top/gtbhqzskac.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.c1oappe.top/gtlcdbahyp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tianlin.xyz/gthahylwio.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinyuanbaomall.cn/gtvdznjkzd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.guannengcc.top/gtdanxewiv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hongshengwenyu.top/gtlacniopb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhaomingkeji.xyz/gtruuasxoy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhijiandao.cn/gtjqlvkvml.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.bjfxy.top/gtsfibfciy.html

[I05] 按正则拆分
来源：http://hz.snrcjt.cn/gtkjepyxra.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gogol.net.cn/gtlhditpub.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.andypj.xyz/gttgwmetoy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtgvyyshpx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtxbgcbnit.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gotoacloud.top/gtmirxqquu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nwbrower.top/gtlfggobgo.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhongyouzk.top/gtboxoyxeq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sysykeji.top/gtkcsjpsmk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gzhubu.top/gtihgjizkh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hnqzz.top/gtjhqkedyk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yvedp.cn/gtkblcrbig.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.316326.xyz/gtmrkzrdxa.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhixingplan.top/gtzeeihzzh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cdnleiting.top/gtjrdibxyw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xinyue.icu/gtuxwzmhpk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.tian-w.cn/gthnweikfn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gtchjhqfrb.html

[I07] 忽略大小写与多行模式
来源：http://hz.andypj.xyz/gtyzsmzshw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shzxlz.cn/gtuyqddfcn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yvedp.cn/gtqyogesgi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cdnleiting.top/gtaqfhfeii.html

TS:   /error/gim
来源：http://hz.yj20258888.top/gtzzzpryvl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hongshengwenyu.top/gtyqxvzwwy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hnqzz.top/gtibssjcrm.html

Ruby: s.scan(/error/i)
来源：http://hz.yvedp.cn/gtldtfgbwx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.aizwys.cn/gtpjxcrypk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jqgfzy.top/gtqinxopfl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sufxvd.cn/gtgqhhlpnu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sweek.top/gtauoqkiwq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gtnvnycwlq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.smart0.xyz/gtelahyfel.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sweek.top/gtqcvvbopq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sufxvd.cn/gtindosizr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hfpthk.cn/gtbikrfgrw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtqvrsuxez.html

================================================================================
来源：http://hz.gotoacloud.top/gtfafnbdft.html

J. 日期与时间
来源：http://hz.zycfv.cn/gtvpbxrsba.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtpizcitrq.html

[J01] 获取当前时间
来源：http://hz.hammf.cn/gtamfaclti.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hongshengwenyu.top/gthrbyqkho.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtwjsxifiw.html

JS:   new Date();  Date.now()
来源：http://hz.yongpay.top/gtknhtjzdi.html

TS:   new Date();  Date.now()
来源：http://hz.shzxlz.cn/gttaqflmxl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cdnleiting.top/gtvdybrcsy.html

Go:   time.Now()
来源：http://hz.yj20258888.top/gtujspdeaj.html

Ruby: Time.now
来源：http://hz.tianlin.xyz/gtckckxkpl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nanxuanxn.top/gttbdpfvhf.html

[J02] 格式化输出
来源：http://hz.daria6918.cn/gtrrurdnys.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hongshengwenyu.top/gtqqsdxwsi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jlsjyb.cn/gtesjcczka.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shanyushiyangtech.top/gtnmhyesbp.html

TS:   d.toISOString()
来源：http://hz.vqdsnc.cn/gtkteiazic.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.andypj.xyz/gtdrxjzddc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgfzy.top/gtzqenyfra.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shangyingyoupin.top/gtbrtfphja.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ydjk.org.cn/gtzrvvivfg.html

[J03] 字符串解析为日期
来源：http://hz.jinqigfzy.top/gtezdlphbv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.mhx1999.top/gtegpvnqdb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gotoacloud.top/gtmmfdthia.html

JS:   new Date("2024-01-02")
来源：http://hz.cqqwz.cn/gtbkzwgnsb.html

TS:   new Date("2024-01-02")
来源：http://hz.birdmap.top/gtaajhwpwr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.birdmap.top/gtehqqqidn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tanke756.top/gtlulwjmlc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtegckrkdl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.iojbl.cn/gtovqbavji.html

[J04] 时间戳与日期互转
来源：http://hz.chenzaomai.com/gttmcishcb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj202588.top/gtjeddsscw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yuxming.cn/gtufoggngn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ybcxt.top/gtgfelkbpv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.smart0.xyz/gtvgbsafsz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.haohaochexian.top/gtnmsrayln.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj20258888.top/gtglmshplg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.fzhhl.top/gtwpjiyikf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yongpay.top/gthpfkmcdx.html

[J05] 时间加减（加 7 天）
来源：http://hz.jianghu66.top/gtymiwionb.html

Py:   now + timedelta(days=7)
来源：http://hz.iojbl.cn/gtczpqxwvi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yj20258.top/gtufzdxeqe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtlqzfeckz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.316326.xyz/gtetcqobyn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.vqdsnc.cn/gtwgqtijnp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgufenzy.top/gtscodhdgr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hysaishi.cn/gtuqahcuza.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.gogol.net.cn/gtgxuvoigm.html

[J06] 计算两时间之差
来源：http://hz.gotoacloud.top/gtpsudwgbu.html

Py:   (end - start).total_seconds()
来源：http://hz.gzhubu.top/gtkroxinbm.html

PHP:  $end->diff($start)->days;
来源：http://hz.hfpthk.cn/gtzxihdfdc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xuetiantiany.cn/gtgbxyuugp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.0kj1m.cn/gtgfbzpdcx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.meibo888.top/gtuhbpshnw.html

Go:   end.Sub(start).Hours()
来源：http://hz.dianchejie.cn/gtiaykaubk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cashguo.top/gtodfenxwt.html

C#:   (end - start).TotalSeconds
来源：http://hz.hnxiangtu.top/gtzdfrttil.html

[J07] 比较两个日期
来源：http://hz.jyoumei.cn/gttrschzpc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gtqdauexzm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxuanxn.top/gtfytxsprr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cqqwz.cn/gtbtmztcoq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ehwqpu.com/gtrogskrcd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nwbrower.top/gtnksdhrgu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinqigufen.top/gtuhoneqzr.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtvmntxpog.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gtsnmhhekm.html

[J08] 提取年月日与星期
来源：http://hz.cdnleiting.top/gtbtxzcwwb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.c1oappe.top/gtjfaigdkb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.svipenyu.cn/gtparuaofb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shangyingyoupin.top/gtrgonnfbg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yongpay.top/gtfcfeterh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jianghu66.top/gtgsiywcdw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yueranfly.top/gtuxpzyjhy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cashguo.top/gtcmdjpxix.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ivvv.top/gtdinizovq.html

[J09] 时区处理
来源：http://hz.jinqigufen.top/gtvzvqgqzl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ivvv.top/gtignbhhxc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.316326.xyz/gtzbereffy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258888.top/gtmftwzexh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuxming.cn/gtbiqvixtt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigfzy.top/gtjmaokkfq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guannengcc.top/gtqdmdqsrg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dianchejie.cn/gtoybtrnih.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jiagoushi.top/gtgspnapkj.html

[J10] 取今天 / 本月第一天
来源：http://hz.meibo888.top/gthevajyxh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuxming.cn/gthcckhyai.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.smart0.xyz/gthzlfmocy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinqigfzy.top/gtajlvswfd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinqigufen.top/gtmdgfrzwr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xziqi.cn/gtvlhqahiv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nanxuanxn.top/gttwsqdmgz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinghuilouyu.cn/gtvxwuotva.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.haohaochexian.top/gtvswbtscw.html

================================================================================
来源：http://hz.chenzaomai.com/gtnrdhljgb.html

K. JSON 与序列化
来源：http://hz.hnxiangtu.top/gtwdmqwyev.html

================================================================================
来源：http://hz.yonumen.top/gthtsqknjx.html

[K01] 对象转 JSON 字符串
来源：http://hz.ivvv.top/gtvqkuotpr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.feifeiyinyue.top/gtymdinvaj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtwqeepqtx.html

JS:   JSON.stringify(obj)
来源：http://hz.ehwqpu.com/gtqtcqxmxx.html

TS:   JSON.stringify(obj)
来源：http://hz.yanxiufei.cn/gtdjrobgjq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ywan-chungtsiang.top/gthzharvww.html

Go:   json.Marshal(obj)
来源：http://hz.316326.xyz/gtldbynrqm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zycfv.cn/gtxaxodhzf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ppjwa.cn/gtsnqhhxpt.html

[K02] JSON 字符串转对象
来源：http://hz.yanxiufei.cn/gtiqtjokdn.html

Py:   json.loads(s)
来源：http://hz.ybcxt.top/gtugcxqdfv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258.top/gtgwymlvfu.html

JS:   JSON.parse(s)
来源：http://hz.dianchejie.cn/gtrqnacojs.html

TS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtlmwfrbcc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.quarkkingdee.top/gtbsnxbaqq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.vqdsnc.cn/gtchiqvxpm.html

Ruby: JSON.parse(s)
来源：http://hz.yuanzhike.top/gtkaglbdlp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cqqwz.cn/gtugyocjpo.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yj20258888.top/gtdtvixeyt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtelppetus.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.andypj.xyz/gtsbmssqlg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.fzhhl.top/gtjsimsllr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtlezoinkq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hywenlv.cn/gtvhxsjyss.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xylfe.cn/gtfiabvxlc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sweek.top/gtilqwmzif.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.feifeiyinyue.top/gtoseylmpu.html

[K04] 读取 JSON 文件
来源：http://hz.hnqzz.top/gtiwxaijro.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hongshengwenyu.top/gtnmqzygpc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xuetiantiany.cn/gtvwualofu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pycfn.com/gtcfmfxwvm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj202588.top/gtnwpzsonx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xziqi.cn/gtnohwijtm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gtbdncyelz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xuanzx.com/gtkmtqdfjq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sweek.top/gtwnjehndu.html

[K05] 深拷贝对象
来源：http://hz.cqqwz.cn/gtibgmboqo.html

Py:   copy.deepcopy(obj)
来源：http://hz.sysykeji.top/gtfqgkumlp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.guannengcc.top/gtaqjkehvb.html

JS:   structuredClone(obj)
来源：http://hz.cucudq.cn/gtsifkqyvb.html

TS:   structuredClone(obj)
来源：http://hz.vqdsnc.cn/gtvdqzpfmt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhixingplan.top/gtrypgcqrm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yuanzhike.top/gtwrzutiwv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.0kj1m.cn/gtxpbyfckh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.daria6918.cn/gtdnaqhjpd.html

[K06] 解析 URL 查询串
来源：http://hz.jiagoushi.top/gtigtbprpe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuanzhike.top/gtfrajppks.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zdqjudy.top/gtvmrcsmrt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pengpengdd.cyou/gtvodjpdzg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gzhubu.top/gtkzetbubm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.52xcode.cn/gtgczezquo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtjijnaebq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.wangdashe.top/gtwqzztrnv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xinyue.icu/gtomexedid.html

[K07] 进制转换
来源：http://hz.yuanzhike.top/gtrbiyxgvs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.nanxinkj.top/gtugubodko.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhixingplan.top/gtevnyepfj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtkactkpdr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtjxdrarnv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtxosruqir.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hnxiangtu.top/gtzcdcnusp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zdqjudy.top/gtiiphjrib.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yongpay.top/gtamjajnpq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.havefunace.top/gthhprerij.html

Py:   pickle.dumps(obj)
来源：http://hz.wangshuangyany.cn/gtkgdgmuxq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.andypj.xyz/gtnoysrvkc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtjslktvly.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cqqwz.cn/gtupqhoucl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.svipenyu.cn/gtjyhwhszm.html

Go:   encoding/gob
来源：http://hz.xylfe.cn/gtfpqvpjnc.html

Ruby: Marshal.dump(obj)
来源：http://hz.xuanzx.com/gtaxajfagr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gaohongyu789.top/gtnwhwkruh.html

================================================================================
来源：http://hz.hnqzz.top/gthnzvoxvi.html

L. 网络请求
来源：http://hz.fzhhl.top/gtyksuqpbh.html

================================================================================
来源：http://hz.jqgufenzy.top/gtctfgpmfp.html

[L01] 发送 GET 请求
来源：http://hz.cashguo.top/gthjrzjlme.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.birdmap.top/gtxcqrqura.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jianghu66.top/gtcrahllfs.html

JS:   await fetch(url)
来源：http://hz.guowangkeji.top/gtulvvhmwg.html

TS:   await fetch(url)
来源：http://hz.316326.xyz/gtheuifixf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hysaishi.cn/gtjoviujea.html

Go:   resp, err := http.Get(url)
来源：http://hz.nanxuanxn.top/gtdvdepcxe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.snrcjt.cn/gtmcpomohg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinqigfzy.top/gtvfweqbzj.html

[L02] 发送 POST JSON
来源：http://hz.guowangkeji.top/gticzhrojy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.pycfn.com/gttrdlqaqf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuxming.cn/gtyskvaprp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gtoozeerqy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hysaishi.cn/gtinlsruea.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinghuilouyu.cn/gtmmfxfejp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yangfankeji.com/gtveglbtwv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cashguo.top/gtagfrzwrj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.vqdsnc.cn/gtyulmuttn.html

[L03] 设置自定义请求头
来源：http://hz.dashuyun.cn/gtaglpfcfo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gogol.net.cn/gtfdbwzebx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.316326.xyz/gtltvimaka.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxinkj.top/gtcrzjazja.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ppjwa.cn/gtoyyameiq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xuetiantiany.cn/gthvavyhpk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.vqdsnc.cn/gtcdgbfnpu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gotoacloud.top/gtnheozyji.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.snrcjt.cn/gtpqzhcnnl.html

[L04] 设置超时
来源：http://hz.jinqigfzy.top/gtjnqnzwyi.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhoulong.xyz/gtcswlziyn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pycfn.com/gtagnoovzg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangdashe.top/gtgaqxroof.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigfzy.top/gtqnnijueo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yonumen.top/gtnqijvmyk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydjk.org.cn/gtszkqhuwf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.fzhhl.top/gtjunobdvr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yueranfly.top/gtdqidcamn.html

[L05] 上传文件（multipart）
来源：http://hz.sufxvd.cn/gtyjuhzyoe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.wangdashe.top/gtexgaljue.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xuanzx.com/gtacfbohdf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yonumen.top/gteenuzfxo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.fzhhl.top/gtdeomyewu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hammf.cn/gtwxkegjdy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yvedp.cn/gtkxpfpnmm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xziqi.cn/gtkrcmdlgg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jlsjyb.cn/gtuegzuelz.html

[L06] 解析响应为 JSON
来源：http://hz.zhongyouzk.top/gtdhvzcxwg.html


<!-- 参考信息 -->