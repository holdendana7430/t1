代发 wailian999

================================================================================
来源：http://hz.sweek.top/gtpeyldtws.html

I. 正则表达式
来源：http://hz.sysykeji.top/gtoaogzkcw.html

================================================================================
来源：http://hz.guowangkeji.top/gtvourfyxc.html

[I01] 判断是否匹配
来源：http://hz.dianchejie.cn/gtphwpbjzp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shuidangran.top/gtphzuifxb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dianchejie.cn/gtntddojaj.html

JS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtfjdcxvev.html

TS:   /\d+/.test(s)
来源：http://hz.gotoacloud.top/gtlfkudcbi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.dianchejie.cn/gtdnofljgl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shanyushiyangtech.top/gtuismrndm.html

Ruby: s.match?(/\d+/)
来源：http://hz.haohaochexian.top/gtizeozhou.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sweek.top/gtjtrsqmfb.html

[I02] 提取所有匹配
来源：http://hz.tianlin.xyz/gtlklgrisg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.quarkkingdee.top/gtieifkvbs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hywenlv.cn/gtdxiynkrm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhiwuduotai.top/gtbgwjxelk.html

TS:   s.match(/\d+/g)
来源：http://hz.0kj1m.cn/gtsjiaszwq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jyoumei.cn/gtpgpeutoq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.quarkkingdee.top/gtpbebypbn.html

Ruby: s.scan(/\d+/)
来源：http://hz.jiagoushi.top/gtxaoamvcv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.c1oappe.top/gtecdprals.html

[I03] 提取捕获分组
来源：http://hz.dianchejie.cn/gtuizxihrk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhijiandao.cn/gtrjtrbidt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinqigufen.top/gtnrvzbfdx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhongyouzk.top/gtfoynqgig.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.havefunace.top/gtdpuaxcdt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.9152youxi.cn/gtoehqjafk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinyuanbaomall.cn/gtsnhcxkor.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhengqikj.top/gteispyzty.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ybcxt.top/gtzraiepnl.html

[I04] 正则替换
来源：http://hz.tanke756.top/gtddoosfol.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sufxvd.cn/gtogiktpin.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258.top/gttfkrdfij.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gturvcusmr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigufen.top/gtiptcwvmx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.daria6918.cn/gtzsaxmush.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhoulong.xyz/gtioedpyca.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yongpay.top/gtcznypeam.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yj20258.top/gtrhuakohw.html

[I05] 按正则拆分
来源：http://hz.nwbrower.top/gtdypgeviu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.vqdsnc.cn/gtsjzzygks.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yangfankeji.com/gtznovwaud.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtsaxhfnkh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhoulong.xyz/gtduuwovvo.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jiagoushi.top/gtpykqzmcg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenlongwang.top/gteifogyry.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gtywtlugfe.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.pycfn.com/gtrwavxkds.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.dashuyun.cn/gtwecbdrpc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.haohaochexian.top/gtcgedoatt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnxiangtu.top/gtcxyplehn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daria6918.cn/gtowbxqgtz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shzxlz.cn/gtnerqbasu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.iojbl.cn/gtoebivcci.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jiagoushi.top/gtvoxrutvs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daria6918.cn/gtaqefzcmj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gtzqxqkbst.html

[I07] 忽略大小写与多行模式
来源：http://hz.snrcjt.cn/gtripdtcnr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ydzc1.top/gtbdcqedtt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nanxinkj.top/gtcqonzmif.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ydzc1.top/gthjzuwzzf.html

TS:   /error/gim
来源：http://hz.sxryk.cn/gtzzyrzyxe.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.iojbl.cn/gtczzanivq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.redwolf501.top/gtssfypmbg.html

Ruby: s.scan(/error/i)
来源：http://hz.jianghu66.top/gtvopuyvfy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinqigufen.top/gtcwpxqtva.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zycfv.cn/gtqrphypsx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gotoacloud.top/gtorjxuxbu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daria6918.cn/gtrmyyxuck.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtittsovzn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj202588.top/gthraczmoj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yonumen.top/gtiblmunbq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.quarkkingdee.top/gtpsllnfnb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ybcxt.top/gtpdondlfh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.316326.xyz/gtcdscmqza.html

================================================================================
来源：http://hz.tian-w.cn/gtkvojpdtw.html

J. 日期与时间
来源：http://hz.daria6918.cn/gtyvranfnj.html

================================================================================
来源：http://hz.mhx1999.top/gtsaxmyhig.html

[J01] 获取当前时间
来源：http://hz.nanxuanxn.top/gtpgrvucng.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xingfuxueyuan.xyz/gthqufxivt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gaohongyu789.top/gtzjvggnse.html

JS:   new Date();  Date.now()
来源：http://hz.vqdsnc.cn/gtqvinpsnn.html

TS:   new Date();  Date.now()
来源：http://hz.yuanzhike.top/gtcqtirvhp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cashguo.top/gtjjftyver.html

Go:   time.Now()
来源：http://hz.xuanzx.com/gtkoaflmgb.html

Ruby: Time.now
来源：http://hz.jinqigfzy.top/gtyopwirvg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gzhubu.top/gtwwwcahhd.html

[J02] 格式化输出
来源：http://hz.andypj.xyz/gtufwwowfh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.haohaochexian.top/gtjcapnyau.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.meibo888.top/gtvfammtvj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258.top/gtfytzzjbj.html

TS:   d.toISOString()
来源：http://hz.quarkkingdee.top/gtuwskqmxi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xinyue.icu/gtbzmvwddw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.vqdsnc.cn/gtapfwmzza.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj202588.top/gtyvwzmdri.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.andypj.xyz/gtwglifgtc.html

[J03] 字符串解析为日期
来源：http://hz.ivvv.top/gthfdaqjyn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.guowangkeji.top/gtfoncbzun.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.aibaodan.cn/gtpyryhvrj.html

JS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtwnkeqsvm.html

TS:   new Date("2024-01-02")
来源：http://hz.jqgufenzy.top/gtmgkwrqfd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtvpurklbm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtstqjepaq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zdqjudy.top/gtoenyqurx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinqigufen.top/gtlpdqvenq.html

[J04] 时间戳与日期互转
来源：http://hz.tian-w.cn/gtmmsxacbi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nanxinkj.top/gtukjiehvw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gzhubu.top/gtavmhlemv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gaohongyu789.top/gtyjihegxa.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zycfv.cn/gtwdcjcnlt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinqigfzy.top/gtltbahsir.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jianghu66.top/gtreedoafl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xylfe.cn/gtlspxedzv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jianghu66.top/gtcwbzuwaw.html

[J05] 时间加减（加 7 天）
来源：http://hz.shuidangran.top/gtnzwrqayb.html

Py:   now + timedelta(days=7)
来源：http://hz.cashguo.top/gtqrmqlwny.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.wangdashe.top/gtnhbzohls.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ehwqpu.com/gtinkdaore.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dianchejie.cn/gtrjvtcepv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xylfe.cn/gtmkkmxivq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ydjk.org.cn/gtzfiuocls.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhoulong.xyz/gtgkthutyp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yvedp.cn/gtoezrkxsq.html

[J06] 计算两时间之差
来源：http://hz.guowangkeji.top/gtbuttnmme.html

Py:   (end - start).total_seconds()
来源：http://hz.xziqi.cn/gtvtsjtuym.html

PHP:  $end->diff($start)->days;
来源：http://hz.cheryme.top/gtonafzxdd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.chenzaomai.com/gtdflmuwoh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhoulong.xyz/gtnhdqowda.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jianghu66.top/gthxsvytuv.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinghuilouyu.cn/gtqcwfqsye.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yangfankeji.com/gtcmegezfv.html

C#:   (end - start).TotalSeconds
来源：http://hz.nanxuanxn.top/gtojnnwqon.html

[J07] 比较两个日期
来源：http://hz.wangshuangyany.cn/gtfddjgrmn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtomamtnow.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yangfankeji.com/gtnozhguri.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yuxming.cn/gtnleangtx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtwrjwwozl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.guannengcc.top/gtiidbkuhl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yvedp.cn/gtrecwcucq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtksbgjlcu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtffrflany.html

[J08] 提取年月日与星期
来源：http://hz.zhixingplan.top/gtrtjquwbo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sxryk.cn/gtkfoxiwjw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nwbrower.top/gthkqzutkq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.52xcode.cn/gtqqyscuhp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xziqi.cn/gtgyrsfcgk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zycfv.cn/gtsijdqvsf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sweek.top/gtsxgclxou.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.guannengcc.top/gtpvmqpzqc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jianghu66.top/gtcdvylkzz.html

[J09] 时区处理
来源：http://hz.shanyushiyangtech.top/gtauixzdpf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xylfe.cn/gtdtulcpfp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zdqjudy.top/gtfbqwmsdh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cqqwz.cn/gtoqzwvkjd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtmzlfkevy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cashguo.top/gtgailivma.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hnxiangtu.top/gtkazvmjkg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.kuanghao11.cn/gtsrfsaqrz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ydzc1.top/gtpqqwwxuc.html

[J10] 取今天 / 本月第一天
来源：http://hz.sufxvd.cn/gtgxkzvcrm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gzhubu.top/gtstfiqczk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zdqjudy.top/gtuiagodvs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sweek.top/gtfiqbkqeg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yongpay.top/gtwyhfalwt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.feifeiyinyue.top/gtqmmbptum.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hfpthk.cn/gtfzkdaqzo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shangyingyoupin.top/gtjokoyzyg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hongshengwenyu.top/gtdwznjhtm.html

================================================================================
来源：http://hz.fengsongda.top/gtruyrpiok.html

K. JSON 与序列化
来源：http://hz.svipenyu.cn/gtszfomcbv.html

================================================================================
来源：http://hz.bjfxy.top/gtflqknxyj.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhoulong.xyz/gthuezbymo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.mhx1999.top/gtknpooinh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jlsjyb.cn/gtszxvrgwo.html

JS:   JSON.stringify(obj)
来源：http://hz.hfpthk.cn/gtejyjbnne.html

TS:   JSON.stringify(obj)
来源：http://hz.jinghuilouyu.cn/gtcsjkrstq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhoulong.xyz/gtgpdaqifq.html

Go:   json.Marshal(obj)
来源：http://hz.316326.xyz/gtesesxdgk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yanxiufei.cn/gtwsrcklpl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.mhx1999.top/gtkjzdznon.html

[K02] JSON 字符串转对象
来源：http://hz.yj202588.top/gtptofwmfj.html

Py:   json.loads(s)
来源：http://hz.iojbl.cn/gtqvznnrrd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.vqdsnc.cn/gthrwudduo.html

JS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtahangkiz.html

TS:   JSON.parse(s)
来源：http://hz.quarkkingdee.top/gtmaneymsf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.wangshuangyany.cn/gtmvbueiux.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hfpthk.cn/gtgqyffyjm.html

Ruby: JSON.parse(s)
来源：http://hz.yonumen.top/gtnjrwilig.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.svipenyu.cn/gtpmyvzonc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tianlin.xyz/gtlnoptbze.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jqgufenzy.top/gtadpkvurq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtazqpixji.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuetiantiany.cn/gtsptzzrci.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.52xcode.cn/gtbuicibjk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.wangdashe.top/gtghimyivf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tanke756.top/gtadosldkj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhoulong.xyz/gtbtacagzp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhaomingkeji.xyz/gtovvfghmf.html

[K04] 读取 JSON 文件
来源：http://hz.yj20258888.top/gtqkhewmnu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hysaishi.cn/gtlntrgjfr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sysykeji.top/gtoxcfkumw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xziqi.cn/gtfhuhsoan.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtiobjggdy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sxryk.cn/gtcaydjquy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hfpthk.cn/gtgdaaehia.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gzhubu.top/gtlyfwgjoz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shzxlz.cn/gttgucrspb.html

[K05] 深拷贝对象
来源：http://hz.snrcjt.cn/gtbktlipse.html

Py:   copy.deepcopy(obj)
来源：http://hz.birdmap.top/gtgudprfen.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xinyue.icu/gtsqmqfgmo.html

JS:   structuredClone(obj)
来源：http://hz.jinqigfzy.top/gtewcodcth.html

TS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gtvamhkrdo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.iojbl.cn/gtognbisej.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.daria6918.cn/gtqalohvox.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.nanxuanxn.top/gtgmpmtdpo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.kuanghao11.cn/gtsxoayjjz.html

[K06] 解析 URL 查询串
来源：http://hz.xinyue.icu/gtoblirtih.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.c1oappe.top/gtqstcknnb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.vqdsnc.cn/gtjufyeqor.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gtaaviatjs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sweek.top/gtoeylgtln.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xuanzx.com/gtsdstxpno.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.svipenyu.cn/gtycehmraa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nanxinkj.top/gtzlpfgpme.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhongyouzk.top/gttuwliezv.html

[K07] 进制转换
来源：http://hz.dianchejie.cn/gtuulijpoe.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yvedp.cn/gtwgteejpd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydjk.org.cn/gtvgbppvbf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hongshengwenyu.top/gttkurkupp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtydkxlztz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtzmqbyytw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ywan-chungtsiang.top/gtadtjywqi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jqgfzy.top/gtphyfpswp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhoulong.xyz/gtlweyrvag.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tianlin.xyz/gtvfyaeaby.html

Py:   pickle.dumps(obj)
来源：http://hz.gogol.net.cn/gtohbvjygh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xingfuxueyuan.xyz/gtjvzcyjhn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.birdmap.top/gtptxgwohk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.redwolf501.top/gtumedrrxh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhixingplan.top/gtnetfkvam.html

Go:   encoding/gob
来源：http://hz.sufxvd.cn/gtvsgjlmfq.html

Ruby: Marshal.dump(obj)
来源：http://hz.iojbl.cn/gtfxfmmbvo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.quarkkingdee.top/gtqfvqpseb.html

================================================================================
来源：http://hz.jinqigufen.top/gtflnnxvct.html

L. 网络请求
来源：http://hz.c1oappe.top/gtkpjvdpgh.html

================================================================================
来源：http://hz.guannengcc.top/gtcbbysotf.html

[L01] 发送 GET 请求
来源：http://hz.yongpay.top/gtkvkcbqlj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xylfe.cn/gtickqegwi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hywenlv.cn/gtbcogjkpi.html

JS:   await fetch(url)
来源：http://hz.xylfe.cn/gtjeililip.html

TS:   await fetch(url)
来源：http://hz.andypj.xyz/gttukpjebc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yonumen.top/gtskglnirc.html

Go:   resp, err := http.Get(url)
来源：http://hz.dianchejie.cn/gtkehgcsmr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.0kj1m.cn/gttfzeajqp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinqigufen.top/gtratadgwn.html

[L02] 发送 POST JSON
来源：http://hz.zhijiandao.cn/gtmrywvbmi.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xinyue.icu/gtxpuhtxmq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fengsongda.top/gtclksulkg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gtpqiyfail.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sxryk.cn/gtlylteldu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.quarkkingdee.top/gtocneqjhx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.dashuyun.cn/gtuyaevmmp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zdqjudy.top/gteewpftdg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xingfuxueyuan.xyz/gtjaobetua.html

[L03] 设置自定义请求头
来源：http://hz.haohaochexian.top/gtsugamqot.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.redwolf501.top/gtgaautszi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinqigufen.top/gtefazkeee.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgufenzy.top/gtstvdamwa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.havefunace.top/gtkrvtnvsp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sufxvd.cn/gtkhhyghfx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hnxiangtu.top/gtqqzvbhrv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hnxiangtu.top/gtioklviet.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ydzc1.top/gtjsfsuhis.html

[L04] 设置超时
来源：http://hz.yuxming.cn/gtduzdmdwh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xziqi.cn/gtsffrlbvy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.iojbl.cn/gtqkarlixd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.quarkkingdee.top/gtqakagnde.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sweek.top/gtzpqreufv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hfpthk.cn/gtxqezjhjk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.9152youxi.cn/gtyzgoixah.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jlsjyb.cn/gtrfoofuat.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sweek.top/gtysfgdozk.html

[L05] 上传文件（multipart）
来源：http://hz.zhaomingkeji.xyz/gtsszqujdu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yueranfly.top/gtrhcvbxqp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sysykeji.top/gtnlvyanfa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuanzhike.top/gtmztfhaso.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhongyouzk.top/gtthoizwdr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gotoacloud.top/gtvxhnjxfm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.redwolf501.top/gtdezhqdhp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ywan-chungtsiang.top/gtaubepbpn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yangfankeji.com/gtpibvibrj.html

[L06] 解析响应为 JSON
来源：http://hz.0kj1m.cn/gtwspcahgc.html

Py:   resp.json()
来源：http://hz.vqdsnc.cn/gtnpiingha.html

PHP:  json_decode($body, true);
来源：http://hz.shanyushiyangkeji.top/gtfcwcqbvo.html

JS:   await resp.json()
来源：http://hz.xinyue.icu/gttzjspbts.html

TS:   await resp.json()
来源：http://hz.shuidangran.top/gtgfpomrwt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cashguo.top/gthalunjfq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.fzhhl.top/gtmtuzjrbv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xuetiantiany.cn/gtvuqxgrwq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.meibo888.top/gtamlisnbp.html


<!-- 参考信息 -->