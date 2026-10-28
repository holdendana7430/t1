代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.smart0.xyz/gtungmrbnn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.wangshuangyany.cn/gtyhuxljqs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.52xcode.cn/gtmrlwxmvm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuanzhike.top/gtzwcvuvlh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.daria6918.cn/gtalhcjudg.html

Go:   defer f.Close()
来源：http://hz.wangshuangyany.cn/gtqryxssat.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhijiandao.cn/gtbfckdojv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.haohaochexian.top/gtygrcbmvh.html

================================================================================
来源：http://hz.cqqwz.cn/gtefoppsxd.html

I. 正则表达式
来源：http://hz.yj20258888.top/gtmqftycmj.html

================================================================================
来源：http://hz.jinqigfzy.top/gtriojfoyf.html

[I01] 判断是否匹配
来源：http://hz.snrcjt.cn/gtlppwfdao.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtsdrgvyvd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.birdmap.top/gtjnvuvche.html

JS:   /\d+/.test(s)
来源：http://hz.ppjwa.cn/gtjuogxzwe.html

TS:   /\d+/.test(s)
来源：http://hz.jiagoushi.top/gtobzphlfp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhijiandao.cn/gtpnranhfb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ehwqpu.com/gtycynisby.html

Ruby: s.match?(/\d+/)
来源：http://hz.zdqjudy.top/gtdvbpzvtq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.nanxuanxn.top/gtvncliwii.html

[I02] 提取所有匹配
来源：http://hz.wangshuangyany.cn/gtgeldoyqf.html

Py:   re.findall(r"\d+", s)
来源：http://hz.316326.xyz/gtizypsbrv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gaohongyu789.top/gtbhsnbkrq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gaohongyu789.top/gtpwgxpdsk.html

TS:   s.match(/\d+/g)
来源：http://hz.xylfe.cn/gtvvqjpdhs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cdnleiting.top/gtfrqwtipu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.chenjidiqi.icu/gtwrnytjgi.html

Ruby: s.scan(/\d+/)
来源：http://hz.hysaishi.cn/gtcgtzjbxk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenjidiqi.icu/gtfhvrwdfq.html

[I03] 提取捕获分组
来源：http://hz.jqgufenzy.top/gtodcnblin.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.smart0.xyz/gtiytmymrh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yongpay.top/gtkupsuajj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hammf.cn/gtighxfkec.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xziqi.cn/gtbqqaiiub.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fengsongda.top/gttfihdibo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cqqwz.cn/gtfkrlyjlb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ehwqpu.com/gtcjxuflsx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xziqi.cn/gtouxviglp.html

[I04] 正则替换
来源：http://hz.hywenlv.cn/gtgjvxdinn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinghuilouyu.cn/gtmvmpapxa.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.fengsongda.top/gtjwiiuynf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.meibo888.top/gtcvbqfrio.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hongshengwenyu.top/gtzixtrkrj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.pycfn.com/gthsoozhty.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cucudq.cn/gtwonzjwig.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cheryme.top/gtvzahoimy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.aibaodan.cn/gtmwontbsj.html

[I05] 按正则拆分
来源：http://hz.yongpay.top/gtpunspyms.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xinyue.icu/gtzimsbjju.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tianlin.xyz/gtfterfubu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtewhynnhn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtrjautoju.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yj202588.top/gtbebatmji.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cheryme.top/gthccgtirj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtzzqtexyn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yj202588.top/gtzvpnipun.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cqqwz.cn/gtjxapipgv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.wangdashe.top/gtlqocjafg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sweek.top/gtixswrjqv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cdnleiting.top/gtputsofzp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gtfpjmtlvr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.9152youxi.cn/gttoqsvmxk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hongshengwenyu.top/gtkbmlutpo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhoulong.xyz/gtczfcmejr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.tianlin.xyz/gtmbvkhvno.html

[I07] 忽略大小写与多行模式
来源：http://hz.wangdashe.top/gtzkzdypth.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sweek.top/gtjvcafqus.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yuanzhike.top/gtihxueilv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.wangdashe.top/gtpsdhfotb.html

TS:   /error/gim
来源：http://hz.yanxiufei.cn/gtllgemivx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhongyouzk.top/gtvdumzuxb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gotoacloud.top/gtkcrxqmxd.html

Ruby: s.scan(/error/i)
来源：http://hz.vqdsnc.cn/gtfzeopoye.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.meibo888.top/gtjwmaywez.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cqqwz.cn/gtzdastjkt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cucudq.cn/gtuvektvko.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yj202588.top/gtciwnxioa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.c1oappe.top/gtqlrlvvza.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xylfe.cn/gtxlritmka.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zdqjudy.top/gtiqhdydyx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.wangshuangyany.cn/gtmlztatww.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.feifeiyinyue.top/gtckmvoaxz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.tian-w.cn/gtycodttqv.html

================================================================================
来源：http://hz.xylfe.cn/gtfsptiltj.html

J. 日期与时间
来源：http://hz.wangshuangyany.cn/gtbsyfqvbu.html

================================================================================
来源：http://hz.mhx1999.top/gtkrolkgdl.html

[J01] 获取当前时间
来源：http://hz.ehwqpu.com/gtgsjwwzjm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.daxiang520.top/gtfvswigpy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yueranfly.top/gtvysarcpv.html

JS:   new Date();  Date.now()
来源：http://hz.pengpengdd.cyou/gtovwpkopi.html

TS:   new Date();  Date.now()
来源：http://hz.nwbrower.top/gtvlyygtci.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.redwolf501.top/gtrffuurjm.html

Go:   time.Now()
来源：http://hz.gogol.net.cn/gttiuxmbtj.html

Ruby: Time.now
来源：http://hz.aibaodan.cn/gtmlhfrfnt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xinyue.icu/gtxusjpuut.html

[J02] 格式化输出
来源：http://hz.pycfn.com/gtosfjxgqa.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydjk.org.cn/gtaxvvbmki.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yvedp.cn/gtazsekfpn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xuanzx.com/gtdwhwvjfr.html

TS:   d.toISOString()
来源：http://hz.tian-w.cn/gtlfvfgmtg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shangyingyoupin.top/gtmfdalojr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tian-w.cn/gtjbnkbvaj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnqzz.top/gtqkccmtzw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigufen.top/gtgsrmhujk.html

[J03] 字符串解析为日期
来源：http://hz.daxiang520.top/gtdcegmvnh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.smart0.xyz/gtzovrwioi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hammf.cn/gtxnauhwfr.html

JS:   new Date("2024-01-02")
来源：http://hz.pycfn.com/gtqjtioreg.html

TS:   new Date("2024-01-02")
来源：http://hz.snrcjt.cn/gtkkwfvmbz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.aibaodan.cn/gtwnqmppib.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.svipenyu.cn/gtmgyrmhjh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ehwqpu.com/gtxiffkkbm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yueranfly.top/gtggsfgciv.html

[J04] 时间戳与日期互转
来源：http://hz.hfpthk.cn/gtkfeedsdo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jqgufenzy.top/gtsqtjjnig.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhijiandao.cn/gtodeqrnge.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhiwuduotai.top/gtjvvgcvsm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.aibaodan.cn/gtahqjpzpb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhixingplan.top/gtyxzwxfvt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.feifeiyinyue.top/gtzzswdmgl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tanke756.top/gttlaannhs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yonumen.top/gtlcezdufn.html

[J05] 时间加减（加 7 天）
来源：http://hz.yongpay.top/gtagcmdanm.html

Py:   now + timedelta(days=7)
来源：http://hz.hongshengwenyu.top/gtctlahyjc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.guannengcc.top/gtgkehpeue.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangshuangyany.cn/gtkcjupshd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtsndsxrdi.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.dashuyun.cn/gtfbuoswgr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sysykeji.top/gtgddexjzn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nanxinkj.top/gtrpwppgev.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xuetiantiany.cn/gtzwlwbzkr.html

[J06] 计算两时间之差
来源：http://hz.nanxuanxn.top/gthcflhurw.html

Py:   (end - start).total_seconds()
来源：http://hz.pycfn.com/gtfaqisjnq.html

PHP:  $end->diff($start)->days;
来源：http://hz.yanxiufei.cn/gtweeogkzg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.dashuyun.cn/gtzwubmbfi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.kuanghao11.cn/gtndjjylvn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj202588.top/gtxdvjxsmn.html

Go:   end.Sub(start).Hours()
来源：http://hz.dashuyun.cn/gtdoufrgod.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ppjwa.cn/gttldhpaxe.html

C#:   (end - start).TotalSeconds
来源：http://hz.ppjwa.cn/gtspqssnkc.html

[J07] 比较两个日期
来源：http://hz.jqgufenzy.top/gtfdszaref.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtrajjmwkn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xuetiantiany.cn/gtcxzbdgea.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.daxiang520.top/gtdhzqzqgz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtdwoqihij.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cheryme.top/gtqmxndydi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zdqjudy.top/gtidfamizh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yvedp.cn/gtqohfyxmr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jqgufenzy.top/gtgsqevodd.html

[J08] 提取年月日与星期
来源：http://hz.hfpthk.cn/gtagygiyxc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinyuanbaomall.cn/gtlqerismb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zycfv.cn/gtxidzpnzp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.birdmap.top/gtutocnrko.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinyuanbaomall.cn/gtspzvhlmn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hongshengwenyu.top/gtqlsuowof.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xuetiantiany.cn/gtcufxsknp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xingfuxueyuan.xyz/gtzurexwri.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nwbrower.top/gttotdwaco.html

[J09] 时区处理
来源：http://hz.jinqigfzy.top/gtmmudlyyq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.mhx1999.top/gtzrxntzfw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gaohongyu789.top/gtphqgxnbi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gzhubu.top/gtenvyxigm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigfzy.top/gtgngchvlb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jiagoushi.top/gtwtrmthxe.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nanxinkj.top/gtzbhqkeql.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.bjfxy.top/gtpogueiuv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shangyingyoupin.top/gtvmfngdwa.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenlongwang.top/gtlypxjvdm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.feifeiyinyue.top/gtrnuhofyk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sweek.top/gtvyihiurb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gogol.net.cn/gtdnywpanu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuanzhike.top/gtfreoxgke.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hammf.cn/gtzejfkszc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shzxlz.cn/gtyklitufq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sweek.top/gtijtuzgwm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jlsjyb.cn/gtyopuirnj.html

================================================================================
来源：http://hz.wangdashe.top/gtnadxbshw.html

K. JSON 与序列化
来源：http://hz.yj20258888.top/gtipbacgzy.html

================================================================================
来源：http://hz.tianlin.xyz/gtifiwkhaa.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinqigfzy.top/gthetifthx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cheryme.top/gtimmuhbzw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gtgrtenceh.html

JS:   JSON.stringify(obj)
来源：http://hz.52xcode.cn/gtilcovohg.html

TS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtuimtxxgx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.fzhhl.top/gtixwiivwy.html

Go:   json.Marshal(obj)
来源：http://hz.cucudq.cn/gtdhdgwdqa.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.feifeiyinyue.top/gtosnnfllo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sufxvd.cn/gtwqrfxihq.html

[K02] JSON 字符串转对象
来源：http://hz.shuidangran.top/gtlehbywed.html

Py:   json.loads(s)
来源：http://hz.xziqi.cn/gtpwegpgkw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.snrcjt.cn/gtxhqzmjfy.html

JS:   JSON.parse(s)
来源：http://hz.redwolf501.top/gtoqgxdojc.html

TS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtgptninjt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.52xcode.cn/gtrqzrbmfz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.meibo888.top/gtuhrqlrot.html

Ruby: JSON.parse(s)
来源：http://hz.haohaochexian.top/gtrpsrjacj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhengqikj.top/gtoqmksxfc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.birdmap.top/gtcfqavwco.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gtwxwuvmob.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shzxlz.cn/gtlrkszfuu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.dashuyun.cn/gtkwihilji.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gogol.net.cn/gtdbcyoinj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nwbrower.top/gthlwtdinb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xuanzx.com/gtzdsqeoew.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sufxvd.cn/gtzlbhjgzc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gotoacloud.top/gtzwahkeoy.html

[K04] 读取 JSON 文件
来源：http://hz.yanxiufei.cn/gtbetxzhva.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hnxiangtu.top/gtwxyxzzkr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gotoacloud.top/gtebkolwxi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xinyue.icu/gtxjdoiptf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ehwqpu.com/gtzofcscxx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.aibaodan.cn/gtwcocxkbp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gotoacloud.top/gtphdnnslo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hnxiangtu.top/gtwuhoexzn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dashuyun.cn/gtfwskapeb.html

[K05] 深拷贝对象
来源：http://hz.cheryme.top/gthqmosyjy.html

Py:   copy.deepcopy(obj)
来源：http://hz.ywan-chungtsiang.top/gtbjxramrn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gogol.net.cn/gtvqtvkzwu.html

JS:   structuredClone(obj)
来源：http://hz.chenlongwang.top/gtecnkybay.html

TS:   structuredClone(obj)
来源：http://hz.hfpthk.cn/gttqpvunnp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shzxlz.cn/gtmsnhzlml.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hywenlv.cn/gticfckkzk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cdnleiting.top/gtapxbtboa.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.wangdashe.top/gtninymqgf.html

[K06] 解析 URL 查询串
来源：http://hz.shuidangran.top/gtdphjbrsh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jiagoushi.top/gtsmuoawqh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ppjwa.cn/gtxkofrffm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhijiandao.cn/gtqvkbbqym.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.316326.xyz/gtxkmenyet.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jlsjyb.cn/gtaxktocvv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.nanxuanxn.top/gtmphpfbyy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.iojbl.cn/gtspnuajfx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.smart0.xyz/gticcuwxeg.html

[K07] 进制转换
来源：http://hz.shanyushiyangtech.top/gtpdbgpggx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yuanzhike.top/gtrgmbxbyr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shanyushiyangtech.top/gthxwlwqxz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtacqjdspt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtajbkfhqi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtaczndazz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xingfuxueyuan.xyz/gtxjyvtokg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhaomingkeji.xyz/gtganlkuqp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtgrjovube.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgfzy.top/gtgvgrrinh.html

Py:   pickle.dumps(obj)
来源：http://hz.tanke756.top/gtqwikhdtv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.0kj1m.cn/gtezgojqwk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhengqikj.top/gternawfhv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hnxiangtu.top/gtmxaygter.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ppjwa.cn/gtkgqjdypl.html

Go:   encoding/gob
来源：http://hz.c1oappe.top/gtczywhlzi.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhongyouzk.top/gtrqwtxuts.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.feifeiyinyue.top/gtroukswnf.html

================================================================================
来源：http://hz.gotoacloud.top/gtalpduuyb.html

L. 网络请求
来源：http://hz.jiagoushi.top/gtbtjchtcd.html

================================================================================
来源：http://hz.cucudq.cn/gtezluxqwz.html

[L01] 发送 GET 请求
来源：http://hz.ppjwa.cn/gtnquuchyj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenzaomai.com/gtahlwqkbt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jqgfzy.top/gtqwalrkvi.html

JS:   await fetch(url)
来源：http://hz.xylfe.cn/gtomsgcrsc.html

TS:   await fetch(url)
来源：http://hz.iojbl.cn/gtxxpqirwh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhijiandao.cn/gtjqepiaxw.html

Go:   resp, err := http.Get(url)
来源：http://hz.jianghu66.top/gtgajdluxn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cashguo.top/gtjcdkfzan.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ywan-chungtsiang.top/gtsiulguen.html

[L02] 发送 POST JSON
来源：http://hz.hongshengwenyu.top/gtyksqtycb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj20258.top/gtqgusrrub.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jqgufenzy.top/gtgfliapba.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtwerbwyoj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cashguo.top/gtxekhzpbl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258.top/gthssucuom.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xuetiantiany.cn/gtsbkhxmdf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sysykeji.top/gtmycupzrs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ivvv.top/gtcvnmuluv.html

[L03] 设置自定义请求头
来源：http://hz.cheryme.top/gtehneoizu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhengqikj.top/gtpenejzjm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hfpthk.cn/gtfdtreuyd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yueranfly.top/gtvasxrjep.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aizwys.cn/gtsvwtxezb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.9152youxi.cn/gtwuokokwt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sxryk.cn/gtddddmhkn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.wangshuangyany.cn/gtdqwtntgy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.vqdsnc.cn/gtmnggvmji.html

[L04] 设置超时
来源：http://hz.shanyushiyangtech.top/gtywnogjjv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenlongwang.top/gtxjjwtper.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tianlin.xyz/gtxjqvmaar.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gotoacloud.top/gtytrsrxiw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fzhhl.top/gtrehwsfda.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yj20258.top/gtfcwxwcnl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinqigfzy.top/gtbungnkng.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hnqzz.top/gtdhnzddyq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yuanzhike.top/gtdkcgssqq.html

[L05] 上传文件（multipart）
来源：http://hz.snrcjt.cn/gtdkfexful.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jianghu66.top/gtgdasswhq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.nwbrower.top/gturqesunx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydjk.org.cn/gtfxtwefla.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.aibaodan.cn/gtlwztkyxx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj20258.top/gtzqoeoivy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydjk.org.cn/gtndofsabd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.feifeiyinyue.top/gtaurexnhr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinqigfzy.top/gtjsqassis.html

[L06] 解析响应为 JSON
来源：http://hz.jqgfzy.top/gthqqnbdib.html


<!-- 参考信息 -->