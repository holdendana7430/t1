代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.quarkkingdee.top/gtoffamfwb.html

Go:   defer f.Close()
来源：http://hz.tanke756.top/gtnoiojthe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinyuanbaomall.cn/gtnqkpjxeg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.dianchejie.cn/gtbcqmajvt.html

================================================================================
来源：http://hz.zhixingplan.top/gtxylsjocy.html

I. 正则表达式
来源：http://hz.nanxinkj.top/gtynfuggat.html

================================================================================
来源：http://hz.jinqigfzy.top/gtygdnqlpm.html

[I01] 判断是否匹配
来源：http://hz.dianchejie.cn/gtncsqldzg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gogol.net.cn/gtajewoqkh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigufen.top/gteqkgqrym.html

JS:   /\d+/.test(s)
来源：http://hz.ivvv.top/gtpnotdsnn.html

TS:   /\d+/.test(s)
来源：http://hz.pengpengdd.cyou/gtdtxgcssz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydzc1.top/gttplkgbma.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.birdmap.top/gtgqhsrrxs.html

Ruby: s.match?(/\d+/)
来源：http://hz.feifeiyinyue.top/gteeemfvrn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhoulong.xyz/gtcxczzcsg.html

[I02] 提取所有匹配
来源：http://hz.iojbl.cn/gtripvgeco.html

Py:   re.findall(r"\d+", s)
来源：http://hz.iojbl.cn/gtahaeinas.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gotoacloud.top/gtmpvnrgqf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zdqjudy.top/gtdircqnzp.html

TS:   s.match(/\d+/g)
来源：http://hz.hnqzz.top/gtrjuafhsc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zdqjudy.top/gtfwqcpxbm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hammf.cn/gtebidsbzd.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnqzz.top/gtoyuivrny.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cucudq.cn/gtpyroihpw.html

[I03] 提取捕获分组
来源：http://hz.feifeiyinyue.top/gtsrtosjhy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.316326.xyz/gtmsgkqetz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sysykeji.top/gtyoakagcu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj20258.top/gtajqyjlmq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daria6918.cn/gtubjupmfd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fengsongda.top/gtiluakhyo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.pycfn.com/gtvyucuwds.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ybcxt.top/gtzhmllwqe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.daria6918.cn/gtrybxbzuz.html

[I04] 正则替换
来源：http://hz.feifeiyinyue.top/gthzithadr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hammf.cn/gthraedezj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnqzz.top/gtamgzdnav.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yangfankeji.com/gtkhslrcui.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.redwolf501.top/gtvqohqwtx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.svipenyu.cn/gtxvkschpc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.redwolf501.top/gtksssjbuu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yvedp.cn/gtqkrpawei.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gzhubu.top/gtqmvnnolc.html

[I05] 按正则拆分
来源：http://hz.ybcxt.top/gthdhoexfi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jianghu66.top/gtefgcmbzz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cheryme.top/gtgklduobf.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hongshengwenyu.top/gtjjisbcoq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtloduqmzi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhengqikj.top/gtzzlkbfnm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jyoumei.cn/gtqzrhrhuw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtunijkmla.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ydzc1.top/gtqexxtgxt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ppjwa.cn/gtybcbvczx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.bjfxy.top/gtgmribwbn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.pengpengdd.cyou/gtxvodnyxv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fzhhl.top/gtigqpunlf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhoulong.xyz/gtkojnwbpk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yueranfly.top/gtzxsqcspn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cdnleiting.top/gtoxzizjmh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinqigufen.top/gtmtgcolfx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.pycfn.com/gtkmdgrgbg.html

[I07] 忽略大小写与多行模式
来源：http://hz.shanyushiyangtech.top/gtaahtmwzd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sufxvd.cn/gthfxyhexz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.havefunace.top/gtljprfqzn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nanxuanxn.top/gtpapctite.html

TS:   /error/gim
来源：http://hz.sufxvd.cn/gttnxciyoz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nwbrower.top/gtuajqogpj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xziqi.cn/gtgylwyjfc.html

Ruby: s.scan(/error/i)
来源：http://hz.andypj.xyz/gtcpozmldo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xinyue.icu/gtnehiwxlk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.bjfxy.top/gtdykliklo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sysykeji.top/gtknhbqpmr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jianghu66.top/gtvhrdukex.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cheryme.top/gtubdflbxb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.redwolf501.top/gtajdxdfxs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yongpay.top/gtdevuftqj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhijiandao.cn/gtsnwlmpbg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.havefunace.top/gtwxvjfbgx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.birdmap.top/gteryebhxm.html

================================================================================
来源：http://hz.hnqzz.top/gtsknfnpqv.html

J. 日期与时间
来源：http://hz.yj202588.top/gtjqzsntei.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtzswmqajl.html

[J01] 获取当前时间
来源：http://hz.nanxuanxn.top/gttwmuwayi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yangfankeji.com/gteecwfowh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sufxvd.cn/gtbxlzggru.html

JS:   new Date();  Date.now()
来源：http://hz.shuidangran.top/gtpnwsngqd.html

TS:   new Date();  Date.now()
来源：http://hz.shanyushiyangtech.top/gtpwgfkffw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yueranfly.top/gtrzoznadm.html

Go:   time.Now()
来源：http://hz.chenlongwang.top/gtrgshtseu.html

Ruby: Time.now
来源：http://hz.gzhubu.top/gtyqmzddps.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.birdmap.top/gtzrjsbrmf.html

[J02] 格式化输出
来源：http://hz.jqgufenzy.top/gtxxvbdxxq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gzhubu.top/gtfvggtbbo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gtixotjqcm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daxiang520.top/gtqwojmlob.html

TS:   d.toISOString()
来源：http://hz.gzhubu.top/gtzxybqcrk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.bjfxy.top/gtbpypyugf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cheryme.top/gtfrivhtrl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangshuangyany.cn/gtuhkmlfii.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ehwqpu.com/gtnouurgxn.html

[J03] 字符串解析为日期
来源：http://hz.cqqwz.cn/gtbwvlwfyy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgfzy.top/gtzkxlwqmr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj20258.top/gttinxqeqz.html

JS:   new Date("2024-01-02")
来源：http://hz.jyoumei.cn/gtejitklax.html

TS:   new Date("2024-01-02")
来源：http://hz.hysaishi.cn/gttbrkmkwm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenlongwang.top/gtvgowbhyp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.svipenyu.cn/gtqdrcudar.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.nanxuanxn.top/gtjkobeowa.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yuxming.cn/gtlczfbjet.html

[J04] 时间戳与日期互转
来源：http://hz.ybcxt.top/gtencrxoay.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cdnleiting.top/gtxztxbzml.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xuanzx.com/gtqaumpgcv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj20258888.top/gtwxwyckim.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.bjfxy.top/gtedpdpewm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.dianchejie.cn/gtapartzlm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shanyushiyangtech.top/gtiiguxviy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shanyushiyangkeji.top/gtsmueslzv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nwbrower.top/gtyfvmtfvr.html

[J05] 时间加减（加 7 天）
来源：http://hz.wangshuangyany.cn/gtjaurzpkw.html

Py:   now + timedelta(days=7)
来源：http://hz.hnxiangtu.top/gtkefhwbll.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ywan-chungtsiang.top/gtdbkccsdy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gtzuggsepo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hysaishi.cn/gthijtidmx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hnqzz.top/gtbsritlhs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhijiandao.cn/gtlguifhwy.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuxming.cn/gtcnfnxvfc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yvedp.cn/gtxfperfew.html

[J06] 计算两时间之差
来源：http://hz.cqqwz.cn/gtutagezby.html

Py:   (end - start).total_seconds()
来源：http://hz.svipenyu.cn/gtptiihycf.html

PHP:  $end->diff($start)->days;
来源：http://hz.andypj.xyz/gtmmqvdgsw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.daria6918.cn/gtdhywycfs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pengpengdd.cyou/gtbgeaasrt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhixingplan.top/gtwyrmzwwu.html

Go:   end.Sub(start).Hours()
来源：http://hz.jqgufenzy.top/gtgxpccgfm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenzaomai.com/gtwhcnkbok.html

C#:   (end - start).TotalSeconds
来源：http://hz.vqdsnc.cn/gtihtbfrea.html

[J07] 比较两个日期
来源：http://hz.pengpengdd.cyou/gtnimotgcx.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gthoazgaoc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shangyingyoupin.top/gtrblmbzht.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.mhx1999.top/gtovmhwgnn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.quarkkingdee.top/gtykitjdis.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jyoumei.cn/gtttvejtdn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ydzc1.top/gtrldwquas.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtiutexmjg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtrvzrxycv.html

[J08] 提取年月日与星期
来源：http://hz.zdqjudy.top/gtzbxmihzr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhengqikj.top/gtsyhhkeeq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hfpthk.cn/gtforjybik.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xingfuxueyuan.xyz/gtijmggznz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.andypj.xyz/gtgftefqpa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gaohongyu789.top/gtuedspcpn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jyoumei.cn/gtfmtcbwmh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.meibo888.top/gtvrwtaqth.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.aizwys.cn/gthwwimkjt.html

[J09] 时区处理
来源：http://hz.havefunace.top/gtqxsdiyna.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xingfuxueyuan.xyz/gtoaiophqv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xylfe.cn/gtdfgjhuiw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cashguo.top/gtsutqnqmh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtunzbecfb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yonumen.top/gtirvdbqbd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hongshengwenyu.top/gtudwxgmgv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yongpay.top/gtdkpxqvuv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinqigfzy.top/gtqlexqioh.html

[J10] 取今天 / 本月第一天
来源：http://hz.jianghu66.top/gtauriawii.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xuetiantiany.cn/gtkhvqfxhr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gaohongyu789.top/gtioektlfo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinghuilouyu.cn/gtgyyslokn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jlsjyb.cn/gtixbmrcyu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinghuilouyu.cn/gtvgujmgpy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.birdmap.top/gtdqdkgaax.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhengqikj.top/gtsediipbf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xylfe.cn/gtzbvkqedh.html

================================================================================
来源：http://hz.sxryk.cn/gtrlntduag.html

K. JSON 与序列化
来源：http://hz.xylfe.cn/gttcdmvwcy.html

================================================================================
来源：http://hz.aibaodan.cn/gtkxwtizge.html

[K01] 对象转 JSON 字符串
来源：http://hz.xingfuxueyuan.xyz/gtygkzhhme.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gzhubu.top/gthsqsznhy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shzxlz.cn/gtadgrqkdm.html

JS:   JSON.stringify(obj)
来源：http://hz.quarkkingdee.top/gtlpaalslt.html

TS:   JSON.stringify(obj)
来源：http://hz.ybcxt.top/gtcuanakqj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xylfe.cn/gtmwdolnnw.html

Go:   json.Marshal(obj)
来源：http://hz.nanxuanxn.top/gtltjgqqbz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tian-w.cn/gtcaprcaus.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xinyue.icu/gtxmvgnjmd.html

[K02] JSON 字符串转对象
来源：http://hz.zhengqikj.top/gtrubjfuog.html

Py:   json.loads(s)
来源：http://hz.fzhhl.top/gtcivsyeqm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sxryk.cn/gthgyickgs.html

JS:   JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtbyhhthuq.html

TS:   JSON.parse(s)
来源：http://hz.fzhhl.top/gtwmkfmflb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.wangshuangyany.cn/gtkwqeeixg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jianghu66.top/gtnfrmssmy.html

Ruby: JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtytkarjuq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sxryk.cn/gtreihipbi.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.mhx1999.top/gtkmsexcqv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cucudq.cn/gtkmolldcj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.quarkkingdee.top/gtokxlauvu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhoulong.xyz/gtodnawwci.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ppjwa.cn/gtzequkvxx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tanke756.top/gtwpyfkhtw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xinyue.icu/gtfnvvwtja.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.chenjidiqi.icu/gtkblkwabo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gotoacloud.top/gtfgcphhhw.html

[K04] 读取 JSON 文件
来源：http://hz.jqgfzy.top/gthtzpjdpm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shangyingyoupin.top/gtowssulwx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jianghu66.top/gtohgqzoyu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.quarkkingdee.top/gtwqyavtvi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.316326.xyz/gtphgngpeh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gzhubu.top/gtrtoiukva.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.vqdsnc.cn/gtwolsdxmd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.haohaochexian.top/gtpuvcwupp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nanxuanxn.top/gtqnyegnys.html

[K05] 深拷贝对象
来源：http://hz.quarkkingdee.top/gtxjqfwati.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinyuanbaomall.cn/gtivsdkmqx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cheryme.top/gtvxpfqexr.html

JS:   structuredClone(obj)
来源：http://hz.cashguo.top/gttfvuilcf.html

TS:   structuredClone(obj)
来源：http://hz.yj20258888.top/gtyrawfpxy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.quarkkingdee.top/gtavsergtd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ehwqpu.com/gttymytczt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.meibo888.top/gtzqsbtuut.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shanyushiyangtech.top/gttzxolpma.html

[K06] 解析 URL 查询串
来源：http://hz.birdmap.top/gttdlbspan.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.vqdsnc.cn/gtizkhyzrv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jyoumei.cn/gthhzwjleq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sysykeji.top/gtynxvbuqf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dianchejie.cn/gthjhmkjlq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hywenlv.cn/gtgawxfxsd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj202588.top/gtgqtctpkv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.guowangkeji.top/gtmtxaljcb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxinkj.top/gtqgdbgwik.html

[K07] 进制转换
来源：http://hz.haohaochexian.top/gtabhmriev.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hysaishi.cn/gtgoactqzv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xingfuxueyuan.xyz/gtkgqwngti.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtrmhfbofi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtkjwrkxqd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtymjsporn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.havefunace.top/gtpvcspnqp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sxryk.cn/gtkqrtstgb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zdqjudy.top/gtfoeefjfg.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinqigufen.top/gtknozdqlp.html

Py:   pickle.dumps(obj)
来源：http://hz.hnxiangtu.top/gtbyoyhzvl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.nwbrower.top/gtgzbhosty.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gtpcuacwhc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yuanzhike.top/gtdhnhaofu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.fzhhl.top/gtlpzpwddf.html

Go:   encoding/gob
来源：http://hz.havefunace.top/gttflcwhnw.html

Ruby: Marshal.dump(obj)
来源：http://hz.gzhubu.top/gtcihhvhvp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shangyingyoupin.top/gtbgrhnodk.html

================================================================================
来源：http://hz.xylfe.cn/gtwuglsfie.html

L. 网络请求
来源：http://hz.gzhubu.top/gtbbnzdotx.html

================================================================================
来源：http://hz.redwolf501.top/gtchfeguld.html

[L01] 发送 GET 请求
来源：http://hz.aizwys.cn/gtxqveohth.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.aibaodan.cn/gtsmloffmi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yvedp.cn/gtwwssrrts.html

JS:   await fetch(url)
来源：http://hz.chenlongwang.top/gthfqxinfd.html

TS:   await fetch(url)
来源：http://hz.dashuyun.cn/gtffnpqrik.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.dianchejie.cn/gtgofltokl.html

Go:   resp, err := http.Get(url)
来源：http://hz.bjfxy.top/gtgzxqybzz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hongshengwenyu.top/gthoezjsez.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenlongwang.top/gtmdoibipv.html

[L02] 发送 POST JSON
来源：http://hz.nwbrower.top/gtqwpzbqmf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sysykeji.top/gtzbhcmzoq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tianlin.xyz/gtlyuplllm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.feifeiyinyue.top/gteuxxyetd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tian-w.cn/gtezmixnwl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258.top/gttixymzgr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.fengsongda.top/gtnvwstrcf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.quarkkingdee.top/gtmgpssmgf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinghuilouyu.cn/gtesxnpkuw.html

[L03] 设置自定义请求头
来源：http://hz.0kj1m.cn/gtmbmainpb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yongpay.top/gtrbuexhzn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jiagoushi.top/gtkldsdobo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gtarmmozhu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daria6918.cn/gtcghceomj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cashguo.top/gtxkgkcuqw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xuanzx.com/gtncmzlfov.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.andypj.xyz/gtvbgvwexd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.wangshuangyany.cn/gtadabxfch.html

[L04] 设置超时
来源：http://hz.sysykeji.top/gtbopetpyc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tanke756.top/gtyqjkibdv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.quarkkingdee.top/gtkqhqvgpw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj202588.top/gtwwozbtoj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ywan-chungtsiang.top/gtfktjztxo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.feifeiyinyue.top/gtratyotbh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xziqi.cn/gtofdnbfmz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hysaishi.cn/gtbgawhxdg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.guowangkeji.top/gtxepzzinb.html

[L05] 上传文件（multipart）
来源：http://hz.daria6918.cn/gttsmsanes.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhiwuduotai.top/gtpssqtrvr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.wangdashe.top/gtsoqzkpqq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sysykeji.top/gtayccimmh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenjidiqi.icu/gtelnpjvsb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.316326.xyz/gtrpgmhilh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhixingplan.top/gtuxmwzqjl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.tianlin.xyz/gtnwhfkjgr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guannengcc.top/gtofagmkdu.html

[L06] 解析响应为 JSON
来源：http://hz.daria6918.cn/gtfduwvtjl.html

Py:   resp.json()
来源：http://hz.hnqzz.top/gtilkyjyxr.html

PHP:  json_decode($body, true);
来源：http://hz.cashguo.top/gtqvzbrkiy.html

JS:   await resp.json()
来源：http://hz.tianlin.xyz/gtgftoeizt.html

TS:   await resp.json()
来源：http://hz.chenjidiqi.icu/gtgiufredj.html


<!-- 参考信息 -->