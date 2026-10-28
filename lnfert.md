代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gotoacloud.top/gtozjrkldp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hfpthk.cn/gtsexruweh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.52xcode.cn/gtmgalrsjb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj202588.top/gtetuwpesq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.52xcode.cn/gtotpnnxce.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.andypj.xyz/gtzvfzirvq.html

[I04] 正则替换
来源：http://hz.jinqigfzy.top/gtjwnbxwji.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yj20258.top/gtpohgnajh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhongyouzk.top/gteorukyiy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.aizwys.cn/gtsswwkyet.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtrusetkmv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jqgufenzy.top/gtkypvfprl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhixingplan.top/gtskmrttwf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhijiandao.cn/gtwgouzmvt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.guannengcc.top/gtjccnxqbs.html

[I05] 按正则拆分
来源：http://hz.jqgufenzy.top/gtcemzudzl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jqgfzy.top/gtatogqkmc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.snrcjt.cn/gtxqcypzpr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtgrahmhyz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtgcskctmb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinghuilouyu.cn/gtgknnucpj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenzaomai.com/gtzaehsoaj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sweek.top/gtypsizswv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hongshengwenyu.top/gtatwrnnxa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xziqi.cn/gtlwscuzwz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tanke756.top/gtvvgkyssa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinghuilouyu.cn/gtoffozsec.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sweek.top/gtbppmwotz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnxiangtu.top/gtsddbyqju.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj202588.top/gtrvjwtvub.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jianghu66.top/gtytrdouwh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sysykeji.top/gtetwrjsms.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtpbcfokhz.html

[I07] 忽略大小写与多行模式
来源：http://hz.quarkkingdee.top/gtprcpuozi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yuxming.cn/gtttqedewe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ppjwa.cn/gtucrexjbu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hysaishi.cn/gttetrurwm.html

TS:   /error/gim
来源：http://hz.iojbl.cn/gtrmktajgt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.vqdsnc.cn/gtlbsawcfk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.316326.xyz/gtuwgzvubu.html

Ruby: s.scan(/error/i)
来源：http://hz.meibo888.top/gtufxpguyw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.dianchejie.cn/gtravkuefv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cqqwz.cn/gtuknnkzqr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.bjfxy.top/gtcwbyxhqn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cheryme.top/gtkgoboidi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.birdmap.top/gtsefwwptd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtoafycjpb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.quarkkingdee.top/gtwinjckhp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gogol.net.cn/gtwvuklghj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hnxiangtu.top/gtjxndqohw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yongpay.top/gtwymibags.html

================================================================================
来源：http://hz.fengsongda.top/gtvefxrkea.html

J. 日期与时间
来源：http://hz.dianchejie.cn/gtwsnkudpl.html

================================================================================
来源：http://hz.0kj1m.cn/gtokzeytbx.html

[J01] 获取当前时间
来源：http://hz.nanxuanxn.top/gteouqsmch.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shzxlz.cn/gtogpiupnk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.0kj1m.cn/gtvxfidxiz.html

JS:   new Date();  Date.now()
来源：http://hz.hfpthk.cn/gtzkqqbddw.html

TS:   new Date();  Date.now()
来源：http://hz.sxryk.cn/gtcydageti.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.havefunace.top/gtqlkeogqg.html

Go:   time.Now()
来源：http://hz.shangyingyoupin.top/gtnukkbzvx.html

Ruby: Time.now
来源：http://hz.jinghuilouyu.cn/gtddwyiraa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yongpay.top/gtoilirafe.html

[J02] 格式化输出
来源：http://hz.52xcode.cn/gtkdxrxzzi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj202588.top/gtzmfxhqvd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gtutdoumwv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.andypj.xyz/gtmegrycfc.html

TS:   d.toISOString()
来源：http://hz.chenlongwang.top/gtejnrvbus.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.316326.xyz/gtbiwlsuse.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yj20258888.top/gtytmnygmt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nwbrower.top/gtqmzfutoj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gaohongyu789.top/gtwemdyuqw.html

[J03] 字符串解析为日期
来源：http://hz.aizwys.cn/gtfuxaweyz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hammf.cn/gtwfoklywl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.haohaochexian.top/gtvvqpfmkm.html

JS:   new Date("2024-01-02")
来源：http://hz.ppjwa.cn/gtdhzibavl.html

TS:   new Date("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtxlswchvf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj202588.top/gtuelcxpny.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tanke756.top/gtfnoxwija.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cheryme.top/gtqxsnztre.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.redwolf501.top/gtyfuylqds.html

[J04] 时间戳与日期互转
来源：http://hz.wangdashe.top/gteemzsidy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.kuanghao11.cn/gtptaoljvh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.fengsongda.top/gtbryxokpj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ydzc1.top/gtycmyplum.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.daxiang520.top/gtjmczwylk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.52xcode.cn/gteofvqszi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jlsjyb.cn/gtqjssjfjl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhengqikj.top/gtsykdvyae.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xziqi.cn/gtjgcwwhwx.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinyuanbaomall.cn/gtevsrvypb.html

Py:   now + timedelta(days=7)
来源：http://hz.gotoacloud.top/gtuganxuyp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gaohongyu789.top/gtwddspvlp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hysaishi.cn/gtrqogxfha.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigfzy.top/gtnhxevwxd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yanxiufei.cn/gtaknalznh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xziqi.cn/gtfvijstyl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.bjfxy.top/gthxksruvo.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jqgufenzy.top/gtovzljewn.html

[J06] 计算两时间之差
来源：http://hz.jinqigfzy.top/gtzdmwjxxe.html

Py:   (end - start).total_seconds()
来源：http://hz.yonumen.top/gtgjbchmwg.html

PHP:  $end->diff($start)->days;
来源：http://hz.tian-w.cn/gtokqbjckb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nanxuanxn.top/gtlxaddmbi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.snrcjt.cn/gttlhfgiqs.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xingfuxueyuan.xyz/gttroqhoiz.html

Go:   end.Sub(start).Hours()
来源：http://hz.birdmap.top/gtpduarose.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nanxuanxn.top/gtltoofusm.html

C#:   (end - start).TotalSeconds
来源：http://hz.sxryk.cn/gtbnlcbbpi.html

[J07] 比较两个日期
来源：http://hz.gaohongyu789.top/gtuwlqvaqb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtzkztzrxo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnqzz.top/gtxallrbcb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.mhx1999.top/gtnmrrpoip.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhaomingkeji.xyz/gtkqqmzapu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.haohaochexian.top/gtxbshmkzx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ppjwa.cn/gtlphwwbdc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtwuppfsxa.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtybmnawat.html

[J08] 提取年月日与星期
来源：http://hz.ivvv.top/gtkacoihuh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cashguo.top/gtquwupwgw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinyuanbaomall.cn/gtanwlapfo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sweek.top/gtjuvxktit.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ywan-chungtsiang.top/gtsqsxljgd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenlongwang.top/gtcevuxmrp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj20258888.top/gtppdcvwtq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shuidangran.top/gtbgtczhzr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj20258.top/gttdcfpcsy.html

[J09] 时区处理
来源：http://hz.wangshuangyany.cn/gtvkmxxynn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gzhubu.top/gtpebydifu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hongshengwenyu.top/gtkotrghqi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pycfn.com/gtydyuiqlc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.feifeiyinyue.top/gtlsjqrzpp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenlongwang.top/gtzhzziltm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hongshengwenyu.top/gtdgfawxkj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.redwolf501.top/gtdvzxohax.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ppjwa.cn/gtvwjmploh.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhongyouzk.top/gtdwkhskyd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xziqi.cn/gtqsazcrzn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ppjwa.cn/gtntrycokt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shanyushiyangkeji.top/gtbmeloybb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.birdmap.top/gtvbarzbyh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.52xcode.cn/gtrsvdtgkn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cdnleiting.top/gtfvnkfynv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.guowangkeji.top/gtixykkfgd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xingfuxueyuan.xyz/gtokugkyjm.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtlroemnib.html

K. JSON 与序列化
来源：http://hz.gotoacloud.top/gteylwgaro.html

================================================================================
来源：http://hz.hywenlv.cn/gtayrsucaf.html

[K01] 对象转 JSON 字符串
来源：http://hz.pengpengdd.cyou/gtaiuvzegd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shuidangran.top/gtxvwfocho.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cheryme.top/gtozuojeas.html

JS:   JSON.stringify(obj)
来源：http://hz.yongpay.top/gtrldmyogc.html

TS:   JSON.stringify(obj)
来源：http://hz.xingfuxueyuan.xyz/gtqdhwhagc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shanyushiyangtech.top/gtkiqzevnf.html

Go:   json.Marshal(obj)
来源：http://hz.shzxlz.cn/gtzhomcqvr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.birdmap.top/gtjtnrxbpt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nwbrower.top/gtjtnyuimr.html

[K02] JSON 字符串转对象
来源：http://hz.gzhubu.top/gtbqekmeqy.html

Py:   json.loads(s)
来源：http://hz.yj20258888.top/gtdsifepid.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hywenlv.cn/gtzvygaugq.html

JS:   JSON.parse(s)
来源：http://hz.guannengcc.top/gtchdzkywo.html

TS:   JSON.parse(s)
来源：http://hz.chenzaomai.com/gtothwlhhg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cqqwz.cn/gtvgzslpcj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtybnpkiaf.html

Ruby: JSON.parse(s)
来源：http://hz.zhongyouzk.top/gtbamywsit.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhiwuduotai.top/gtrfxialzl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.quarkkingdee.top/gthqmhvilk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xingfuxueyuan.xyz/gtrkjsvrpn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gtksnkogac.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnqzz.top/gtobtkwqhj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zdqjudy.top/gtmkuxqqdp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zdqjudy.top/gtypdltfdq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.0kj1m.cn/gtprnstmab.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.52xcode.cn/gtjtbeafxx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yj20258.top/gtpqypfijf.html

[K04] 读取 JSON 文件
来源：http://hz.haohaochexian.top/gtaddhyxyc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj20258888.top/gtwxdxfoae.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenjidiqi.icu/gtgwltzibc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.c1oappe.top/gtfcgtvrye.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxuanxn.top/gtmswzlkji.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zycfv.cn/gtxydszhav.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gtcrpqgjpc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhongyouzk.top/gtlulylwfq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tianlin.xyz/gtuvtftrtj.html

[K05] 深拷贝对象
来源：http://hz.jianghu66.top/gtrkraxhnp.html

Py:   copy.deepcopy(obj)
来源：http://hz.xingfuxueyuan.xyz/gtwpgggkpp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj20258.top/gtdybqiujz.html

JS:   structuredClone(obj)
来源：http://hz.zdqjudy.top/gthyidsneu.html

TS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtspcphzgx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zycfv.cn/gtlyzhoojq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xinyue.icu/gtajltrpeq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.316326.xyz/gtzgmbzbca.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.dianchejie.cn/gtlbgdzltj.html

[K06] 解析 URL 查询串
来源：http://hz.smart0.xyz/gtepcgjpqt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.dashuyun.cn/gtbqrioqni.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxuanxn.top/gthlqtgfdn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jlsjyb.cn/gtxqlgsvfc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.svipenyu.cn/gtgxehnvek.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ybcxt.top/gtxkiusrwz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yangfankeji.com/gtmyhkbuzl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.redwolf501.top/gthajbhnnl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.daxiang520.top/gtkzygxrwo.html

[K07] 进制转换
来源：http://hz.cheryme.top/gtwlwmswcw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jyoumei.cn/gtvhkzhppc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.meibo888.top/gtbyowxejg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtfuamfadq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtojuzxuqj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtjoxrhoin.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.chenzaomai.com/gtaxtykdvf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.pengpengdd.cyou/gtrrlovsms.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yongpay.top/gtisbauxkl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nwbrower.top/gtgedruneb.html

Py:   pickle.dumps(obj)
来源：http://hz.cheryme.top/gtbfspnypk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.pengpengdd.cyou/gtapcobkrn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.aizwys.cn/gtedseymjc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtupvvrzak.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.nwbrower.top/gtlpntklbs.html

Go:   encoding/gob
来源：http://hz.xinyue.icu/gtehjbrrwx.html

Ruby: Marshal.dump(obj)
来源：http://hz.xziqi.cn/gteenzvptb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hammf.cn/gtikjsitbp.html

================================================================================
来源：http://hz.cqqwz.cn/gtfowhgepi.html

L. 网络请求
来源：http://hz.xingfuxueyuan.xyz/gtvjdfqulj.html

================================================================================
来源：http://hz.bjfxy.top/gtfequzpdx.html

[L01] 发送 GET 请求
来源：http://hz.hammf.cn/gtbzpdixgp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhixingplan.top/gtkykdwmkj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yuanzhike.top/gtwerslsnh.html

JS:   await fetch(url)
来源：http://hz.yanxiufei.cn/gtizyacmda.html

TS:   await fetch(url)
来源：http://hz.ywan-chungtsiang.top/gtzxfnkquc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hammf.cn/gtyvcccglr.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhoulong.xyz/gtvzbgnmdr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gaohongyu789.top/gtdobonmkt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jqgfzy.top/gtchkxelkj.html

[L02] 发送 POST JSON
来源：http://hz.wangshuangyany.cn/gtyxovcpqn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yonumen.top/gtldrisizn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.snrcjt.cn/gtiimkqbcb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenlongwang.top/gtlykrjgzi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gtwfrxhcdd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ybcxt.top/gtvelmvsmc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yj202588.top/gtyagjylhn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ehwqpu.com/gtwbkeqseb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.dianchejie.cn/gtjejoknji.html

[L03] 设置自定义请求头
来源：http://hz.dashuyun.cn/gtiwamjnhv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.fengsongda.top/gttspcvlyz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinqigfzy.top/gtjewpwpvv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gtawslntgw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgfzy.top/gtrwuitgry.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.daxiang520.top/gthrjeuxge.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.daria6918.cn/gtqrlyqhlp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.wangdashe.top/gterkdkvjp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hammf.cn/gtkrltohna.html

[L04] 设置超时
来源：http://hz.jinghuilouyu.cn/gtjilpgold.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jiagoushi.top/gtpruxjwkb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhijiandao.cn/gtmhdcgotj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.svipenyu.cn/gtzqwotqrx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xingfuxueyuan.xyz/gtwjayzgqg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinghuilouyu.cn/gtqcspokso.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cqqwz.cn/gtttsqtxoy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.smart0.xyz/gtklakknnn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuetiantiany.cn/gtcdowcunu.html

[L05] 上传文件（multipart）
来源：http://hz.yonumen.top/gtgrmrlkdf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.vqdsnc.cn/gtvnzmjamo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jqgufenzy.top/gttthptxuf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hysaishi.cn/gtwxmyhyxp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgfzy.top/gtbwzicpiw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hnxiangtu.top/gtaarpdgtq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yueranfly.top/gtcqrpetuo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.redwolf501.top/gtxdmvtmvs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxuanxn.top/gtqjxbyrws.html

[L06] 解析响应为 JSON
来源：http://hz.yuanzhike.top/gtxmmrakcl.html

Py:   resp.json()
来源：http://hz.yvedp.cn/gtpfdwmgqo.html

PHP:  json_decode($body, true);
来源：http://hz.gotoacloud.top/gtjdjxfqka.html

JS:   await resp.json()
来源：http://hz.gaohongyu789.top/gticjykmsm.html

TS:   await resp.json()
来源：http://hz.nanxinkj.top/gtfmvspvnr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jiagoushi.top/gtrobqjqtw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yanxiufei.cn/gtxqmebofa.html

Ruby: JSON.parse(resp.body)
来源：http://hz.316326.xyz/gtnvboublw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shanyushiyangtech.top/gtjbskziaj.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinqigfzy.top/gtzvratfpe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.birdmap.top/gtkblyeiup.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.birdmap.top/gtzdxseoqe.html

JS:   resp.ok;  resp.status
来源：http://hz.yangfankeji.com/gtsvdhqnrz.html

TS:   resp.ok;  resp.status
来源：http://hz.aizwys.cn/gtamvenurf.html

Java: resp.statusCode()
来源：http://hz.pycfn.com/gtsazyzxug.html

Go:   resp.StatusCode
来源：http://hz.yj20258888.top/gtchrowphh.html

Ruby: resp.code.to_i
来源：http://hz.wangdashe.top/gttldkjlmh.html

C#:   (int)resp.StatusCode
来源：http://hz.hysaishi.cn/gteuultmch.html

[L08] 并发请求多个地址
来源：http://hz.jianghu66.top/gthydypsfq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.fzhhl.top/gttdwnnttx.html

PHP:  curl_multi_init() 系列
来源：http://hz.shuidangran.top/gtrkytyiug.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gtuizguiiq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gthchnoihb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shuidangran.top/gtuqgxnxam.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sufxvd.cn/gtrdmwhtzb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zycfv.cn/gthzaykbbv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cheryme.top/gttzskpvwh.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtdswqnwkr.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinqigfzy.top/gtthaahehl.html

================================================================================
来源：http://hz.yj202588.top/gtuzaxbtcn.html

[M01] 读取命令行参数
来源：http://hz.jlsjyb.cn/gtbucpybpi.html

Py:   sys.argv[1:]
来源：http://hz.dianchejie.cn/gteqokcawk.html

PHP:  $argv;  $argc;
来源：http://hz.zhixingplan.top/gtlhggfbvs.html


<!-- 参考信息 -->