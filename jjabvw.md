代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.316326.xyz/gtulslhqwg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xziqi.cn/gttcuyvsef.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxinkj.top/gtngvoears.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.smart0.xyz/gtbnmwyqze.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.vqdsnc.cn/gtlillnyrv.html

Go:   defer f.Close()
来源：http://hz.dashuyun.cn/gtkpvndtaw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yonumen.top/gtmluopscz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zycfv.cn/gtlwxzcwhc.html

================================================================================
来源：http://hz.yangfankeji.com/gtxrusxjzg.html

I. 正则表达式
来源：http://hz.hongshengwenyu.top/gtqjygqutk.html

================================================================================
来源：http://hz.gaohongyu789.top/gttndtyugj.html

[I01] 判断是否匹配
来源：http://hz.wangdashe.top/gtyhyinphc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sysykeji.top/gtkbqgpqxs.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenzaomai.com/gtavdaxsnv.html

JS:   /\d+/.test(s)
来源：http://hz.yuanzhike.top/gtosvhscuq.html

TS:   /\d+/.test(s)
来源：http://hz.jqgfzy.top/gtmzcpvtzp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shuidangran.top/gtsblzfqky.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ydzc1.top/gteybksnvi.html

Ruby: s.match?(/\d+/)
来源：http://hz.iojbl.cn/gtukaffzdc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.meibo888.top/gtzmiqlqby.html

[I02] 提取所有匹配
来源：http://hz.aizwys.cn/gttwjnvrdy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gogol.net.cn/gtrcoarqru.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.52xcode.cn/gtlbzwnlcn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.havefunace.top/gtvfjzxtsj.html

TS:   s.match(/\d+/g)
来源：http://hz.tanke756.top/gtmpjakmty.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ydjk.org.cn/gtnywkepng.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhiwuduotai.top/gtmequqwcl.html

Ruby: s.scan(/\d+/)
来源：http://hz.wangshuangyany.cn/gttuycxgsm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xylfe.cn/gtesiiapqt.html

[I03] 提取捕获分组
来源：http://hz.zhoulong.xyz/gtyoulnlfl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jiagoushi.top/gtlchijyce.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xziqi.cn/gtzusqpwdz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shzxlz.cn/gtzixpkfvo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shangyingyoupin.top/gtctulcqjj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.smart0.xyz/gtsntasyvy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.aizwys.cn/gtfgjgmszt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shanyushiyangtech.top/gtvvqkiuig.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.9152youxi.cn/gtyewadchh.html

[I04] 正则替换
来源：http://hz.ydzc1.top/gtdbniyszb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cqqwz.cn/gtdunvqfrb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhoulong.xyz/gtiurpcmsq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xuanzx.com/gtpkbrrxij.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gogol.net.cn/gtgmbdrnny.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinghuilouyu.cn/gtsenbtuwo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.pengpengdd.cyou/gtidfelhxf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shuidangran.top/gtclwxmgpt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhaomingkeji.xyz/gtioiazjwv.html

[I05] 按正则拆分
来源：http://hz.ywan-chungtsiang.top/gthelpexgd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xuanzx.com/gtemdjcwvy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhongyouzk.top/gthhccnult.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtmivgzwst.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtlpywrdmq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.aibaodan.cn/gtfcdfwuen.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.havefunace.top/gtxjyawsea.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtcujgbsnl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daxiang520.top/gtwbqbsjrt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jiagoushi.top/gtpwkgcsmc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hywenlv.cn/gtgotpwany.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jqgufenzy.top/gtcgxipisk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jyoumei.cn/gtowfaixlm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtankpnauj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hysaishi.cn/gtmleyhmgl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj202588.top/gtrewkcvse.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.52xcode.cn/gtpeqxkmtx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jqgufenzy.top/gtihdudvtp.html

[I07] 忽略大小写与多行模式
来源：http://hz.jlsjyb.cn/gtpiovqyyo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gzhubu.top/gttbxaxuvg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ppjwa.cn/gtzwyqbuyb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.kuanghao11.cn/gtlqansvxj.html

TS:   /error/gim
来源：http://hz.meibo888.top/gthsxabjrz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sweek.top/gtjivbgkrs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sufxvd.cn/gtfrtplatc.html

Ruby: s.scan(/error/i)
来源：http://hz.snrcjt.cn/gtcrfepfax.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shangyingyoupin.top/gtfxnmfyia.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhoulong.xyz/gtxbmnuomd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sxryk.cn/gtbhpsgsrl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ydjk.org.cn/gtwgqzjmyc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cdnleiting.top/gtcnpnitgu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hammf.cn/gtssgbhrif.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.aizwys.cn/gtszmmuxhx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sufxvd.cn/gtuwobrmpa.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj202588.top/gtiuenymwo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cdnleiting.top/gtcxsscprq.html

================================================================================
来源：http://hz.ydjk.org.cn/gtduxbgrrt.html

J. 日期与时间
来源：http://hz.nanxinkj.top/gtkwjvczon.html

================================================================================
来源：http://hz.yj202588.top/gtbdvmypnb.html

[J01] 获取当前时间
来源：http://hz.0kj1m.cn/gtdapqpqth.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.aibaodan.cn/gttwnmmtzg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xinyue.icu/gtijhjjxbd.html

JS:   new Date();  Date.now()
来源：http://hz.yuanzhike.top/gtpcjxyssg.html

TS:   new Date();  Date.now()
来源：http://hz.daxiang520.top/gtljfqvyxd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ydzc1.top/gtqtpwbnsr.html

Go:   time.Now()
来源：http://hz.haohaochexian.top/gtuptkkeof.html

Ruby: Time.now
来源：http://hz.zhoulong.xyz/gtppnjhvtl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hnxiangtu.top/gtacaqsxkh.html

[J02] 格式化输出
来源：http://hz.ivvv.top/gtlmwyommu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gtbluvzoxn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.wangshuangyany.cn/gtzswoybnx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.vqdsnc.cn/gtnrtqqqkm.html

TS:   d.toISOString()
来源：http://hz.cqqwz.cn/gtovmoqxgs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.svipenyu.cn/gtoaeonyqf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yueranfly.top/gtpxhzvxyf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangdashe.top/gtitdmyvfl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.birdmap.top/gtjujlaifw.html

[J03] 字符串解析为日期
来源：http://hz.zhoulong.xyz/gtfgqddsqp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgufenzy.top/gtiwkwjxzn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinghuilouyu.cn/gtgfcocrrw.html

JS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtmdqntqnd.html

TS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gtajtafsob.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtgbbpmedr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cashguo.top/gtggsgiszt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jqgfzy.top/gtpygqqdmw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tanke756.top/gtjeluuomv.html

[J04] 时间戳与日期互转
来源：http://hz.xuetiantiany.cn/gtjldjzbmh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tianlin.xyz/gtpubapker.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ydjk.org.cn/gtpffkluis.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigufen.top/gthkikydwp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.pycfn.com/gttmtmbkmv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhiwuduotai.top/gtxbjvqnoc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hnxiangtu.top/gtxjeqqzgf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.guannengcc.top/gtqlwezgep.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nanxinkj.top/gtlehmfkun.html

[J05] 时间加减（加 7 天）
来源：http://hz.guowangkeji.top/gtqrcnhiaw.html

Py:   now + timedelta(days=7)
来源：http://hz.jyoumei.cn/gtnkljblmk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ydzc1.top/gtpnkihxeb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guowangkeji.top/gtslckente.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigufen.top/gthkfbheum.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.sufxvd.cn/gtxkicrgot.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hfpthk.cn/gttkbcsitn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xylfe.cn/gtxjwxfstx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.chenjidiqi.icu/gtnohhllet.html

[J06] 计算两时间之差
来源：http://hz.zhijiandao.cn/gtxflfivov.html

Py:   (end - start).total_seconds()
来源：http://hz.jiagoushi.top/gtfmnnboql.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhengqikj.top/gtvxlqrusj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jlsjyb.cn/gtkhktadah.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj20258888.top/gtcpwmmwug.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.dashuyun.cn/gtmpflhwia.html

Go:   end.Sub(start).Hours()
来源：http://hz.havefunace.top/gtyqwcqvpi.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ydzc1.top/gtetfghdeq.html

C#:   (end - start).TotalSeconds
来源：http://hz.redwolf501.top/gtlpckemvz.html

[J07] 比较两个日期
来源：http://hz.nanxuanxn.top/gtpuxkrviu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtddrrdxia.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jiagoushi.top/gtndonfugi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtgnkjxxra.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtnmddclgq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.guowangkeji.top/gtppyhngrz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ywan-chungtsiang.top/gtesdhqjke.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtsumhgntm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jyoumei.cn/gtrksloqli.html

[J08] 提取年月日与星期
来源：http://hz.jinqigfzy.top/gtydmuywiw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.feifeiyinyue.top/gtnsbxzamr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yanxiufei.cn/gtttixeeja.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.316326.xyz/gtqmqwyxjl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinyuanbaomall.cn/gtpzhctcdd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hongshengwenyu.top/gtzcsbpmsg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.52xcode.cn/gtnjfqgiva.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hysaishi.cn/gtyyhladtw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.bjfxy.top/gtafcueknn.html

[J09] 时区处理
来源：http://hz.gotoacloud.top/gtmrcrcqqo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jqgfzy.top/gtlbqxpjmc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cdnleiting.top/gtvicxcmyi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuxming.cn/gthseupgur.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gtmmjxghjv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.dianchejie.cn/gtqiicqzkt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.kuanghao11.cn/gtwsflzmwd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ywan-chungtsiang.top/gtswwpgymp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.tianlin.xyz/gtlturvxsu.html

[J10] 取今天 / 本月第一天
来源：http://hz.cheryme.top/gtnvjxqumq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yangfankeji.com/gtazaiidjn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.andypj.xyz/gtqoucbvqu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yvedp.cn/gtodycdjhq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jianghu66.top/gtbnshxumc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shanyushiyangkeji.top/gtwrciijfu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zdqjudy.top/gtcediajjo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yangfankeji.com/gtkqpcaceh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj20258.top/gtrkokzibs.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwzbevift.html

K. JSON 与序列化
来源：http://hz.nanxuanxn.top/gtiksfbkux.html

================================================================================
来源：http://hz.yuanzhike.top/gtmrrsiulp.html

[K01] 对象转 JSON 字符串
来源：http://hz.nwbrower.top/gtxvducxzv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gtvfyghfdl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gtrarvovzr.html

JS:   JSON.stringify(obj)
来源：http://hz.9152youxi.cn/gtakiiwgac.html

TS:   JSON.stringify(obj)
来源：http://hz.gaohongyu789.top/gtjtcwmxdz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gzhubu.top/gtetjpeyev.html

Go:   json.Marshal(obj)
来源：http://hz.vqdsnc.cn/gtndcotvwl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.9152youxi.cn/gtblhrmrfz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hnxiangtu.top/gtihpbmmwf.html

[K02] JSON 字符串转对象
来源：http://hz.jinyuanbaomall.cn/gtqrxpwycq.html

Py:   json.loads(s)
来源：http://hz.feifeiyinyue.top/gttuqkyroj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cqqwz.cn/gtqbkjkigq.html

JS:   JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtbpouadvd.html

TS:   JSON.parse(s)
来源：http://hz.xuanzx.com/gtfoclfuob.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cheryme.top/gtpirloiik.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ivvv.top/gtpajzpnno.html

Ruby: JSON.parse(s)
来源：http://hz.redwolf501.top/gtmytzjqjm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.mhx1999.top/gtxgrqmolf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.fengsongda.top/gtreemkbry.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.daria6918.cn/gtnxhshahp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ydzc1.top/gtnwcpblpu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gtfvscbgqu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.haohaochexian.top/gtngcdmcut.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.pycfn.com/gtsqwcgvua.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jyoumei.cn/gtrqeknjbh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.fengsongda.top/gtsnsougcv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guowangkeji.top/gtstjkejiu.html

[K04] 读取 JSON 文件
来源：http://hz.0kj1m.cn/gtgolibxvr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jianghu66.top/gtoynyhziz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zdqjudy.top/gtgkoyxdic.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hongshengwenyu.top/gthtwytxog.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gogol.net.cn/gtiuretxqd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.feifeiyinyue.top/gtcsymzifs.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yuanzhike.top/gtkikyicgd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xziqi.cn/gtmwagdfbf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shanyushiyangkeji.top/gtahujrieo.html

[K05] 深拷贝对象
来源：http://hz.zhixingplan.top/gtujawzdzu.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinghuilouyu.cn/gtqcbtliio.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hnxiangtu.top/gtweiofryc.html

JS:   structuredClone(obj)
来源：http://hz.sysykeji.top/gtbhwuypqi.html

TS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtzbejgcfl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aibaodan.cn/gtbxpvxupx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nwbrower.top/gtitnpbzya.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.haohaochexian.top/gtuqwtkexq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgufenzy.top/gtocdhvnbp.html

[K06] 解析 URL 查询串
来源：http://hz.andypj.xyz/gtlkfwjikw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.kuanghao11.cn/gtheqvapfv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gaohongyu789.top/gtubotylcv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daxiang520.top/gtxxhutcny.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tianlin.xyz/gttzitdmif.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ivvv.top/gtpeukzvdm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gzhubu.top/gtzxzimqjs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.havefunace.top/gtydnfajqy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.redwolf501.top/gtqmxjvzpi.html

[K07] 进制转换
来源：http://hz.jqgufenzy.top/gtpdmfmlpc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.fzhhl.top/gtopfmnxcl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xingfuxueyuan.xyz/gtljvufhul.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nwbrower.top/gtjhkxchhd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtjhvwxsaa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtclcbbfvd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ybcxt.top/gtggrpqcak.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tanke756.top/gtprfcusuf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtaacwnbeh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nanxuanxn.top/gtcajazzgt.html

Py:   pickle.dumps(obj)
来源：http://hz.daria6918.cn/gtzmveaobn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinyuanbaomall.cn/gtzufejfys.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtvdhtjrlq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ybcxt.top/gtjpthiovc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.pycfn.com/gtqluagtmg.html

Go:   encoding/gob
来源：http://hz.ydjk.org.cn/gtawvwvkta.html

Ruby: Marshal.dump(obj)
来源：http://hz.aibaodan.cn/gthhgaevyy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.birdmap.top/gtghywamip.html

================================================================================
来源：http://hz.ehwqpu.com/gtakttovbw.html

L. 网络请求
来源：http://hz.yuxming.cn/gtebkcekbp.html

================================================================================
来源：http://hz.kuanghao11.cn/gtmgvhunxs.html

[L01] 发送 GET 请求
来源：http://hz.guowangkeji.top/gtkjxxnskx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tanke756.top/gtildujmgi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.dashuyun.cn/gtxvwqqbaz.html

JS:   await fetch(url)
来源：http://hz.daria6918.cn/gtrqpkuabr.html

TS:   await fetch(url)
来源：http://hz.shanyushiyangtech.top/gtrjqxxlqr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhixingplan.top/gtcuategfp.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhixingplan.top/gtjhbxkful.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.vqdsnc.cn/gtonjiqbum.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ivvv.top/gtfwgupoxw.html

[L02] 发送 POST JSON
来源：http://hz.fengsongda.top/gtzytyyrga.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tian-w.cn/gtioxlyzoe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xylfe.cn/gtfevasawx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gthtbxwryl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258.top/gteusmgpgk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sysykeji.top/gtrfkytusf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sufxvd.cn/gtdsnyarbn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gotoacloud.top/gtyqvumxjb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cheryme.top/gtbpgagbvh.html

[L03] 设置自定义请求头
来源：http://hz.tanke756.top/gtvkjevsbk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shzxlz.cn/gtzxsxqsrg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhongyouzk.top/gtxbzcmiio.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydzc1.top/gtptzhwuel.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.kuanghao11.cn/gtahlkkrjg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gaohongyu789.top/gtmulctqih.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yj20258.top/gtobgmqxfn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.mhx1999.top/gtoidpaefm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ppjwa.cn/gthkyqhgux.html

[L04] 设置超时
来源：http://hz.yuanzhike.top/gtjvgrugko.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yanxiufei.cn/gtmodapbuo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jqgfzy.top/gtcfukhxdi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xinyue.icu/gtdsqqbqdr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ybcxt.top/gtkommcgvh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.havefunace.top/gtykfxxufq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yanxiufei.cn/gtdftxuown.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yonumen.top/gtocyojmyk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yonumen.top/gtodihbcur.html

[L05] 上传文件（multipart）
来源：http://hz.nanxinkj.top/gtykjcarrv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinghuilouyu.cn/gtmcpfffjh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.chenlongwang.top/gttbkvpkad.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.pycfn.com/gtbbptzwwe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gotoacloud.top/gtbfyyfwhz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yanxiufei.cn/gtipayblff.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shanyushiyangtech.top/gtwhrwvbft.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.daria6918.cn/gtwqrclhwr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenzaomai.com/gtslycuork.html

[L06] 解析响应为 JSON
来源：http://hz.bjfxy.top/gtcvmwkuna.html


<!-- 参考信息 -->