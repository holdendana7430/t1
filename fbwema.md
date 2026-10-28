代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ivvv.top/gtrermudau.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yvedp.cn/gtowyhdggk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.andypj.xyz/gtvooejvpn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.wangdashe.top/gthgdrkzsw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ydjk.org.cn/gtoyinetzi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhiwuduotai.top/gtemmxikvs.html

[I04] 正则替换
来源：http://hz.nanxinkj.top/gtlnnoocyb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yvedp.cn/gtrucwutvp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258888.top/gtsuhuovom.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cheryme.top/gtkincnflw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhengqikj.top/gtzmuiiqqn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gotoacloud.top/gtevsrmwug.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shzxlz.cn/gtltirmdwj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnqzz.top/gtkyjfnxav.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ppjwa.cn/gtuuxojbxb.html

[I05] 按正则拆分
来源：http://hz.guannengcc.top/gthkyjtlva.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jlsjyb.cn/gttuuzpsyx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.kuanghao11.cn/gtktfcvhca.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gtjwpyaydc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtowivibqk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.daxiang520.top/gtutdphxkc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhengqikj.top/gtgzeugoqi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtayhoxfll.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cqqwz.cn/gtgsmlftex.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tanke756.top/gtvskprzde.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xylfe.cn/gtbnqkkorg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cashguo.top/gtswetgadc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shzxlz.cn/gtgqhqwgrj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.meibo888.top/gteimbbjdl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.fzhhl.top/gtqmwhhhxb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ivvv.top/gtzrufyrsj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.iojbl.cn/gtdbyppwsc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sweek.top/gtpmdpcwfb.html

[I07] 忽略大小写与多行模式
来源：http://hz.xziqi.cn/gtgplxyfun.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sufxvd.cn/gtpzwoerdy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hnqzz.top/gtbpbgyebe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nanxinkj.top/gthrjhdivc.html

TS:   /error/gim
来源：http://hz.jqgufenzy.top/gtouhmsddk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gotoacloud.top/gtkmtoozvy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.aibaodan.cn/gtsfiazidi.html

Ruby: s.scan(/error/i)
来源：http://hz.guannengcc.top/gtlqnkprjh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.svipenyu.cn/gtktwlpeow.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shanyushiyangtech.top/gtpmgumiwg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sysykeji.top/gtfksynjns.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.fzhhl.top/gtbbazxmdn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.quarkkingdee.top/gtjwrghitu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fzhhl.top/gtkuvsmfqi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shanyushiyangkeji.top/gtyrifadnl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.haohaochexian.top/gtddzydudg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shangyingyoupin.top/gtbibvblhf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yonumen.top/gtqcfirkax.html

================================================================================
来源：http://hz.sysykeji.top/gtawithlah.html

J. 日期与时间
来源：http://hz.ppjwa.cn/gtexkngsxd.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtraxqayuf.html

[J01] 获取当前时间
来源：http://hz.ybcxt.top/gtrsggukyj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hammf.cn/gtzozrflkc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hywenlv.cn/gtsngeomho.html

JS:   new Date();  Date.now()
来源：http://hz.316326.xyz/gtyjbrqxaf.html

TS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtwoqbrbco.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj20258.top/gtemibghlg.html

Go:   time.Now()
来源：http://hz.dashuyun.cn/gtzidywcmi.html

Ruby: Time.now
来源：http://hz.9152youxi.cn/gtwgknnpcc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hysaishi.cn/gtayptkxti.html

[J02] 格式化输出
来源：http://hz.ivvv.top/gtvtyoecsp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gaohongyu789.top/gtzwhbaqbv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhaomingkeji.xyz/gtxntxgzam.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.wangdashe.top/gtwqaqdyig.html

TS:   d.toISOString()
来源：http://hz.sufxvd.cn/gtauckxnia.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.fengsongda.top/gtoqbzqcvf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zycfv.cn/gtweabxltb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.9152youxi.cn/gtyprwglhe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhaomingkeji.xyz/gtpwlblmcb.html

[J03] 字符串解析为日期
来源：http://hz.xinyue.icu/gtyjqrvjkx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhaomingkeji.xyz/gtjecrzvez.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenzaomai.com/gtkbazchda.html

JS:   new Date("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtcvddnnqj.html

TS:   new Date("2024-01-02")
来源：http://hz.birdmap.top/gtvnhdxvzn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yongpay.top/gtqkzkabqq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.pengpengdd.cyou/gtsxvpxgcv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ydzc1.top/gtepgyerwo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shzxlz.cn/gtzcgzlrsn.html

[J04] 时间戳与日期互转
来源：http://hz.yongpay.top/gtgvbqhoii.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenlongwang.top/gtddynopxh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hfpthk.cn/gtglasuckh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tanke756.top/gtvnmpqwdc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xziqi.cn/gtegwrlhtc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hnxiangtu.top/gtvlqhcdgu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj202588.top/gtjdbsfuvr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yuxming.cn/gtmczysrkf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yongpay.top/gtgvsdlwmu.html

[J05] 时间加减（加 7 天）
来源：http://hz.sufxvd.cn/gtfrijflff.html

Py:   now + timedelta(days=7)
来源：http://hz.cdnleiting.top/gttwmziyoe.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yanxiufei.cn/gtydjfixio.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj202588.top/gtsazyrouf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuxming.cn/gtokfyphkt.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zycfv.cn/gtsnogqete.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shzxlz.cn/gtzbwwylcw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.quarkkingdee.top/gtzjzchtup.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xziqi.cn/gtbvbsfjze.html

[J06] 计算两时间之差
来源：http://hz.yanxiufei.cn/gtgpwygesi.html

Py:   (end - start).total_seconds()
来源：http://hz.nanxinkj.top/gtsggfkjkj.html

PHP:  $end->diff($start)->days;
来源：http://hz.jqgfzy.top/gtfdamjyti.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sysykeji.top/gttpbgaryf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zycfv.cn/gtburjyekh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenlongwang.top/gtglxgikoh.html

Go:   end.Sub(start).Hours()
来源：http://hz.svipenyu.cn/gtcmxnhhbz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ywan-chungtsiang.top/gtorbdhhcs.html

C#:   (end - start).TotalSeconds
来源：http://hz.sxryk.cn/gtzphpwvfb.html

[J07] 比较两个日期
来源：http://hz.jiagoushi.top/gtysqbquxz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtgjktuawg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj202588.top/gtgoslsrpi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.c1oappe.top/gtfpjdzoic.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtjitnssmm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhiwuduotai.top/gtgefpdwgt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yangfankeji.com/gttdxyrbvh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhijiandao.cn/gtfkrurdvk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gtwnyjdbei.html

[J08] 提取年月日与星期
来源：http://hz.jinqigufen.top/gtsavojnfq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.fengsongda.top/gtzinissmn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cashguo.top/gtckuaitdc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.c1oappe.top/gtmbeueqfk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sufxvd.cn/gtwkgjuppo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinyuanbaomall.cn/gtyjbgwcyv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.kuanghao11.cn/gtqjpizdpz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shzxlz.cn/gtfxhfgkjl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ydjk.org.cn/gtvnuopnjz.html

[J09] 时区处理
来源：http://hz.guowangkeji.top/gtfjpbeqzj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xinyue.icu/gtsdydewkz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhixingplan.top/gtsmpufsku.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtnbkmvvph.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnqzz.top/gtdenergtc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ehwqpu.com/gtetzahfft.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.pengpengdd.cyou/gtfhwgwdpd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hywenlv.cn/gtuvvomcly.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.chenjidiqi.icu/gttedmriag.html

[J10] 取今天 / 本月第一天
来源：http://hz.pengpengdd.cyou/gtkgvlssjd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shuidangran.top/gtlbuieuyq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yanxiufei.cn/gtoogeolqv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ydjk.org.cn/gtxapcwrtj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.iojbl.cn/gtpyvqimcg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shanyushiyangkeji.top/gtnaollrbp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jyoumei.cn/gtjfsnzkjw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.mhx1999.top/gtpuiyrcoz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.quarkkingdee.top/gtwdiuaaev.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtmagjremv.html

K. JSON 与序列化
来源：http://hz.sysykeji.top/gtxksbmbau.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtoitdhaee.html

[K01] 对象转 JSON 字符串
来源：http://hz.wangshuangyany.cn/gtlgostbyp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhiwuduotai.top/gtwzxxjfub.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.iojbl.cn/gtljmxyqhc.html

JS:   JSON.stringify(obj)
来源：http://hz.svipenyu.cn/gtxoubvpgs.html

TS:   JSON.stringify(obj)
来源：http://hz.wangdashe.top/gtijjnohdx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tianlin.xyz/gtjiminiko.html

Go:   json.Marshal(obj)
来源：http://hz.quarkkingdee.top/gtseczehmk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.dashuyun.cn/gtvgogbimm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.c1oappe.top/gtriwcilhh.html

[K02] JSON 字符串转对象
来源：http://hz.yj202588.top/gtwofpbalf.html

Py:   json.loads(s)
来源：http://hz.ybcxt.top/gttkkpormd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zdqjudy.top/gtymswlclp.html

JS:   JSON.parse(s)
来源：http://hz.bjfxy.top/gtivuhhios.html

TS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtxvebzdem.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.c1oappe.top/gtmqgukgut.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jiagoushi.top/gtwwsgyqfg.html

Ruby: JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtvtlohfzv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xuanzx.com/gtjpcrsqjv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.birdmap.top/gtccjiyoto.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xingfuxueyuan.xyz/gtrlnwmols.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.smart0.xyz/gtflpmxmgg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtxrfwnolv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gtdfrxnkmn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shangyingyoupin.top/gtlpyepwxz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.0kj1m.cn/gtcfrfdxme.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jianghu66.top/gthuwrwxgi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.feifeiyinyue.top/gtixulpock.html

[K04] 读取 JSON 文件
来源：http://hz.c1oappe.top/gtkfuvddrb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shanyushiyangkeji.top/gtvtbinpcz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhiwuduotai.top/gtnritwmhv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gogol.net.cn/gtxufxdhcs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangkeji.top/gtcgtncjzr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhengqikj.top/gtsxnabqrj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.mhx1999.top/gtcvdcbpem.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhijiandao.cn/gtywxggtch.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tianlin.xyz/gtabjsoqxz.html

[K05] 深拷贝对象
来源：http://hz.daxiang520.top/gtddnbltxf.html

Py:   copy.deepcopy(obj)
来源：http://hz.fzhhl.top/gtfijizcxj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gotoacloud.top/gtrvefusmv.html

JS:   structuredClone(obj)
来源：http://hz.daxiang520.top/gtlzvgtmco.html

TS:   structuredClone(obj)
来源：http://hz.sweek.top/gtmkwwqvco.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.wangshuangyany.cn/gtltqpjpok.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xuetiantiany.cn/gtegssjihh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fengsongda.top/gtjqzgikgx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.feifeiyinyue.top/gtavfclszb.html

[K06] 解析 URL 查询串
来源：http://hz.cashguo.top/gtapnhfsvy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cashguo.top/gtuqotszxb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinghuilouyu.cn/gtdjanunzl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.havefunace.top/gtqmztxdmg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gaohongyu789.top/gtuyrjqiwo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nwbrower.top/gtxrxnrllm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.nanxinkj.top/gtodiurluu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shanyushiyangtech.top/gtqozspkhp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigufen.top/gtydmmdqio.html

[K07] 进制转换
来源：http://hz.aizwys.cn/gtfnlbqxrw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.redwolf501.top/gtxazopqfh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hammf.cn/gtmtmzfxid.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.daxiang520.top/gtdglqevot.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtmekvurdo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gtphhyqxfw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.aibaodan.cn/gtaaurzsah.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.c1oappe.top/gtrmknubge.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinqigfzy.top/gtjqglvasp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.fzhhl.top/gtylyrlgma.html

Py:   pickle.dumps(obj)
来源：http://hz.xuetiantiany.cn/gtfyfwyeel.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ydjk.org.cn/gtjdjamvvl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhaomingkeji.xyz/gtkqmvhbqd.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhongyouzk.top/gtsqdbmxrd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinghuilouyu.cn/gtbdtjlcqc.html

Go:   encoding/gob
来源：http://hz.zycfv.cn/gtynkrrusg.html

Ruby: Marshal.dump(obj)
来源：http://hz.tanke756.top/gtzyghpxhl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hnxiangtu.top/gtknbzapmr.html

================================================================================
来源：http://hz.yongpay.top/gtxautjuju.html

L. 网络请求
来源：http://hz.quarkkingdee.top/gtfiiacbva.html

================================================================================
来源：http://hz.meibo888.top/gtbwwogiuh.html

[L01] 发送 GET 请求
来源：http://hz.yj202588.top/gtnftwskxg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.bjfxy.top/gtlilkqgps.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yueranfly.top/gtekxyxdjh.html

JS:   await fetch(url)
来源：http://hz.hnxiangtu.top/gtvnvowtia.html

TS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gtsgakgzro.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.9152youxi.cn/gtnkhbooho.html

Go:   resp, err := http.Get(url)
来源：http://hz.zdqjudy.top/gtrbhmgnsw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.kuanghao11.cn/gtaoapmfnb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shangyingyoupin.top/gtmgbgmqtt.html

[L02] 发送 POST JSON
来源：http://hz.chenjidiqi.icu/gtfrudtgyg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhongyouzk.top/gtsrvurqwk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ppjwa.cn/gtlkipzoel.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenjidiqi.icu/gthnckdjbz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ybcxt.top/gtvyhmidwt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258888.top/gtcfidvcrf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.svipenyu.cn/gtirnmiycx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xuetiantiany.cn/gtkhaoeaql.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xuanzx.com/gtnjwsamxe.html

[L03] 设置自定义请求头
来源：http://hz.jinqigufen.top/gtfpgxqjcd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.bjfxy.top/gtblbllgwr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jqgfzy.top/gtdsucjryd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenlongwang.top/gttkfxjtxr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gtmmcaptdv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sysykeji.top/gtbcmselgu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.guannengcc.top/gtacgkwmrb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ehwqpu.com/gtjdmvbpbn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jiagoushi.top/gtwaylfbap.html

[L04] 设置超时
来源：http://hz.tianlin.xyz/gtbimprdbi.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hywenlv.cn/gtiylgictc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.iojbl.cn/gtmthydhue.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dianchejie.cn/gtganxtldu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gtkwxtjtsl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yanxiufei.cn/gtsngtbtzr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.redwolf501.top/gtbepnzqfl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xinyue.icu/gtuubqugwi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hywenlv.cn/gtjamzqluw.html

[L05] 上传文件（multipart）
来源：http://hz.xingfuxueyuan.xyz/gtjluoacov.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhijiandao.cn/gtigmvxhcr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.bjfxy.top/gtyuwnvqwz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sufxvd.cn/gtrrolozra.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgfzy.top/gtgbyfgxja.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hammf.cn/gtfbsddcpl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.aizwys.cn/gtksjalwnq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yongpay.top/gtzwcrdvmj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhaomingkeji.xyz/gtribqyzei.html

[L06] 解析响应为 JSON
来源：http://hz.cdnleiting.top/gtxdlxykwc.html

Py:   resp.json()
来源：http://hz.0kj1m.cn/gtabcmvugr.html

PHP:  json_decode($body, true);
来源：http://hz.sxryk.cn/gtcoszhfth.html

JS:   await resp.json()
来源：http://hz.zhixingplan.top/gtuxzgmfsz.html

TS:   await resp.json()
来源：http://hz.aibaodan.cn/gtqhrdumbr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shangyingyoupin.top/gtfirudvwn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhixingplan.top/gtpfrbdywj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sysykeji.top/gtokljrhte.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xuetiantiany.cn/gtkrxoboma.html

[L07] 处理 HTTP 状态码
来源：http://hz.hywenlv.cn/gtczoredxs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shanyushiyangtech.top/gtchirevjl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ydzc1.top/gtwgejovot.html

JS:   resp.ok;  resp.status
来源：http://hz.ydzc1.top/gthnpifydc.html

TS:   resp.ok;  resp.status
来源：http://hz.pengpengdd.cyou/gtgmovkffh.html

Java: resp.statusCode()
来源：http://hz.tianlin.xyz/gtytnikxbi.html

Go:   resp.StatusCode
来源：http://hz.hywenlv.cn/gtdlkijcwo.html

Ruby: resp.code.to_i
来源：http://hz.zycfv.cn/gtwukxvxwo.html

C#:   (int)resp.StatusCode
来源：http://hz.zhijiandao.cn/gtslwyviyz.html

[L08] 并发请求多个地址
来源：http://hz.yongpay.top/gtdmxwcldo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ydzc1.top/gtluareczi.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhijiandao.cn/gtudlcvqcu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fzhhl.top/gtflgavrev.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenlongwang.top/gthxltubgq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shanyushiyangtech.top/gttvoloqfo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yanxiufei.cn/gtclqckavb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.bjfxy.top/gtaersquhd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.pengpengdd.cyou/gthrfzyzmz.html

================================================================================
来源：http://hz.pycfn.com/gtwdxwbdwq.html

M. 命令行 / 进程 / 环境
来源：http://hz.yangfankeji.com/gteleoebtu.html

================================================================================
来源：http://hz.dianchejie.cn/gtmsceehsw.html

[M01] 读取命令行参数
来源：http://hz.quarkkingdee.top/gtcebscddf.html

Py:   sys.argv[1:]
来源：http://hz.9152youxi.cn/gtlohxosyo.html

PHP:  $argv;  $argc;
来源：http://hz.redwolf501.top/gtmcovpdkr.html


<!-- 参考信息 -->