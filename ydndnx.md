代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydjk.org.cn/gtxzkwmugo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ppjwa.cn/gtuzpbpzsp.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhixingplan.top/gtdmhbjvbu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.9152youxi.cn/gthzwuebge.html

[I02] 提取所有匹配
来源：http://hz.haohaochexian.top/gtjvrdagsr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.fzhhl.top/gtlumjaoiv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ppjwa.cn/gtcuaeedwn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.wangdashe.top/gtjqxlsbrq.html

TS:   s.match(/\d+/g)
来源：http://hz.daria6918.cn/gtzpsgqwiw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.dianchejie.cn/gtaegsglse.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.havefunace.top/gtxuspdlhl.html

Ruby: s.scan(/\d+/)
来源：http://hz.feifeiyinyue.top/gtpzzheilw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.0kj1m.cn/gteafewmkt.html

[I03] 提取捕获分组
来源：http://hz.iojbl.cn/gtlvyzuvbg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.snrcjt.cn/gtdcaamdbw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zycfv.cn/gtchxhhlva.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.guannengcc.top/gtfvevkvfa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hfpthk.cn/gttfbibuhv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.birdmap.top/gtawuuvcrh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj20258.top/gtbgenclvt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xylfe.cn/gtiyteddif.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.wangshuangyany.cn/gtbreexles.html

[I04] 正则替换
来源：http://hz.bjfxy.top/gtaabqubaa.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinqigfzy.top/gtpmhejafr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.feifeiyinyue.top/gtipbrslmf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtdwbgteba.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhiwuduotai.top/gtqhfwnaii.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhengqikj.top/gtrponcejx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shangyingyoupin.top/gtikhaftgx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ywan-chungtsiang.top/gtbkuwnfvo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hysaishi.cn/gtxmoozzww.html

[I05] 按正则拆分
来源：http://hz.zhongyouzk.top/gtjmgtvxwp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ydjk.org.cn/gttzejvqfz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hnxiangtu.top/gtnyzriwxv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtkbawrqjg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gtgskvlayp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhiwuduotai.top/gtfsazoaqh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.meibo888.top/gtlijogtbo.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtewjictqa.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhongyouzk.top/gtvhwzbyjl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.vqdsnc.cn/gtkxjmjjpb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sysykeji.top/gtuxgrobuh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ybcxt.top/gtukygfggu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yonumen.top/gtubitblgr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtcvpxhlcv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nwbrower.top/gtcqreaeln.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinghuilouyu.cn/gtyzdkmkpn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guowangkeji.top/gtdrarixla.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.fengsongda.top/gttsbjmfgf.html

[I07] 忽略大小写与多行模式
来源：http://hz.nwbrower.top/gtimoikjdh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj20258888.top/gtwwcrpeos.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yonumen.top/gtoijwochc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.svipenyu.cn/gtqyacwecs.html

TS:   /error/gim
来源：http://hz.svipenyu.cn/gtesgpxhgy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cdnleiting.top/gtpyfhhuvv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj20258.top/gtnxvjljiq.html

Ruby: s.scan(/error/i)
来源：http://hz.tianlin.xyz/gtoxyneldw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258.top/gtotjsgcph.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuanzhike.top/gtokhpdmmo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sweek.top/gtdrwfswbr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigfzy.top/gttvvctgem.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtmjlkrxxg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gtivtfatrb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.dashuyun.cn/gtweaacwij.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.feifeiyinyue.top/gtnoswedxe.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yonumen.top/gtirhkvaiv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxinkj.top/gtuaolxgnq.html

================================================================================
来源：http://hz.ydzc1.top/gtcwuwuxdx.html

J. 日期与时间
来源：http://hz.ivvv.top/gtxqcgriry.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtwnucaqgo.html

[J01] 获取当前时间
来源：http://hz.chenzaomai.com/gtevdwtpyj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.iojbl.cn/gtkgqipkrj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gotoacloud.top/gtvoyuufyk.html

JS:   new Date();  Date.now()
来源：http://hz.zhixingplan.top/gtddsjcnbx.html

TS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtbujynuez.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xingfuxueyuan.xyz/gtqboaottg.html

Go:   time.Now()
来源：http://hz.shzxlz.cn/gtjwyczlvq.html

Ruby: Time.now
来源：http://hz.mhx1999.top/gtheyjwqel.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ywan-chungtsiang.top/gtsfckrchq.html

[J02] 格式化输出
来源：http://hz.smart0.xyz/gtycbewlak.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gttjealtwc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.wangdashe.top/gtpflmfkqq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.c1oappe.top/gtfeqwcbbo.html

TS:   d.toISOString()
来源：http://hz.cheryme.top/gtpsqvmcba.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinqigufen.top/gtjxvkzfnw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.vqdsnc.cn/gtbjjibqhs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xingfuxueyuan.xyz/gtaxmnnzzm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhoulong.xyz/gtwgqlxyix.html

[J03] 字符串解析为日期
来源：http://hz.yuxming.cn/gtnirvbduq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jyoumei.cn/gtjnyiodgg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hysaishi.cn/gtothciyeg.html

JS:   new Date("2024-01-02")
来源：http://hz.zhengqikj.top/gtywtpgyel.html

TS:   new Date("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtrbaxhzdc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ppjwa.cn/gtggroooup.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shzxlz.cn/gtczlmbftl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jiagoushi.top/gtobxzntww.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.havefunace.top/gtfjsadkhk.html

[J04] 时间戳与日期互转
来源：http://hz.zycfv.cn/gtudoigtvz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hammf.cn/gtzsfxfygx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zycfv.cn/gtyrazqfld.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinyuanbaomall.cn/gtymkrhvng.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ywan-chungtsiang.top/gtsezmamcm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yuxming.cn/gtuxtghsif.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.9152youxi.cn/gtzwmaftlj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.aizwys.cn/gtwfplviuj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gogol.net.cn/gtxzrlnfar.html

[J05] 时间加减（加 7 天）
来源：http://hz.yueranfly.top/gtzrenrtnx.html

Py:   now + timedelta(days=7)
来源：http://hz.nanxuanxn.top/gtlpnxjvej.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.snrcjt.cn/gtltvcqbpw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hywenlv.cn/gtdownmhvo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gogol.net.cn/gtzrqrrvil.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xinyue.icu/gtnuksvcok.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yuxming.cn/gtmamruxkx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.andypj.xyz/gtjusmpwyo.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.andypj.xyz/gtsaxlsvqo.html

[J06] 计算两时间之差
来源：http://hz.ybcxt.top/gthtrpxjuv.html

Py:   (end - start).total_seconds()
来源：http://hz.hywenlv.cn/gtaipmijzy.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj20258.top/gttsxvcuuw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhixingplan.top/gtiwxyndnj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sweek.top/gtbixwwxsh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zdqjudy.top/gtngeswohr.html

Go:   end.Sub(start).Hours()
来源：http://hz.tanke756.top/gtkolllthy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinghuilouyu.cn/gtfatdhxzd.html

C#:   (end - start).TotalSeconds
来源：http://hz.hnqzz.top/gtjnndskeq.html

[J07] 比较两个日期
来源：http://hz.316326.xyz/gtkyrnezel.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtjderhzba.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.0kj1m.cn/gtzlelfksu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.9152youxi.cn/gttqjpbyps.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ybcxt.top/gtgszqbezl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zycfv.cn/gtlhwsuoxz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhengqikj.top/gtuoclpudv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtbtvyiqxe.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtnqkuwrpw.html

[J08] 提取年月日与星期
来源：http://hz.yanxiufei.cn/gtyiawpnle.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.wangdashe.top/gthgngzryv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj202588.top/gtxiydguvv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nwbrower.top/gtljukcmdz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xingfuxueyuan.xyz/gtafplqxib.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.nwbrower.top/gtpfwwapsi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.iojbl.cn/gtukchpllt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.iojbl.cn/gtwjcpuaov.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jlsjyb.cn/gthkphysbz.html

[J09] 时区处理
来源：http://hz.c1oappe.top/gtjoxumenq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yvedp.cn/gtvjtmeizk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhoulong.xyz/gtwxrsmepe.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangtech.top/gtmcyxnwlx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aibaodan.cn/gtchccaihs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sweek.top/gtdoycpjjj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yuanzhike.top/gtvvnymfno.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shanyushiyangkeji.top/gtxqhuiwpz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cdnleiting.top/gtsweislhu.html

[J10] 取今天 / 本月第一天
来源：http://hz.yongpay.top/gtfhwrohbb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tianlin.xyz/gtpkftzzun.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ydzc1.top/gtdwcvcvky.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ivvv.top/gtbdviheca.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ybcxt.top/gtwbgxigbz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nanxuanxn.top/gtszxxbgbi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.mhx1999.top/gtcyhmtmot.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinyuanbaomall.cn/gtrokuglbj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.birdmap.top/gtcmyqyybm.html

================================================================================
来源：http://hz.hnxiangtu.top/gtrvewgame.html

K. JSON 与序列化
来源：http://hz.iojbl.cn/gtzkilycww.html

================================================================================
来源：http://hz.hnqzz.top/gtjjepxdau.html

[K01] 对象转 JSON 字符串
来源：http://hz.fzhhl.top/gtgumthqmw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yvedp.cn/gtpklrbixv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.aibaodan.cn/gtxkmkdxti.html

JS:   JSON.stringify(obj)
来源：http://hz.gogol.net.cn/gtgzwrmoze.html

TS:   JSON.stringify(obj)
来源：http://hz.zhaomingkeji.xyz/gtkyojshnx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xinyue.icu/gtoygiwufd.html

Go:   json.Marshal(obj)
来源：http://hz.pengpengdd.cyou/gtryhcpkre.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jyoumei.cn/gtyewkufkv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.bjfxy.top/gtcbuomnfc.html

[K02] JSON 字符串转对象
来源：http://hz.cashguo.top/gtfkmqdlcu.html

Py:   json.loads(s)
来源：http://hz.hysaishi.cn/gtvqxsbwmk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinqigfzy.top/gtqvchihjt.html

JS:   JSON.parse(s)
来源：http://hz.zycfv.cn/gtbczuzmun.html

TS:   JSON.parse(s)
来源：http://hz.chenzaomai.com/gtbiewfgyo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gzhubu.top/gtmqysfirs.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtidbnsopw.html

Ruby: JSON.parse(s)
来源：http://hz.xinyue.icu/gtganbslbb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinyuanbaomall.cn/gtqmynkbka.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sysykeji.top/gtmayojgxn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtolrfottm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnxiangtu.top/gtvfasjdjm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.fzhhl.top/gtivzuzdjk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtrfcjhobj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sufxvd.cn/gteeqwmqzo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cheryme.top/gthzsngpuv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxinkj.top/gtvtbnrmdj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sufxvd.cn/gtksnhrons.html

[K04] 读取 JSON 文件
来源：http://hz.jinghuilouyu.cn/gtngiuxvne.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sufxvd.cn/gteaealgrv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.aibaodan.cn/gtgblhatus.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtvcjbfmze.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.bjfxy.top/gtohykxblz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shuidangran.top/gtsjojfpbt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jqgfzy.top/gttynyofdw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gzhubu.top/gtbhgfslgt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shzxlz.cn/gttspnxeki.html

[K05] 深拷贝对象
来源：http://hz.xuanzx.com/gtsgjfssim.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxuanxn.top/gtqszmceuv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.c1oappe.top/gthiemnxgb.html

JS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gttywuydyv.html

TS:   structuredClone(obj)
来源：http://hz.yj20258888.top/gtacorfqvj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.nanxinkj.top/gtbrtwlkkj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hysaishi.cn/gtdokyexmr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ywan-chungtsiang.top/gtqwnwlicl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sweek.top/gtausmqtnw.html

[K06] 解析 URL 查询串
来源：http://hz.cdnleiting.top/gtutfvlexl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.smart0.xyz/gtvvgiamzw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ybcxt.top/gtnqaqhmlp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jianghu66.top/gtzstzlgie.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yangfankeji.com/gtosvwxwox.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hywenlv.cn/gtcrxdpiwt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hnqzz.top/gtrlyfhgmb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtqndbpgtx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gzhubu.top/gtkpfegezm.html

[K07] 进制转换
来源：http://hz.sxryk.cn/gtfkdyhbtz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zdqjudy.top/gtnjrxrqnd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nwbrower.top/gtoqiseuxs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtqmkrghbs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtnlvyfkdx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtgxdhbhds.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinghuilouyu.cn/gtwjbowiis.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jyoumei.cn/gtroqvjqqp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.0kj1m.cn/gtgtynevto.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gotoacloud.top/gtdfohpzzf.html

Py:   pickle.dumps(obj)
来源：http://hz.chenjidiqi.icu/gtrrzkcilp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shzxlz.cn/gtjpllcobe.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jlsjyb.cn/gtgtiihgkw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.52xcode.cn/gtqmetqrkh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.c1oappe.top/gtlvxvqjem.html

Go:   encoding/gob
来源：http://hz.snrcjt.cn/gtzyhrawzj.html

Ruby: Marshal.dump(obj)
来源：http://hz.haohaochexian.top/gtehtzqekz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shuidangran.top/gtlcmbtpgz.html

================================================================================
来源：http://hz.cqqwz.cn/gtcspogugb.html

L. 网络请求
来源：http://hz.daria6918.cn/gtbhebsjnh.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtetlelvzx.html

[L01] 发送 GET 请求
来源：http://hz.cashguo.top/gtcrtkligx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.vqdsnc.cn/gtfwfeftqr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cashguo.top/gticdednzj.html

JS:   await fetch(url)
来源：http://hz.gzhubu.top/gtmdtgxdit.html

TS:   await fetch(url)
来源：http://hz.haohaochexian.top/gtrmbyioha.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.guowangkeji.top/gtlijfremx.html

Go:   resp, err := http.Get(url)
来源：http://hz.jqgfzy.top/gtbdehhqfv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinqigfzy.top/gtkoegrjef.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hywenlv.cn/gtiymjbepl.html

[L02] 发送 POST JSON
来源：http://hz.jqgufenzy.top/gtwizwubva.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guannengcc.top/gtffduxqkj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shzxlz.cn/gtreyouibw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aizwys.cn/gtgrtmlasc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnqzz.top/gtvjowdfve.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.birdmap.top/gtwaasqvoh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xuanzx.com/gtlmptkgbp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.haohaochexian.top/gtjfkfobym.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.wangshuangyany.cn/gtycfjsxgx.html

[L03] 设置自定义请求头
来源：http://hz.zhoulong.xyz/gtvrafyvrk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jqgfzy.top/gtvhanezdi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ydzc1.top/gtggxvqswm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuanzhike.top/gtmxiesogb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtiwzkyscc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yvedp.cn/gtqlsrepzm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinghuilouyu.cn/gttwmqwnud.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yuanzhike.top/gtumcbtaph.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.c1oappe.top/gtmwxxftbg.html

[L04] 设置超时
来源：http://hz.yuxming.cn/gtybgomjop.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jianghu66.top/gtxcrdbtzo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ywan-chungtsiang.top/gtcjuseodk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ivvv.top/gtoaduytyg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.iojbl.cn/gtznwlhrvn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.guannengcc.top/gtczsdydbp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cheryme.top/gtwxnhqjkv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ehwqpu.com/gtwwqrpzwp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cqqwz.cn/gthhatarhz.html

[L05] 上传文件（multipart）
来源：http://hz.c1oappe.top/gtjanxupjx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shuidangran.top/gtrbmjutip.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.mhx1999.top/gtqlkeooee.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangshuangyany.cn/gthvkcukjl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hysaishi.cn/gtfhudieep.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.aizwys.cn/gtzrwntqzz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.snrcjt.cn/gtprklfrrs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhixingplan.top/gtxpztdmev.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jiagoushi.top/gtuwgzqlvb.html

[L06] 解析响应为 JSON
来源：http://hz.yanxiufei.cn/gtiexybjld.html

Py:   resp.json()
来源：http://hz.zdqjudy.top/gtacubwcaf.html

PHP:  json_decode($body, true);
来源：http://hz.zhijiandao.cn/gtfqezhnni.html

JS:   await resp.json()
来源：http://hz.jyoumei.cn/gtumterbto.html

TS:   await resp.json()
来源：http://hz.zhixingplan.top/gthdljtrel.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.daxiang520.top/gtkqebpoeq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dashuyun.cn/gtdicscykz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhengqikj.top/gtdztbqwer.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zycfv.cn/gtcidjakkm.html

[L07] 处理 HTTP 状态码
来源：http://hz.tianlin.xyz/gtvaaccaak.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cashguo.top/gtcxnwgyes.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hysaishi.cn/gtzfzduvxn.html

JS:   resp.ok;  resp.status
来源：http://hz.hnxiangtu.top/gtttvdxqhs.html

TS:   resp.ok;  resp.status
来源：http://hz.jiagoushi.top/gtyhsfcqzz.html

Java: resp.statusCode()
来源：http://hz.zdqjudy.top/gtnhbhrpko.html

Go:   resp.StatusCode
来源：http://hz.zhixingplan.top/gtcdsgfwqf.html

Ruby: resp.code.to_i
来源：http://hz.gzhubu.top/gtlsyfeeoh.html


<!-- 参考信息 -->