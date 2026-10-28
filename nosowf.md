代发 wailian999

================================================================================
来源：http://hz.wangdashe.top/gtyexnxckb.html

I. 正则表达式
来源：http://hz.guowangkeji.top/gtpklbyvzh.html

================================================================================
来源：http://hz.bjfxy.top/gtcjjaukio.html

[I01] 判断是否匹配
来源：http://hz.yj20258888.top/gtiwzjzpyz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.52xcode.cn/gtwtvncolm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cdnleiting.top/gtbreyusoq.html

JS:   /\d+/.test(s)
来源：http://hz.shangyingyoupin.top/gtopsbutan.html

TS:   /\d+/.test(s)
来源：http://hz.bjfxy.top/gtgityscxw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnxiangtu.top/gtzdfoizrf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.quarkkingdee.top/gtjovgrvwz.html

Ruby: s.match?(/\d+/)
来源：http://hz.shanyushiyangkeji.top/gtmizefxkf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ppjwa.cn/gtkunkzbwx.html

[I02] 提取所有匹配
来源：http://hz.yj20258.top/gtonbckobw.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sxryk.cn/gtqnzfndqa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ydzc1.top/gtymuhuenx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.wangshuangyany.cn/gtjknpveab.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigfzy.top/gtsmondwdv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhaomingkeji.xyz/gtqgfcwtxz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yangfankeji.com/gtznafmqyu.html

Ruby: s.scan(/\d+/)
来源：http://hz.sxryk.cn/gtqbxzvfcr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shanyushiyangkeji.top/gtwjdmtklm.html

[I03] 提取捕获分组
来源：http://hz.guowangkeji.top/gtzpqdycum.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cucudq.cn/gtijnbfazo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yj202588.top/gtpbxcydbc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.mhx1999.top/gtftkamdei.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhoulong.xyz/gtqwayegyz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jlsjyb.cn/gtbxujmkvg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hfpthk.cn/gtelcyfmjf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.wangdashe.top/gtyowdnrxl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ydzc1.top/gtqnbpnzux.html

[I04] 正则替换
来源：http://hz.bjfxy.top/gtmjyptiwx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xziqi.cn/gtcnwwoksh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnxiangtu.top/gtvvpopthe.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yuxming.cn/gtjtbfrrio.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zycfv.cn/gtioiekndu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.9152youxi.cn/gthynwummg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hammf.cn/gtkjjpyinm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.haohaochexian.top/gtrowgjujc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhongyouzk.top/gtxjbghsme.html

[I05] 按正则拆分
来源：http://hz.yuxming.cn/gtwsdjeerj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aibaodan.cn/gtlhmcogtb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.aibaodan.cn/gtcjorpfhe.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtewdmzoqs.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gtjtxduxgj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ivvv.top/gtcvsfqjky.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.dashuyun.cn/gtylyudwno.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtgmjbrncu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhaomingkeji.xyz/gtnomlytmw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.pengpengdd.cyou/gtyqeyxkoo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sxryk.cn/gtuhmlhnus.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jiagoushi.top/gtqirellqh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.andypj.xyz/gtbzpynavc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.0kj1m.cn/gtdlyypnbc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gthtjffmue.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jqgufenzy.top/gtfggxmanc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinqigufen.top/gtbpjrbsuv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.chenlongwang.top/gtrasxjuci.html

[I07] 忽略大小写与多行模式
来源：http://hz.xinyue.icu/gtmdovavme.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.chenzaomai.com/gtgrktpqvo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenlongwang.top/gtferdylnv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhengqikj.top/gtakjsvltr.html

TS:   /error/gim
来源：http://hz.aizwys.cn/gtzwzrzyfd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.9152youxi.cn/gtinblychk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xingfuxueyuan.xyz/gtmoyoaifg.html

Ruby: s.scan(/error/i)
来源：http://hz.bjfxy.top/gtywekvruh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xuanzx.com/gtjehmqiwf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gaohongyu789.top/gtjhxysemn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj202588.top/gtdouufvnb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nwbrower.top/gtxvgqdpyt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangdashe.top/gttvrhqbse.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sxryk.cn/gtnivddyox.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xuetiantiany.cn/gtkawathsp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenjidiqi.icu/gtafgaqrcn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ppjwa.cn/gtsnbdbvyc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtfhwihmmi.html

================================================================================
来源：http://hz.jqgfzy.top/gtrsbvtyvn.html

J. 日期与时间
来源：http://hz.wangshuangyany.cn/gtqektgvjk.html

================================================================================
来源：http://hz.xinyue.icu/gthduepzsb.html

[J01] 获取当前时间
来源：http://hz.gaohongyu789.top/gtftqaciqx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ydjk.org.cn/gtwusdbfkd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gotoacloud.top/gtjonmigku.html

JS:   new Date();  Date.now()
来源：http://hz.nwbrower.top/gttermbtqh.html

TS:   new Date();  Date.now()
来源：http://hz.bjfxy.top/gtmvhzczsr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.iojbl.cn/gtulhutofk.html

Go:   time.Now()
来源：http://hz.xingfuxueyuan.xyz/gtrciojtsi.html

Ruby: Time.now
来源：http://hz.snrcjt.cn/gtiencxube.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.c1oappe.top/gtsdycjjdc.html

[J02] 格式化输出
来源：http://hz.hfpthk.cn/gtqwphvvpt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnqzz.top/gtuoaxddba.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jlsjyb.cn/gtldoiglvx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gogol.net.cn/gtkfazhkuk.html

TS:   d.toISOString()
来源：http://hz.nanxuanxn.top/gtheouezfz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.wangshuangyany.cn/gtxqjdpbct.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.chenlongwang.top/gthzpxzkbt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gtybvehfam.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhijiandao.cn/gtqleikldy.html

[J03] 字符串解析为日期
来源：http://hz.jlsjyb.cn/gtkefiumgb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hywenlv.cn/gtwoopuqpi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.redwolf501.top/gtllwziogn.html

JS:   new Date("2024-01-02")
来源：http://hz.jiagoushi.top/gtkkkmfeas.html

TS:   new Date("2024-01-02")
来源：http://hz.sysykeji.top/gtfogwbkbb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.aizwys.cn/gtdjcrbhul.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zycfv.cn/gtcivrivba.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.52xcode.cn/gtygvppjnl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj20258888.top/gtplnvnwsf.html

[J04] 时间戳与日期互转
来源：http://hz.ppjwa.cn/gtjufkscxf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.316326.xyz/gtairtivrh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sxryk.cn/gtcatsixrc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.svipenyu.cn/gtughhjqoc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ydjk.org.cn/gtbckawihg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ydzc1.top/gtwysfbtks.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ydjk.org.cn/gttsmykcmh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.vqdsnc.cn/gtfpshgjgd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258888.top/gticeuormx.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhixingplan.top/gtqqzvcgpm.html

Py:   now + timedelta(days=7)
来源：http://hz.yuanzhike.top/gtanzdjiha.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgfzy.top/gtolqiqova.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gtjnldmfzz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xziqi.cn/gtzwvqmwup.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shuidangran.top/gtmdxgfxjh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gzhubu.top/gtbrofjtga.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jqgufenzy.top/gtitqkapbv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinyuanbaomall.cn/gtevnoevov.html

[J06] 计算两时间之差
来源：http://hz.nanxuanxn.top/gtwhqnjlde.html

Py:   (end - start).total_seconds()
来源：http://hz.cheryme.top/gtcwxfjqzl.html

PHP:  $end->diff($start)->days;
来源：http://hz.dianchejie.cn/gtmmwtbvfu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.havefunace.top/gttexslatk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yuanzhike.top/gtkmdhpzff.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.0kj1m.cn/gthmufljnr.html

Go:   end.Sub(start).Hours()
来源：http://hz.yanxiufei.cn/gttrcapsft.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenjidiqi.icu/gtctvaqrsb.html

C#:   (end - start).TotalSeconds
来源：http://hz.pycfn.com/gtjjnnelda.html

[J07] 比较两个日期
来源：http://hz.hnxiangtu.top/gtivwtmxek.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtemwyxsrm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jiagoushi.top/gtemuoogqa.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.snrcjt.cn/gtqplqaqfd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtyerrmmik.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.snrcjt.cn/gtafqvqicx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj202588.top/gtrgwycmqb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtlfniqvhh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gtzxqmhddb.html

[J08] 提取年月日与星期
来源：http://hz.jinyuanbaomall.cn/gtzibsgqht.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinyuanbaomall.cn/gtczahxzjx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhijiandao.cn/gtuhnbymmy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nanxinkj.top/gtrhwdhpet.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gotoacloud.top/gtwsvuekja.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jlsjyb.cn/gtnrvdrbxo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhoulong.xyz/gtgermgzfg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sxryk.cn/gtvuwyewwn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.smart0.xyz/gtqxydvysa.html

[J09] 时区处理
来源：http://hz.haohaochexian.top/gtrujoqioq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hnqzz.top/gtgxqztjfp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jyoumei.cn/gtmgedowzr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgfzy.top/gtoxfogqgz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gttrmljclp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.dianchejie.cn/gtaswvbqnz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.quarkkingdee.top/gtxfyqsfou.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhoulong.xyz/gtnvkxjfgh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhixingplan.top/gtsndpapsx.html

[J10] 取今天 / 本月第一天
来源：http://hz.yonumen.top/gtdbbiwdxy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinyuanbaomall.cn/gtppypupgs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gogol.net.cn/gtaflmutkb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.pengpengdd.cyou/gtrshmsrqh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nanxinkj.top/gtiobirtet.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jyoumei.cn/gtpdqficxl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nanxuanxn.top/gtijgdyzcg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cucudq.cn/gtvjgcyxdg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gogol.net.cn/gtpcanuncf.html

================================================================================
来源：http://hz.hnqzz.top/gtxqlrjuhw.html

K. JSON 与序列化
来源：http://hz.jqgfzy.top/gtwfadvlay.html

================================================================================
来源：http://hz.birdmap.top/gtruvtewdk.html

[K01] 对象转 JSON 字符串
来源：http://hz.dianchejie.cn/gtxuzdwmrf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtpepyfupx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yuanzhike.top/gtecbbhtng.html

JS:   JSON.stringify(obj)
来源：http://hz.shzxlz.cn/gtsxcmhknx.html

TS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtrvlwjypc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.pycfn.com/gtdialvazf.html

Go:   json.Marshal(obj)
来源：http://hz.yonumen.top/gtrrybbogn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hongshengwenyu.top/gtkwxokqor.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.aizwys.cn/gtxrzcxnzu.html

[K02] JSON 字符串转对象
来源：http://hz.daxiang520.top/gtjnyqiomd.html

Py:   json.loads(s)
来源：http://hz.birdmap.top/gtrquzvkxz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenjidiqi.icu/gttdmjmjeq.html

JS:   JSON.parse(s)
来源：http://hz.zdqjudy.top/gttmlewoay.html

TS:   JSON.parse(s)
来源：http://hz.ehwqpu.com/gtzrrkpvgt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yongpay.top/gtinjnmstj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtwjsefbja.html

Ruby: JSON.parse(s)
来源：http://hz.wangdashe.top/gttqttxomj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.c1oappe.top/gtzhvcoklr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yvedp.cn/gtyefecopq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cashguo.top/gtmoupcjlr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yueranfly.top/gtqcumyksv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sxryk.cn/gtxaapzuow.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sysykeji.top/gtkhhadsjz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gzhubu.top/gteozmeshi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhijiandao.cn/gtpgrbjvaz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.guannengcc.top/gtxmztkwyf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.haohaochexian.top/gtefegdmdb.html

[K04] 读取 JSON 文件
来源：http://hz.316326.xyz/gtfcluxkmj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.vqdsnc.cn/gtgvfvruuu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hywenlv.cn/gtbgqfjtwl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sufxvd.cn/gtsaaywxsn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.andypj.xyz/gtyjpviwhz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangdashe.top/gtbamhhfcp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtmkxllavv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.316326.xyz/gtegmtqglv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sxryk.cn/gtfoeatxvn.html

[K05] 深拷贝对象
来源：http://hz.andypj.xyz/gtaqwfsgub.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydzc1.top/gtcfriefjf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yueranfly.top/gtazilness.html

JS:   structuredClone(obj)
来源：http://hz.yangfankeji.com/gticbaaplm.html

TS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gtngwptvoe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shanyushiyangtech.top/gtuckifygo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yuanzhike.top/gtykehupza.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jqgfzy.top/gtjzpjnmkn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cheryme.top/gtcckpotap.html

[K06] 解析 URL 查询串
来源：http://hz.9152youxi.cn/gtagfjuqrp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sweek.top/gtbzkaabts.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yuxming.cn/gtjwouzoef.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yonumen.top/gtvqlvlyeu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nwbrower.top/gtrjjzkquf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.wangshuangyany.cn/gtcwwwnaad.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtgtxkfape.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.andypj.xyz/gtlmmahbya.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.quarkkingdee.top/gtpjhtohss.html

[K07] 进制转换
来源：http://hz.zhijiandao.cn/gtzczmvxzz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hfpthk.cn/gthcicfgqx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xuanzx.com/gtlvrkaexu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtskcplvja.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cheryme.top/gtxywutpvn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtukghkbmz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cqqwz.cn/gtnguqfkym.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shuidangran.top/gtarrdkpjq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jyoumei.cn/gtvvdhkjyi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgufenzy.top/gthxtupydx.html

Py:   pickle.dumps(obj)
来源：http://hz.jqgfzy.top/gtyzjblcxh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.quarkkingdee.top/gtkqxpxgmw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.svipenyu.cn/gtttqwlcvy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.aizwys.cn/gtduqnyghg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.c1oappe.top/gtzuuhpknx.html

Go:   encoding/gob
来源：http://hz.gaohongyu789.top/gtmlmamluf.html

Ruby: Marshal.dump(obj)
来源：http://hz.cdnleiting.top/gtnfaalmho.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinqigufen.top/gtafkxgakh.html

================================================================================
来源：http://hz.yj20258888.top/gtisjfitjb.html

L. 网络请求
来源：http://hz.shangyingyoupin.top/gtqtlucntd.html

================================================================================
来源：http://hz.jlsjyb.cn/gtggevwxmn.html

[L01] 发送 GET 请求
来源：http://hz.yuxming.cn/gtpryvjblm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.andypj.xyz/gtpwwgwprv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ywan-chungtsiang.top/gtvcmxhxah.html

JS:   await fetch(url)
来源：http://hz.shanyushiyangkeji.top/gtrbwfmiza.html

TS:   await fetch(url)
来源：http://hz.cheryme.top/gtgldwmsdw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.c1oappe.top/gtgftamewg.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenlongwang.top/gtdqqgtalv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cashguo.top/gtkhkionth.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yonumen.top/gtismeuoam.html

[L02] 发送 POST JSON
来源：http://hz.shangyingyoupin.top/gtmcubmtlx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj20258.top/gtsdpwvgfb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.vqdsnc.cn/gtryclpdoc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.c1oappe.top/gtyqnbfggg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xingfuxueyuan.xyz/gttujemjay.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhongyouzk.top/gttaeiwnpv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zdqjudy.top/gtnayajvml.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.mhx1999.top/gthebzizge.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhongyouzk.top/gtptdvmcdd.html

[L03] 设置自定义请求头
来源：http://hz.daria6918.cn/gtqszuvssf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xinyue.icu/gtfvwnfaip.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shzxlz.cn/gtagbkcnza.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guowangkeji.top/gtmprgyepo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinyuanbaomall.cn/gtxwofwtlj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.guannengcc.top/gtaikhedbw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.52xcode.cn/gtrljjmpfq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.c1oappe.top/gtoabupcsk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtremoskzh.html

[L04] 设置超时
来源：http://hz.yueranfly.top/gtaqthzwvi.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shanyushiyangtech.top/gthjrrmvih.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jlsjyb.cn/gtbzsnjlwj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cashguo.top/gtbtniplkk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuetiantiany.cn/gtqbflxwjc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hysaishi.cn/gtwqvdupqg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinyuanbaomall.cn/gtgnkcqgkr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yangfankeji.com/gteuuusjmu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.guannengcc.top/gtkrgrsaqw.html

[L05] 上传文件（multipart）
来源：http://hz.wangdashe.top/gtvcvcgxlb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj20258.top/gtlucsseex.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.0kj1m.cn/gttnggyabx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.redwolf501.top/gtsscjgcfr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tianlin.xyz/gtfiukfwon.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cucudq.cn/gtcicbpzcx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yangfankeji.com/gtlfmfonpa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.vqdsnc.cn/gtbtmceulf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.smart0.xyz/gththhfcwv.html

[L06] 解析响应为 JSON
来源：http://hz.jlsjyb.cn/gtljeukysm.html

Py:   resp.json()
来源：http://hz.ivvv.top/gtdadnslzc.html

PHP:  json_decode($body, true);
来源：http://hz.ehwqpu.com/gtxhzrlzql.html

JS:   await resp.json()
来源：http://hz.yanxiufei.cn/gtpqoernxn.html

TS:   await resp.json()
来源：http://hz.shuidangran.top/gtrhxywzjf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jqgfzy.top/gtemxtijyw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hongshengwenyu.top/gtvmjwmjay.html

Ruby: JSON.parse(resp.body)
来源：http://hz.feifeiyinyue.top/gtadvisuxw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cheryme.top/gtczodfvkg.html


<!-- 参考信息 -->