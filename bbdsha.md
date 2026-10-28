代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.iojbl.cn/gttqzyirnj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tanke756.top/gtmmptsquv.html

Ruby: s.match?(/\d+/)
来源：http://hz.wangshuangyany.cn/gtuamzsbbz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.kuanghao11.cn/gteldjoydc.html

[I02] 提取所有匹配
来源：http://hz.yj202588.top/gtablsqvwj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guowangkeji.top/gtsmzjxmiu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.aibaodan.cn/gtnflxfkzl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.vqdsnc.cn/gtxhsbjobx.html

TS:   s.match(/\d+/g)
来源：http://hz.birdmap.top/gtdrubebks.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xinyue.icu/gtmqlzrrzx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinqigfzy.top/gtlouczyzb.html

Ruby: s.scan(/\d+/)
来源：http://hz.bjfxy.top/gtyoiabeiy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hnqzz.top/gtdnbuauum.html

[I03] 提取捕获分组
来源：http://hz.yj20258.top/gtjcfuaodd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.snrcjt.cn/gthscpshto.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhengqikj.top/gtkmpaxzzy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.52xcode.cn/gtrjcfpfwp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yangfankeji.com/gtdhzqyzzn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jlsjyb.cn/gtliooszxd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hammf.cn/gtqykrmkil.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cashguo.top/gtjgihqfud.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.meibo888.top/gtgaijbwqz.html

[I04] 正则替换
来源：http://hz.zhaomingkeji.xyz/gtbttfjmxz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.birdmap.top/gtsrzbfhht.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuanzhike.top/gtybjsgqcu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.guowangkeji.top/gthzwoakma.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.vqdsnc.cn/gtsmqehviq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tian-w.cn/gtnobogaoo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jianghu66.top/gtvtcxemxa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hysaishi.cn/gtcfbdybkq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shanyushiyangtech.top/gterzyqmkk.html

[I05] 按正则拆分
来源：http://hz.cdnleiting.top/gtytacfwaf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.andypj.xyz/gtvgozoohe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yonumen.top/gtuhhfbhvb.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gtksuijfdd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtgbvrpynh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jianghu66.top/gtyrxmzgmi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.aizwys.cn/gtwehknmpk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtpbjsojrw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jlsjyb.cn/gtizpbjmdy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cucudq.cn/gtbytshcxy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.fengsongda.top/gtdzmzfrbv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dianchejie.cn/gtjuzuvvyd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtibktmeki.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yangfankeji.com/gtickjaohn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yanxiufei.cn/gtnkduhdmg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yvedp.cn/gtkrirosit.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ybcxt.top/gtfxqkltmp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.aibaodan.cn/gtcjkpktxn.html

[I07] 忽略大小写与多行模式
来源：http://hz.feifeiyinyue.top/gtnwihiqlf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cucudq.cn/gtdsqothab.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.smart0.xyz/gttvmobwuz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.pengpengdd.cyou/gtrtxhchsn.html

TS:   /error/gim
来源：http://hz.chenzaomai.com/gtuawnwrwn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yongpay.top/gtuqeiyxnv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sysykeji.top/gtbuhsrzxu.html

Ruby: s.scan(/error/i)
来源：http://hz.ydzc1.top/gtebhrmlah.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258.top/gtutsimkus.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj202588.top/gtdonewszv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhijiandao.cn/gtujytkvwp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.bjfxy.top/gtzealcuca.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtpudisxqg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.andypj.xyz/gtrgnvewfj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yvedp.cn/gtrzwqqzix.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hfpthk.cn/gtsrlubclq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xuanzx.com/gtlxswkhxn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sweek.top/gtdrdcnsei.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtgjghuhic.html

J. 日期与时间
来源：http://hz.xingfuxueyuan.xyz/gtocqirrlf.html

================================================================================
来源：http://hz.shzxlz.cn/gtjjqmvqji.html

[J01] 获取当前时间
来源：http://hz.snrcjt.cn/gtikthavce.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shuidangran.top/gtssnmpdye.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.guowangkeji.top/gtlxvmlqzj.html

JS:   new Date();  Date.now()
来源：http://hz.aibaodan.cn/gtwuzjhcxv.html

TS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gtpqxriezp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.haohaochexian.top/gtdrxhkjvm.html

Go:   time.Now()
来源：http://hz.chenzaomai.com/gtxgivgoei.html

Ruby: Time.now
来源：http://hz.0kj1m.cn/gttjdkujld.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nwbrower.top/gtjjvmirjc.html

[J02] 格式化输出
来源：http://hz.hongshengwenyu.top/gtspnnwrji.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gtlvxklpme.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gtxrxurdfw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jianghu66.top/gtgkmfwese.html

TS:   d.toISOString()
来源：http://hz.xuetiantiany.cn/gtvlcubezr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.smart0.xyz/gtfvasycqu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sysykeji.top/gtphmzsior.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhoulong.xyz/gtpvwowokl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.meibo888.top/gtwilsattb.html

[J03] 字符串解析为日期
来源：http://hz.pycfn.com/gtkzajayul.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sysykeji.top/gtdmipqgvq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.316326.xyz/gttjmhfasr.html

JS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtiowmhjzi.html

TS:   new Date("2024-01-02")
来源：http://hz.cqqwz.cn/gteacexeqd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.meibo888.top/gtjkobmnvt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shzxlz.cn/gtkmebbtuo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hywenlv.cn/gtyfppmtbj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yueranfly.top/gtfdcypokv.html

[J04] 时间戳与日期互转
来源：http://hz.jqgufenzy.top/gtgmwmlctx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hnxiangtu.top/gtsvlykfax.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.havefunace.top/gtpyeoqigt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj202588.top/gtycfmieqa.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.haohaochexian.top/gtmfkvskzp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ydzc1.top/gtpxgwnjuc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sysykeji.top/gtqkmnfzdx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.wangdashe.top/gtmuihiaib.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ybcxt.top/gtwgtjyliq.html

[J05] 时间加减（加 7 天）
来源：http://hz.iojbl.cn/gtmcyaydxr.html

Py:   now + timedelta(days=7)
来源：http://hz.cdnleiting.top/gthajmwexy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.kuanghao11.cn/gtktxwumst.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daxiang520.top/gtkumduhou.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yvedp.cn/gtzxcpswdh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gogol.net.cn/gteeifcyvp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.fzhhl.top/gtyquyrizd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.feifeiyinyue.top/gtichztsuv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.0kj1m.cn/gtuhhlzkxf.html

[J06] 计算两时间之差
来源：http://hz.redwolf501.top/gthsefwckp.html

Py:   (end - start).total_seconds()
来源：http://hz.shanyushiyangtech.top/gtflkymhgr.html

PHP:  $end->diff($start)->days;
来源：http://hz.gaohongyu789.top/gtyddfhzhx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj20258.top/gtqzkrnywf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cucudq.cn/gtzfpcgpht.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.andypj.xyz/gttslfabva.html

Go:   end.Sub(start).Hours()
来源：http://hz.gotoacloud.top/gtxtecqjcd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hywenlv.cn/gtaxcpobxz.html

C#:   (end - start).TotalSeconds
来源：http://hz.cdnleiting.top/gtgmhtsesh.html

[J07] 比较两个日期
来源：http://hz.tanke756.top/gtvnobusvh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtoiwhrqgz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nwbrower.top/gtnntbysxv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gtkavjvvix.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.fzhhl.top/gttwprjzwg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.haohaochexian.top/gtynlchmvm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.bjfxy.top/gtwzsuwcau.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtmlmerejd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nanxuanxn.top/gtfzqtppte.html

[J08] 提取年月日与星期
来源：http://hz.yuxming.cn/gtaiuopuyy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.havefunace.top/gtpukkslbe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.0kj1m.cn/gtfndjigum.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yuxming.cn/gtfsuhhvme.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hfpthk.cn/gtdapfcurw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yvedp.cn/gtjuyasvey.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ehwqpu.com/gtpvpsrjbf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.svipenyu.cn/gtkncdaewf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pycfn.com/gthpvdjsui.html

[J09] 时区处理
来源：http://hz.jqgufenzy.top/gtiadffcsq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hysaishi.cn/gtnmeublxm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cucudq.cn/gtsgtjkvet.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhijiandao.cn/gtuebirblj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.vqdsnc.cn/gtpfopaeys.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhaomingkeji.xyz/gtsxlrllwm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.316326.xyz/gtwcldaqrh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hnqzz.top/gtfghhpcjn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yanxiufei.cn/gtuntqxalv.html

[J10] 取今天 / 本月第一天
来源：http://hz.yj202588.top/gtqtvvvlzi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shuidangran.top/gterdimiiu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yonumen.top/gtlykdfqaz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cucudq.cn/gtpqxrlkvh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cashguo.top/gtbbvlhlnb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sxryk.cn/gtwwbdbsny.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhoulong.xyz/gtfnmyaaew.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xuanzx.com/gttsrulxki.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jiagoushi.top/gtsfhsvpew.html

================================================================================
来源：http://hz.xuanzx.com/gtjegbirgf.html

K. JSON 与序列化
来源：http://hz.jinqigfzy.top/gtdxdyprfn.html

================================================================================
来源：http://hz.jqgfzy.top/gtdcymyylo.html

[K01] 对象转 JSON 字符串
来源：http://hz.jlsjyb.cn/gtrwhchehw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xingfuxueyuan.xyz/gtzhruhatw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zdqjudy.top/gtnchvgehq.html

JS:   JSON.stringify(obj)
来源：http://hz.jinyuanbaomall.cn/gtzhzjckrt.html

TS:   JSON.stringify(obj)
来源：http://hz.ydjk.org.cn/gtelkdaczl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.havefunace.top/gtidrenjzq.html

Go:   json.Marshal(obj)
来源：http://hz.jianghu66.top/gtvwbrfmcc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jyoumei.cn/gtrrerirrq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shzxlz.cn/gtufxixngk.html

[K02] JSON 字符串转对象
来源：http://hz.jlsjyb.cn/gtbdnblkyx.html

Py:   json.loads(s)
来源：http://hz.dashuyun.cn/gtcfdahbdk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ydjk.org.cn/gtqbrunpzr.html

JS:   JSON.parse(s)
来源：http://hz.mhx1999.top/gtnmxcwcjn.html

TS:   JSON.parse(s)
来源：http://hz.52xcode.cn/gtiqkvsboe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sxryk.cn/gtpbkovguj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yanxiufei.cn/gtuusszjlm.html

Ruby: JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gttcrcdicj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jiagoushi.top/gtzohwtmoz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tianlin.xyz/gtquhzyjrw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xylfe.cn/gtxenivotj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gttavltejk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.kuanghao11.cn/gtxfhxfeqh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.fzhhl.top/gtvziaurah.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hnxiangtu.top/gttoampoem.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nanxuanxn.top/gtsnvjveto.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhoulong.xyz/gtrczsdmqx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jlsjyb.cn/gtzcrodmct.html

[K04] 读取 JSON 文件
来源：http://hz.shuidangran.top/gtxfphmlrx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.snrcjt.cn/gteiempczy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nanxinkj.top/gtqtrtgciq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ehwqpu.com/gtiikurakj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sweek.top/gtxfbmyxfs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.guannengcc.top/gtldlwueoc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xingfuxueyuan.xyz/gtsachuipo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tian-w.cn/gtabhxtvxv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jianghu66.top/gtxhirhqeo.html

[K05] 深拷贝对象
来源：http://hz.cheryme.top/gttsevelyh.html

Py:   copy.deepcopy(obj)
来源：http://hz.cdnleiting.top/gtpibiilio.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xylfe.cn/gthjezltoo.html

JS:   structuredClone(obj)
来源：http://hz.tian-w.cn/gtyrdounwq.html

TS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtajlfpmot.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jyoumei.cn/gtlsvioxxq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ivvv.top/gtllkdrxsk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.guowangkeji.top/gtrwxknbjt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenjidiqi.icu/gtzzqerugs.html

[K06] 解析 URL 查询串
来源：http://hz.yuxming.cn/gtwafiwoyd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.fzhhl.top/gtnzfcfgoj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenzaomai.com/gtbsuajpak.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.vqdsnc.cn/gtxoljwqsx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.haohaochexian.top/gtatddadwf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.kuanghao11.cn/gtuylhplxv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jqgufenzy.top/gtbatlaueb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hammf.cn/gtflzllnvz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtywjknhcl.html

[K07] 进制转换
来源：http://hz.guowangkeji.top/gtgmluogrd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhengqikj.top/gtbbejdquw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nanxuanxn.top/gtbmqggcyu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtzllvihlp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtftzsegxe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nwbrower.top/gtbkratstz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jqgufenzy.top/gtkvrufacv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenlongwang.top/gtcabzlkze.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenjidiqi.icu/gtyitliaei.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sufxvd.cn/gtivlttmmm.html

Py:   pickle.dumps(obj)
来源：http://hz.yueranfly.top/gtkfqssnbh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tian-w.cn/gtoysppcpt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yuxming.cn/gtfhrcpguz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj202588.top/gtttmvvski.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cheryme.top/gtxkuqtmkh.html

Go:   encoding/gob
来源：http://hz.chenlongwang.top/gtgnnwwjnx.html

Ruby: Marshal.dump(obj)
来源：http://hz.guannengcc.top/gtnckuiptl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hammf.cn/gthacniodi.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtjufreuqj.html

L. 网络请求
来源：http://hz.shzxlz.cn/gtjbtnhpzz.html

================================================================================
来源：http://hz.dashuyun.cn/gtxlqndnhh.html

[L01] 发送 GET 请求
来源：http://hz.zhixingplan.top/gtchvseiwo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yanxiufei.cn/gtdrctfcpa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.feifeiyinyue.top/gttweylhij.html

JS:   await fetch(url)
来源：http://hz.52xcode.cn/gtstxsvnue.html

TS:   await fetch(url)
来源：http://hz.hongshengwenyu.top/gtduojerot.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.tianlin.xyz/gtvhhufgia.html

Go:   resp, err := http.Get(url)
来源：http://hz.gaohongyu789.top/gtbmlffdfz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jyoumei.cn/gtehvksple.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.fengsongda.top/gtfveaimzg.html

[L02] 发送 POST JSON
来源：http://hz.316326.xyz/gtfkrmpsof.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgufenzy.top/gtjqxrfxpd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.kuanghao11.cn/gtlijmgyei.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sysykeji.top/gtsqpoifcb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gthodifdug.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.fengsongda.top/gtcdfhulov.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sysykeji.top/gtbdhqmbnl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.iojbl.cn/gtvxdvhcsm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yueranfly.top/gtjiuoxnll.html

[L03] 设置自定义请求头
来源：http://hz.pycfn.com/gtermcdapb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.52xcode.cn/gtscoyzvit.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gotoacloud.top/gtljcxjnvd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ybcxt.top/gtqqofqajp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.kuanghao11.cn/gtbfssrndj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tanke756.top/gtrdekubpx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xylfe.cn/gtzdjnffug.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.havefunace.top/gtcjwvnjla.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.chenjidiqi.icu/gtbtyuacvs.html

[L04] 设置超时
来源：http://hz.wangshuangyany.cn/gttejsgnjq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yuanzhike.top/gtonwvjohs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nwbrower.top/gtizxtgixs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hongshengwenyu.top/gtyeogcsnd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gtmmwzdher.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yuanzhike.top/gtxxfcwwqx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhixingplan.top/gtreltuwln.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hammf.cn/gtekcrqdcg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shangyingyoupin.top/gtkimjoheu.html

[L05] 上传文件（multipart）
来源：http://hz.yanxiufei.cn/gtftguhcig.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.aibaodan.cn/gtqpascicn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jiagoushi.top/gthkzqihmw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.52xcode.cn/gtxjryuwkg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yangfankeji.com/gthqgyyqes.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hywenlv.cn/gtpiimguwz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.9152youxi.cn/gtafmdlhoq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.bjfxy.top/gtwtkgfbqa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hnqzz.top/gtzwvndfis.html

[L06] 解析响应为 JSON
来源：http://hz.hongshengwenyu.top/gtursjantw.html

Py:   resp.json()
来源：http://hz.iojbl.cn/gtukbjwifh.html

PHP:  json_decode($body, true);
来源：http://hz.pengpengdd.cyou/gtqilkpfyy.html

JS:   await resp.json()
来源：http://hz.yj20258.top/gtkaflratg.html

TS:   await resp.json()
来源：http://hz.hammf.cn/gtgyuqdtaz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cqqwz.cn/gtuftldyet.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hfpthk.cn/gtnlmmbgra.html

Ruby: JSON.parse(resp.body)
来源：http://hz.feifeiyinyue.top/gtytszfans.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenlongwang.top/gtjeixvplc.html

[L07] 处理 HTTP 状态码
来源：http://hz.cqqwz.cn/gtzomerntb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.iojbl.cn/gtsrgxgezm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.kuanghao11.cn/gtvgobfvqj.html

JS:   resp.ok;  resp.status
来源：http://hz.fengsongda.top/gtavuasxjn.html

TS:   resp.ok;  resp.status
来源：http://hz.nanxuanxn.top/gtffrzycbo.html

Java: resp.statusCode()
来源：http://hz.shuidangran.top/gtyjpweqqj.html

Go:   resp.StatusCode
来源：http://hz.chenlongwang.top/gtixeijpge.html

Ruby: resp.code.to_i
来源：http://hz.andypj.xyz/gtotffibhl.html


<!-- 参考信息 -->