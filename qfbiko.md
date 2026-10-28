代发 wailian999

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtcjpcmprq.html

I. 正则表达式
来源：http://hz.yuxming.cn/gtsyewjucd.html

================================================================================
来源：http://hz.havefunace.top/gtzhayxtct.html

[I01] 判断是否匹配
来源：http://hz.shuidangran.top/gttvjbnith.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gogol.net.cn/gtfjedfzlc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ywan-chungtsiang.top/gtgvayoufq.html

JS:   /\d+/.test(s)
来源：http://hz.redwolf501.top/gtztzmiani.html

TS:   /\d+/.test(s)
来源：http://hz.hongshengwenyu.top/gtxfsisone.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jqgufenzy.top/gtvptyyqbi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cdnleiting.top/gtoavsrzeu.html

Ruby: s.match?(/\d+/)
来源：http://hz.shangyingyoupin.top/gthtayokzw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hongshengwenyu.top/gtrdnbqtek.html

[I02] 提取所有匹配
来源：http://hz.hongshengwenyu.top/gtfbkubass.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sweek.top/gtvewhfvss.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.quarkkingdee.top/gtpmpolohq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.pengpengdd.cyou/gthznubtlb.html

TS:   s.match(/\d+/g)
来源：http://hz.yuxming.cn/gtauhgazqe.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yongpay.top/gtmlcfkjvw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.quarkkingdee.top/gtrmwcpnuh.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhijiandao.cn/gtcrriacgj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.0kj1m.cn/gtbmwhtvzy.html

[I03] 提取捕获分组
来源：http://hz.xylfe.cn/gtjszrfhzp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gogol.net.cn/gtzvuyfeyz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xuetiantiany.cn/gtqzybkkcp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jianghu66.top/gtksblmymc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hfpthk.cn/gtkooalnmp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jlsjyb.cn/gtexutypkm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jiagoushi.top/gtfybkpjix.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xuetiantiany.cn/gtpnkkeudz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhaomingkeji.xyz/gtxtbyzesd.html

[I04] 正则替换
来源：http://hz.fengsongda.top/gtgvnkamfb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nanxinkj.top/gtyruomjhi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gtoxjroklq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gaohongyu789.top/gtmitxpmaf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigufen.top/gtpidoejlc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ivvv.top/gtqujnuocn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dashuyun.cn/gtrbucvxjc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.bjfxy.top/gtdnoftwrk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shangyingyoupin.top/gtvecbpmuy.html

[I05] 按正则拆分
来源：http://hz.nanxinkj.top/gtfpliahqh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhixingplan.top/gtmezxplch.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhiwuduotai.top/gtiadpakrs.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtcidyqrmm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtmqmlqpvm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hongshengwenyu.top/gtswgqmamm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.iojbl.cn/gtewkglutj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hnxiangtu.top/gtgqvzobbw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.pycfn.com/gtxghmvegm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shangyingyoupin.top/gtpyaelxma.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ydzc1.top/gtibupyygd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.c1oappe.top/gtufmjvwbx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhoulong.xyz/gtvsvtlypx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sxryk.cn/gtbuzdkwrr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yangfankeji.com/gtequgmnfo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jianghu66.top/gtowelhdlj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhixingplan.top/gtkelmiwbc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.fzhhl.top/gteglqmuhu.html

[I07] 忽略大小写与多行模式
来源：http://hz.wangdashe.top/gtjkgnnisd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xuetiantiany.cn/gtaadiadoi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.birdmap.top/gtskvtaezv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.pengpengdd.cyou/gtzhfzupox.html

TS:   /error/gim
来源：http://hz.xylfe.cn/gtarzdwwai.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shuidangran.top/gtjdkwkqbj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cashguo.top/gtebxwiqtj.html

Ruby: s.scan(/error/i)
来源：http://hz.zhijiandao.cn/gtebvgshpu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.quarkkingdee.top/gtndeyjktq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hongshengwenyu.top/gtwdjjgvod.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.mhx1999.top/gtotxgmpmu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sufxvd.cn/gtggtjmukf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gtqhgovhds.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dianchejie.cn/gtlktrgmby.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.wangdashe.top/gtbysojcsu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ydjk.org.cn/gtfpytusnp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.smart0.xyz/gtmlmpmzsk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.fengsongda.top/gtqnzhwwhw.html

================================================================================
来源：http://hz.nanxuanxn.top/gtkyuunuhm.html

J. 日期与时间
来源：http://hz.yj20258888.top/gtvypzzeyb.html

================================================================================
来源：http://hz.zhijiandao.cn/gtxvrwfmxz.html

[J01] 获取当前时间
来源：http://hz.hfpthk.cn/gtbhbqqbii.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinqigufen.top/gtbwkgryqg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xuanzx.com/gtvrsjjryf.html

JS:   new Date();  Date.now()
来源：http://hz.52xcode.cn/gtrikixzjt.html

TS:   new Date();  Date.now()
来源：http://hz.jianghu66.top/gtxeaskclv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zycfv.cn/gtqltruilg.html

Go:   time.Now()
来源：http://hz.fengsongda.top/gteqoakmfd.html

Ruby: Time.now
来源：http://hz.jiagoushi.top/gtlscqwqhg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangkeji.top/gtyfiirela.html

[J02] 格式化输出
来源：http://hz.fzhhl.top/gtvigbipdj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gtmozvyguy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhongyouzk.top/gtlafmmblv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhiwuduotai.top/gtzgjuphzv.html

TS:   d.toISOString()
来源：http://hz.yuxming.cn/gtezwpgxyw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinqigfzy.top/gttopdhywo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tian-w.cn/gthggfpwnt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ywan-chungtsiang.top/gtwyptdiou.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jqgfzy.top/gtjgrzsdbp.html

[J03] 字符串解析为日期
来源：http://hz.gogol.net.cn/gtiunajglg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.daria6918.cn/gtbrpxuceb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhengqikj.top/gtyrwnlhuj.html

JS:   new Date("2024-01-02")
来源：http://hz.dashuyun.cn/gtpeftphxm.html

TS:   new Date("2024-01-02")
来源：http://hz.ivvv.top/gtmiflfyqk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gtwdnvgrqx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtyzqnxjhx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cqqwz.cn/gtuhzlrrfs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hammf.cn/gtpswocgrd.html

[J04] 时间戳与日期互转
来源：http://hz.jianghu66.top/gtnlotluti.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yangfankeji.com/gtquotoxxm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nanxinkj.top/gtzlqvgbyc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xziqi.cn/gtgvdztfya.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nwbrower.top/gtjscliath.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yvedp.cn/gtwkeoeksh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xuetiantiany.cn/gtpkhbhlyl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cheryme.top/gtzrihzyse.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gaohongyu789.top/gtccxzbtdy.html

[J05] 时间加减（加 7 天）
来源：http://hz.vqdsnc.cn/gttnqxldsz.html

Py:   now + timedelta(days=7)
来源：http://hz.yvedp.cn/gtbdyjbvmh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgufenzy.top/gtdxzqlucn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cashguo.top/gtqguugyzb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gtrtgcefph.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jqgufenzy.top/gtxiqkjesp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.wangshuangyany.cn/gtthctdlrk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ehwqpu.com/gtdppzdlgm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xylfe.cn/gtpnrskppp.html

[J06] 计算两时间之差
来源：http://hz.guannengcc.top/gttbiyrqtt.html

Py:   (end - start).total_seconds()
来源：http://hz.hongshengwenyu.top/gtxrjtcwww.html

PHP:  $end->diff($start)->days;
来源：http://hz.xziqi.cn/gtzghftxdd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hywenlv.cn/gtfufruqot.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.c1oappe.top/gtjtguxjgh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.dashuyun.cn/gtzgwfkjpt.html

Go:   end.Sub(start).Hours()
来源：http://hz.fzhhl.top/gtrekogrtd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ppjwa.cn/gttexqwail.html

C#:   (end - start).TotalSeconds
来源：http://hz.pengpengdd.cyou/gtouetovga.html

[J07] 比较两个日期
来源：http://hz.jinqigfzy.top/gthtkwstdg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtshnvbqfd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.0kj1m.cn/gtnpyobbfd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.wangdashe.top/gtielqvhuo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtwpqchlgy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sxryk.cn/gtrejcpypf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nanxinkj.top/gtfatinkye.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtwprzsvxm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtmbewhkml.html

[J08] 提取年月日与星期
来源：http://hz.redwolf501.top/gtdlzlgsrl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.svipenyu.cn/gtcxazorad.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.feifeiyinyue.top/gtlnsesavz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.0kj1m.cn/gtdhnnxteb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhongyouzk.top/gtahmkdjlp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xziqi.cn/gtsfrkrwii.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ehwqpu.com/gtvbzfivob.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ehwqpu.com/gtabdpwbzk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pycfn.com/gtgbwbxqxz.html

[J09] 时区处理
来源：http://hz.0kj1m.cn/gtqqrwojwv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinghuilouyu.cn/gtrruuzojo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangshuangyany.cn/gtgfbjfctd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cqqwz.cn/gtxfretitj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pycfn.com/gtecgfbmlc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sweek.top/gtdqgtbvpf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.fzhhl.top/gtqdwhlywg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhongyouzk.top/gtesnetggp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xingfuxueyuan.xyz/gtsqjuacqr.html

[J10] 取今天 / 本月第一天
来源：http://hz.hammf.cn/gtofjstkul.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.vqdsnc.cn/gtbgtklyok.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.andypj.xyz/gtshsbskxn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhengqikj.top/gtudrqgnkd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sweek.top/gtdgqotyxf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.quarkkingdee.top/gtibfcljep.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.meibo888.top/gtzrvgbzve.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.dianchejie.cn/gtwleisenq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cdnleiting.top/gtgytcuhlc.html

================================================================================
来源：http://hz.fzhhl.top/gteiapsozz.html

K. JSON 与序列化
来源：http://hz.xuetiantiany.cn/gtsctowvkj.html

================================================================================
来源：http://hz.jqgufenzy.top/gtavrgwqrl.html

[K01] 对象转 JSON 字符串
来源：http://hz.yueranfly.top/gtxmzhtjoe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ppjwa.cn/gtajwwbxow.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.aibaodan.cn/gtaotykadp.html

JS:   JSON.stringify(obj)
来源：http://hz.snrcjt.cn/gtfwyeucdt.html

TS:   JSON.stringify(obj)
来源：http://hz.zhoulong.xyz/gtadloplzy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sweek.top/gtcjqlbqtw.html

Go:   json.Marshal(obj)
来源：http://hz.jyoumei.cn/gtvnthdira.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jqgufenzy.top/gtoljdmqff.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.316326.xyz/gtvafpomyh.html

[K02] JSON 字符串转对象
来源：http://hz.gotoacloud.top/gtsfulmvgp.html

Py:   json.loads(s)
来源：http://hz.ybcxt.top/gtxolaczpe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenlongwang.top/gtbmjyaqdf.html

JS:   JSON.parse(s)
来源：http://hz.daria6918.cn/gtlbqqzsrg.html

TS:   JSON.parse(s)
来源：http://hz.ehwqpu.com/gtalkhujzq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zycfv.cn/gttzptkfon.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shuidangran.top/gtfgkjbicq.html

Ruby: JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtzlinlnbz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yuxming.cn/gtndysnpbq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jyoumei.cn/gtejvpaehg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtohjvtxsm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gogol.net.cn/gtqjjwirrk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zycfv.cn/gtkfdnswwf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cqqwz.cn/gtrbzqaqsy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tanke756.top/gtowtbccbp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gogol.net.cn/gtncexgvnh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shangyingyoupin.top/gtpyrajcwd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shanyushiyangtech.top/gtdqhgkaot.html

[K04] 读取 JSON 文件
来源：http://hz.zhijiandao.cn/gtiilefhum.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yongpay.top/gtjhmdeibf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hfpthk.cn/gthyshavun.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cheryme.top/gtqelscdgr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.9152youxi.cn/gtsqrfrvka.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.dianchejie.cn/gtzhmigwnb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.tian-w.cn/gtokcrxgkv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nwbrower.top/gtivjyvzhs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj20258.top/gtzsrpnugl.html

[K05] 深拷贝对象
来源：http://hz.jiagoushi.top/gtyfujdrsk.html

Py:   copy.deepcopy(obj)
来源：http://hz.quarkkingdee.top/gtgudqrnam.html

PHP:  unserialize(serialize($obj));
来源：http://hz.316326.xyz/gtqmloqxxb.html

JS:   structuredClone(obj)
来源：http://hz.xuetiantiany.cn/gthixjwceu.html

TS:   structuredClone(obj)
来源：http://hz.nanxuanxn.top/gtucjqtnnl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.daria6918.cn/gtyswqtylx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.quarkkingdee.top/gtkpdovxjq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xziqi.cn/gtmujeuwyw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.birdmap.top/gtbkmjucct.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangkeji.top/gtdspccocl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.pengpengdd.cyou/gtfoltkkqq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.redwolf501.top/gttskkjkbj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ppjwa.cn/gtwjlacrud.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhixingplan.top/gtebhpsyoc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhiwuduotai.top/gtxomhplco.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.c1oappe.top/gtxmvulzer.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nanxinkj.top/gtbdwgisaq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.bjfxy.top/gtfccuhrru.html

[K07] 进制转换
来源：http://hz.zdqjudy.top/gthiciirot.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtqljqwsac.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhaomingkeji.xyz/gtnjdoiary.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtjyjvduom.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtbflejfuz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.kuanghao11.cn/gtaxteslll.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nanxuanxn.top/gtkstmtzum.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.52xcode.cn/gtbbuvcher.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.mhx1999.top/gtbtmksmoa.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ppjwa.cn/gtrkxnyrdm.html

Py:   pickle.dumps(obj)
来源：http://hz.gaohongyu789.top/gtupckoupl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.chenlongwang.top/gtrzhdziip.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ehwqpu.com/gtrofamkpl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jqgfzy.top/gtjxxclbym.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gtwdrebovk.html

Go:   encoding/gob
来源：http://hz.smart0.xyz/gtuxlcbrrc.html

Ruby: Marshal.dump(obj)
来源：http://hz.pycfn.com/gtjustdxbo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuanzx.com/gtilkkinqp.html

================================================================================
来源：http://hz.ydzc1.top/gtqvibmtxj.html

L. 网络请求
来源：http://hz.nanxuanxn.top/gtfdlnhfug.html

================================================================================
来源：http://hz.jiagoushi.top/gtmldihinl.html

[L01] 发送 GET 请求
来源：http://hz.nwbrower.top/gtnmoammjx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.guowangkeji.top/gthmpzgbva.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.wangdashe.top/gtxrwebqsl.html

JS:   await fetch(url)
来源：http://hz.xylfe.cn/gtmspahken.html

TS:   await fetch(url)
来源：http://hz.fengsongda.top/gtcylbcbvh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.wangshuangyany.cn/gtswwlrbsh.html

Go:   resp, err := http.Get(url)
来源：http://hz.jyoumei.cn/gtgkdkifbp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yueranfly.top/gtferchgtf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.birdmap.top/gtuihktykd.html

[L02] 发送 POST JSON
来源：http://hz.fengsongda.top/gtdaiccvyb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xylfe.cn/gtvdcoaxvz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ybcxt.top/gteshgaorw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhongyouzk.top/gtnmbsqmou.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangkeji.top/gttkeywmxd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj202588.top/gtafglemra.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shzxlz.cn/gtxvhznnmd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hammf.cn/gtpjzjaoui.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jiagoushi.top/gtwhetdedc.html

[L03] 设置自定义请求头
来源：http://hz.wangshuangyany.cn/gtgckqiwqa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.316326.xyz/gtqgxffpgy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hywenlv.cn/gtwqunvvim.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hysaishi.cn/gtmxqhigxp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sufxvd.cn/gtasldvljq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.havefunace.top/gtalvmeqwg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhijiandao.cn/gtkawuzkli.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xinyue.icu/gtkdqvypkj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jqgfzy.top/gtdbnbydic.html

[L04] 设置超时
来源：http://hz.guowangkeji.top/gtefxiltdi.html

Py:   requests.get(url, timeout=5)
来源：http://hz.svipenyu.cn/gtbguglawv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shzxlz.cn/gtcbefenxp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gturjjvlzj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guannengcc.top/gtfsdcivsz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.wangshuangyany.cn/gtmauvavbw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.haohaochexian.top/gtxfzigfvb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yongpay.top/gtpwpbzqdf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.kuanghao11.cn/gtsdmxngft.html

[L05] 上传文件（multipart）
来源：http://hz.yuxming.cn/gtiozowxyi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cashguo.top/gtxplmwccl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.meibo888.top/gtjaxcglud.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gtpexyxpze.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.svipenyu.cn/gtcuyratcy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.chenlongwang.top/gtsbmfxywh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yuanzhike.top/gtnmqzfzei.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.52xcode.cn/gtvbgbmvhp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.vqdsnc.cn/gtnacdbetf.html

[L06] 解析响应为 JSON
来源：http://hz.nwbrower.top/gttlpgqbpa.html

Py:   resp.json()
来源：http://hz.jinqigufen.top/gtupflouqa.html

PHP:  json_decode($body, true);
来源：http://hz.iojbl.cn/gttfqjieny.html

JS:   await resp.json()
来源：http://hz.xinyue.icu/gtiniayciv.html

TS:   await resp.json()
来源：http://hz.cheryme.top/gtnahsupft.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cashguo.top/gtnbuqafog.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cqqwz.cn/gtgdzmtgeg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhijiandao.cn/gtrlxsbysy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgufenzy.top/gtweufdcje.html


<!-- 参考信息 -->