代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.daxiang520.top/gtdfxfdoeu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhoulong.xyz/gtwurxgefp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.wangshuangyany.cn/gtihgsecpj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gzhubu.top/gtcziqlzaz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hnqzz.top/gttvsoxzec.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuxming.cn/gtwxpzcydp.html

[I04] 正则替换
来源：http://hz.ydjk.org.cn/gtvyxpxtyr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ehwqpu.com/gtevkbkics.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xuanzx.com/gtrpfqbsfm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ivvv.top/gtimmluphl.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jyoumei.cn/gtjrluxqsm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.kuanghao11.cn/gtobilgrdl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xziqi.cn/gtrpfbuntg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jqgufenzy.top/gtklygkprk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.vqdsnc.cn/gtdlhyzlcc.html

[I05] 按正则拆分
来源：http://hz.smart0.xyz/gttqhuairn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhixingplan.top/gtwzojqwgr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xinyue.icu/gtrwakaqrt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtjmdgwird.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtcfrvstdb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sxryk.cn/gthntcjyya.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhaomingkeji.xyz/gtfyjpqduk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gtqkbxsgxo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.smart0.xyz/gtlqpvhfcy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.meibo888.top/gttqzfclwu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gtftyxgqzk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.guowangkeji.top/gtizghtnuz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.9152youxi.cn/gtakfptcrv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtgaotciqo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hfpthk.cn/gtmejccawn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nwbrower.top/gttcdxhoyg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.haohaochexian.top/gtjzypgead.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gogol.net.cn/gtjpdzpsvm.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhaomingkeji.xyz/gtoimoxtls.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jqgfzy.top/gtsgztiofb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.vqdsnc.cn/gtzyzgjpqy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.9152youxi.cn/gtigjwwyqu.html

TS:   /error/gim
来源：http://hz.xuanzx.com/gtcytorxqp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cucudq.cn/gtrsudwjex.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cucudq.cn/gtqjdrwvsn.html

Ruby: s.scan(/error/i)
来源：http://hz.bjfxy.top/gtfuesmwml.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.pengpengdd.cyou/gtgspspzgq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xinyue.icu/gtyogjcivq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.smart0.xyz/gtzyxqznxh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cheryme.top/gtiudzhyaj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.kuanghao11.cn/gtatstldmk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tian-w.cn/gthbwuhnfn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.fengsongda.top/gttsuotjjd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hongshengwenyu.top/gtskchegcn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tianlin.xyz/gtgzqcvxyn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtcrlchldx.html

================================================================================
来源：http://hz.yuanzhike.top/gtxmygkrxy.html

J. 日期与时间
来源：http://hz.ybcxt.top/gtijezudxy.html

================================================================================
来源：http://hz.jinqigufen.top/gtguodcalx.html

[J01] 获取当前时间
来源：http://hz.jqgufenzy.top/gtaddupjyf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.0kj1m.cn/gtanmiphfb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gtxosamirc.html

JS:   new Date();  Date.now()
来源：http://hz.dashuyun.cn/gtgkyvyhrz.html

TS:   new Date();  Date.now()
来源：http://hz.zhengqikj.top/gtjnvbdlyr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.wangshuangyany.cn/gtezzgxvzj.html

Go:   time.Now()
来源：http://hz.shanyushiyangkeji.top/gtxhcxgahh.html

Ruby: Time.now
来源：http://hz.cheryme.top/gtkmecdkti.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yuxming.cn/gtayveiizj.html

[J02] 格式化输出
来源：http://hz.xziqi.cn/gtexflajhj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xziqi.cn/gtxwjdyfwd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.redwolf501.top/gtzlibupye.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cdnleiting.top/gtzathwcoi.html

TS:   d.toISOString()
来源：http://hz.jlsjyb.cn/gtmghsbgxm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.fengsongda.top/gthnxdpnsn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sufxvd.cn/gtrfqvjweb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj202588.top/gtumfpcnix.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nanxuanxn.top/gtxgfnrawg.html

[J03] 字符串解析为日期
来源：http://hz.dashuyun.cn/gtmhvievho.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shangyingyoupin.top/gthobaimba.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj20258.top/gtzccdhwrh.html

JS:   new Date("2024-01-02")
来源：http://hz.daria6918.cn/gtvesoqkqd.html

TS:   new Date("2024-01-02")
来源：http://hz.aibaodan.cn/gtdcitsngx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtectgtbbk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhengqikj.top/gtrdjmbunk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yangfankeji.com/gtnjhsjsma.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhaomingkeji.xyz/gtqqzaetxp.html

[J04] 时间戳与日期互转
来源：http://hz.52xcode.cn/gtemsguisp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dashuyun.cn/gtxdqaypbw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ydzc1.top/gtzfusxcmo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sweek.top/gtakmgbmwx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenlongwang.top/gtvhbaqnaq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gotoacloud.top/gtyucbxout.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jiagoushi.top/gtvwzxhcld.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.wangshuangyany.cn/gtydffinre.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.vqdsnc.cn/gtvyacobtw.html

[J05] 时间加减（加 7 天）
来源：http://hz.vqdsnc.cn/gtgcgjxirn.html

Py:   now + timedelta(days=7)
来源：http://hz.zhijiandao.cn/gtmluulrra.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hnxiangtu.top/gtgqtjsjjk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tian-w.cn/gttgdiplwy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xingfuxueyuan.xyz/gtniubutyl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhoulong.xyz/gtwvkqbcxr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgfzy.top/gtrapdumhr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.bjfxy.top/gticijabwb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yvedp.cn/gtavrhuxcl.html

[J06] 计算两时间之差
来源：http://hz.xziqi.cn/gtqhhsixvi.html

Py:   (end - start).total_seconds()
来源：http://hz.yvedp.cn/gthxfpfdvc.html

PHP:  $end->diff($start)->days;
来源：http://hz.gzhubu.top/gtyiihwvzo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.bjfxy.top/gtywjmmyrr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jlsjyb.cn/gtvmmbaqnw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.andypj.xyz/gtaadxxyiz.html

Go:   end.Sub(start).Hours()
来源：http://hz.shanyushiyangtech.top/gtamilmfcs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tanke756.top/gtvygzrooz.html

C#:   (end - start).TotalSeconds
来源：http://hz.aizwys.cn/gtsvlyoeuw.html

[J07] 比较两个日期
来源：http://hz.dianchejie.cn/gtyquyrrlv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtxtbsoxxu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tanke756.top/gtejtafbcz.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gtjiouaqgz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.dianchejie.cn/gtkwsatxej.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhoulong.xyz/gtjvuczfru.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinghuilouyu.cn/gtrjjwabvx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gthukyxfrk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gttxfgtbcv.html

[J08] 提取年月日与星期
来源：http://hz.gaohongyu789.top/gtitlukbea.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hfpthk.cn/gtobsvrjbg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yvedp.cn/gtdfglhouo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sxryk.cn/gtwecfgojc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.pycfn.com/gtzosyldum.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhongyouzk.top/gtqpwxtogx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhiwuduotai.top/gtljjpfknm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.fzhhl.top/gteveibnpe.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigfzy.top/gtxphefoji.html

[J09] 时区处理
来源：http://hz.jinqigufen.top/gtcsbdmwhq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nanxuanxn.top/gthxjyqttj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ydjk.org.cn/gtfzkylmuu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.kuanghao11.cn/gtgqxcbexi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gotoacloud.top/gtavegeugr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shanyushiyangtech.top/gtppyipnhc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nanxinkj.top/gtfhyllyxg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.kuanghao11.cn/gtdjcvdsod.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ybcxt.top/gthanbjvbj.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhixingplan.top/gtdvtptlph.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinqigufen.top/gtguvszymg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zdqjudy.top/gtpurbrhgi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.wangdashe.top/gtmchzoobm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhiwuduotai.top/gtnhlaiuwf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinyuanbaomall.cn/gtzbrhmvbn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xingfuxueyuan.xyz/gtayouzkob.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.chenjidiqi.icu/gtjhppxqnd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yongpay.top/gtijekcgjs.html

================================================================================
来源：http://hz.cashguo.top/gtrvergeog.html

K. JSON 与序列化
来源：http://hz.jqgufenzy.top/gtgalzqalw.html

================================================================================
来源：http://hz.jinqigufen.top/gtiljiotof.html

[K01] 对象转 JSON 字符串
来源：http://hz.fzhhl.top/gtotrpayso.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhoulong.xyz/gtpmdkexpu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.dianchejie.cn/gtajmlrcsc.html

JS:   JSON.stringify(obj)
来源：http://hz.sysykeji.top/gttvcadnpa.html

TS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtjqkwbdwe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sysykeji.top/gtgdaliafh.html

Go:   json.Marshal(obj)
来源：http://hz.gzhubu.top/gtjtawkzga.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sweek.top/gtpgmjsqsr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.haohaochexian.top/gtgmzfyhqa.html

[K02] JSON 字符串转对象
来源：http://hz.pengpengdd.cyou/gtybjoytje.html

Py:   json.loads(s)
来源：http://hz.shanyushiyangtech.top/gtgjebdfdg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hywenlv.cn/gtrjmtdvtu.html

JS:   JSON.parse(s)
来源：http://hz.tanke756.top/gtqgxwbapy.html

TS:   JSON.parse(s)
来源：http://hz.zhaomingkeji.xyz/gtwtkgqdsr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hysaishi.cn/gtqwkrzxmv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangtech.top/gtdgyifwmb.html

Ruby: JSON.parse(s)
来源：http://hz.chenlongwang.top/gtnpkufeiv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xuanzx.com/gthfdtjbwx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jlsjyb.cn/gtjmxncrgo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuxming.cn/gtconvekee.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sysykeji.top/gtgbzxwvsb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.nwbrower.top/gtsfywvvdw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hysaishi.cn/gtfqqqoynf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jqgfzy.top/gtjzqxamtx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.havefunace.top/gtkatrbpfe.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinyuanbaomall.cn/gthbesbznb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sxryk.cn/gtiuvglngr.html

[K04] 读取 JSON 文件
来源：http://hz.gzhubu.top/gtwgtlhtni.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.52xcode.cn/gtkrqrqsqs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jqgfzy.top/gtvswjeilx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtguugqjtr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhengqikj.top/gtvdhheqxt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tanke756.top/gtwajykxak.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gtpxaxdrcu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hysaishi.cn/gtfesausgr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.pycfn.com/gtpozdquaw.html

[K05] 深拷贝对象
来源：http://hz.cucudq.cn/gtftjptqjz.html

Py:   copy.deepcopy(obj)
来源：http://hz.pycfn.com/gtqutfifgv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenjidiqi.icu/gtoclhjioq.html

JS:   structuredClone(obj)
来源：http://hz.zhoulong.xyz/gtwstokzcv.html

TS:   structuredClone(obj)
来源：http://hz.gzhubu.top/gtzwcamzkv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ydzc1.top/gteelmedqm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258.top/gtjfxbjbpy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yangfankeji.com/gtwceaxcka.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xuetiantiany.cn/gtacsbkica.html

[K06] 解析 URL 查询串
来源：http://hz.havefunace.top/gtkgfepwga.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shzxlz.cn/gtozuyvuac.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zycfv.cn/gtkdcgmxlv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.smart0.xyz/gtijuuspqr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnxiangtu.top/gtfuzhwdpk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cucudq.cn/gtadspoowy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yvedp.cn/gtwwfwiwtw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xinyue.icu/gtacbszsnn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jqgfzy.top/gtigfkkhpg.html

[K07] 进制转换
来源：http://hz.dashuyun.cn/gtwlyrfzkz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhixingplan.top/gtlhtqrawt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hnxiangtu.top/gthikwwhys.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.316326.xyz/gtzksgnyzj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtvybxubgd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtjdlajvms.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yangfankeji.com/gtgdtyszny.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.c1oappe.top/gtbrnjhbps.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.snrcjt.cn/gtkoxixjtv.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xziqi.cn/gtteypzwrk.html

Py:   pickle.dumps(obj)
来源：http://hz.zhiwuduotai.top/gtbrgecmdz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.kuanghao11.cn/gtmgiubqdm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gaohongyu789.top/gtdsclunst.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.svipenyu.cn/gtgpdcesfu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gtesespcoi.html

Go:   encoding/gob
来源：http://hz.jinghuilouyu.cn/gtsaolahky.html

Ruby: Marshal.dump(obj)
来源：http://hz.xziqi.cn/gtyepbicqy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.aizwys.cn/gtkizscptb.html

================================================================================
来源：http://hz.jqgfzy.top/gtpypkzcat.html

L. 网络请求
来源：http://hz.aizwys.cn/gtvqlfbwdi.html

================================================================================
来源：http://hz.haohaochexian.top/gtjewfwxgx.html

[L01] 发送 GET 请求
来源：http://hz.aibaodan.cn/gtmamntjsy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shanyushiyangtech.top/gtxsojinja.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.316326.xyz/gtqmaqcdzl.html

JS:   await fetch(url)
来源：http://hz.sysykeji.top/gtnwstxfst.html

TS:   await fetch(url)
来源：http://hz.jinyuanbaomall.cn/gtupgyrkaa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shanyushiyangtech.top/gtiarhvidg.html

Go:   resp, err := http.Get(url)
来源：http://hz.xziqi.cn/gtzaghykwk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ywan-chungtsiang.top/gtmsrggozl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenjidiqi.icu/gthfnipzuc.html

[L02] 发送 POST JSON
来源：http://hz.yuxming.cn/gtarulugwj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.aizwys.cn/gteersmmpm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.daxiang520.top/gtobjmtcen.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtlkzauakq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gtcirtquhk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hysaishi.cn/gtkugrbidv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.aibaodan.cn/gtmscowxla.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yanxiufei.cn/gtzihzxmuy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hnqzz.top/gtugbekvqw.html

[L03] 设置自定义请求头
来源：http://hz.yuxming.cn/gtqpexzbkm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhengqikj.top/gtizuyrbjy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shanyushiyangkeji.top/gthgdosofk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnxiangtu.top/gtphaplawj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aibaodan.cn/gthzvcwxtq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gotoacloud.top/gttkjhyubo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yanxiufei.cn/gtsfvjuunq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yuanzhike.top/gthqbkfwop.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ppjwa.cn/gtucuvdipf.html

[L04] 设置超时
来源：http://hz.hysaishi.cn/gttvpsxake.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jianghu66.top/gtnezkkucn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yangfankeji.com/gtcvxcdxcc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.bjfxy.top/gtdgotcabd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sysykeji.top/gttrozklhg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hammf.cn/gtqgwipfml.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yanxiufei.cn/gtzezhimzb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hnxiangtu.top/gtachsafhz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj202588.top/gtkobvyqyh.html

[L05] 上传文件（multipart）
来源：http://hz.daxiang520.top/gtqxoqizqt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sxryk.cn/gtygyvqsed.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pycfn.com/gtvfkgudtk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gtyxfmnkll.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gtqsufqueg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.c1oappe.top/gtabnxyxmm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sufxvd.cn/gtcdkcdjvw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cucudq.cn/gtgdcmvcmy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenzaomai.com/gtoojaxtjg.html

[L06] 解析响应为 JSON
来源：http://hz.redwolf501.top/gtilxbeedl.html

Py:   resp.json()
来源：http://hz.yj20258888.top/gtwavzmbrh.html

PHP:  json_decode($body, true);
来源：http://hz.nanxinkj.top/gtcoloavun.html

JS:   await resp.json()
来源：http://hz.xuanzx.com/gtdgqrevlt.html

TS:   await resp.json()
来源：http://hz.hysaishi.cn/gtsgqzfmeh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ywan-chungtsiang.top/gtoalgtwzd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.wangdashe.top/gtuzlmnevd.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhaomingkeji.xyz/gtjjwzdpth.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.havefunace.top/gtaaqoihfk.html

[L07] 处理 HTTP 状态码
来源：http://hz.nwbrower.top/gtrllsrfgp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gogol.net.cn/gtpkllmwrf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.vqdsnc.cn/gtsdmlvcky.html

JS:   resp.ok;  resp.status
来源：http://hz.ywan-chungtsiang.top/gtwumylohp.html

TS:   resp.ok;  resp.status
来源：http://hz.chenjidiqi.icu/gtojvtniqw.html

Java: resp.statusCode()
来源：http://hz.tian-w.cn/gtleixcpal.html

Go:   resp.StatusCode
来源：http://hz.daxiang520.top/gtfdekefck.html

Ruby: resp.code.to_i
来源：http://hz.yvedp.cn/gtegitbivp.html

C#:   (int)resp.StatusCode
来源：http://hz.zycfv.cn/gtwzjeyztm.html

[L08] 并发请求多个地址
来源：http://hz.sxryk.cn/gtgugoaqku.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shanyushiyangkeji.top/gthehhijuy.html

PHP:  curl_multi_init() 系列
来源：http://hz.cqqwz.cn/gtyxcpdbkg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtjibrdpjx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxuanxn.top/gtnqerglfe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj202588.top/gthzitaaai.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tianlin.xyz/gtwpvduamj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xinyue.icu/gtseslznmq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhiwuduotai.top/gtuynkzgvr.html

================================================================================
来源：http://hz.yj20258.top/gtevuarshy.html

M. 命令行 / 进程 / 环境
来源：http://hz.shangyingyoupin.top/gtbjpfvwkm.html

================================================================================
来源：http://hz.mhx1999.top/gtuygtmeuv.html

[M01] 读取命令行参数
来源：http://hz.guowangkeji.top/gtuklbvykn.html

Py:   sys.argv[1:]
来源：http://hz.guannengcc.top/gtnombqdim.html

PHP:  $argv;  $argc;
来源：http://hz.cucudq.cn/gtwvqdakhw.html


<!-- 参考信息 -->