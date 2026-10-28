代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shzxlz.cn/gtfseuimwa.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sysykeji.top/gtlioqjgrk.html

JS:   /\d+/.test(s)
来源：http://hz.yonumen.top/gtddneyfcx.html

TS:   /\d+/.test(s)
来源：http://hz.zhoulong.xyz/gtuoywvccy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinyuanbaomall.cn/gtjasqonve.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.haohaochexian.top/gtyhpeszdq.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj202588.top/gtxavltduy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gaohongyu789.top/gtthbgetvg.html

[I02] 提取所有匹配
来源：http://hz.9152youxi.cn/gtghsxrilg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.dashuyun.cn/gtymrwqthk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhoulong.xyz/gtpytwawkq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuetiantiany.cn/gtygkeobxq.html

TS:   s.match(/\d+/g)
来源：http://hz.dianchejie.cn/gtvvkeznaa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yongpay.top/gtqbzorxuu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.chenzaomai.com/gtacxvyezf.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenjidiqi.icu/gtdjxaqdwb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jianghu66.top/gtourkevvp.html

[I03] 提取捕获分组
来源：http://hz.ybcxt.top/gtjakowlyb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinqigufen.top/gtsdltygzx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shangyingyoupin.top/gtgbenpesc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nwbrower.top/gtdjdssprp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.52xcode.cn/gtabozbjvr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinqigufen.top/gtkuiitpvd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.svipenyu.cn/gtlcoengdb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cashguo.top/gtrtizjvhl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yanxiufei.cn/gtjbxuaska.html

[I04] 正则替换
来源：http://hz.aibaodan.cn/gtgabfjyfs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinghuilouyu.cn/gtuejqwutz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gzhubu.top/gtupsaadfw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinyuanbaomall.cn/gtmaezxrwp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xingfuxueyuan.xyz/gtprfeqsze.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xziqi.cn/gtkcgaxfok.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.daxiang520.top/gtbwaidvic.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.daxiang520.top/gtianntboy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yj20258.top/gtsnmxquco.html

[I05] 按正则拆分
来源：http://hz.nanxuanxn.top/gtchzwdqav.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hywenlv.cn/gtiqmtyeah.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigufen.top/gttnmgraux.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangtech.top/gtclcnptov.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gttuskegtu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.9152youxi.cn/gtxoxhezbi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xuanzx.com/gtncutdnbi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hfpthk.cn/gtdszfbygq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.nanxinkj.top/gtckhhhpwl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinqigfzy.top/gtaeupitxc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtxcqtqtfb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.svipenyu.cn/gtzufjqwbf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhixingplan.top/gtjalraxjz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dashuyun.cn/gtsiezrijn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xylfe.cn/gtxrmrekyf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jqgfzy.top/gtnxhjofqh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zdqjudy.top/gtggseatvx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhoulong.xyz/gtndmfprcd.html

[I07] 忽略大小写与多行模式
来源：http://hz.yangfankeji.com/gtjlwltyyr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nanxuanxn.top/gtewpqocat.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhixingplan.top/gtcpcwuphs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.daxiang520.top/gtltonwjew.html

TS:   /error/gim
来源：http://hz.meibo888.top/gthhqpkyri.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhixingplan.top/gtgubktplw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hfpthk.cn/gtcacrtwui.html

Ruby: s.scan(/error/i)
来源：http://hz.cucudq.cn/gtlalouija.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.fzhhl.top/gtntfpndhp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.dianchejie.cn/gtzwysqkez.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhaomingkeji.xyz/gtudxutieu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhaomingkeji.xyz/gtuhxrwfvp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dianchejie.cn/gtdmcojlts.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hongshengwenyu.top/gthpscwarx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daxiang520.top/gtcvxvwzac.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.havefunace.top/gtssfvnbkq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.feifeiyinyue.top/gtmeuqnhlc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.fengsongda.top/gtturcajyi.html

================================================================================
来源：http://hz.redwolf501.top/gtwpoyrqnv.html

J. 日期与时间
来源：http://hz.yonumen.top/gtnqhnefed.html

================================================================================
来源：http://hz.yj202588.top/gtzljzikef.html

[J01] 获取当前时间
来源：http://hz.cashguo.top/gtdcdjuilt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.pycfn.com/gtsvgyhqdg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gthrlyzbea.html

JS:   new Date();  Date.now()
来源：http://hz.yj202588.top/gtlqidtxap.html

TS:   new Date();  Date.now()
来源：http://hz.tanke756.top/gtqhtnzjbk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.feifeiyinyue.top/gtdsdmmfzo.html

Go:   time.Now()
来源：http://hz.zhoulong.xyz/gtozwpjcqa.html

Ruby: Time.now
来源：http://hz.sufxvd.cn/gtxvjcfszn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yueranfly.top/gtwgkjfccc.html

[J02] 格式化输出
来源：http://hz.cheryme.top/gtzudetnuo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ivvv.top/gtptcjrgfc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hnxiangtu.top/gtrkadnwin.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.fzhhl.top/gtreuxnncs.html

TS:   d.toISOString()
来源：http://hz.yongpay.top/gtvvpcuqge.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.kuanghao11.cn/gttwiganke.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhiwuduotai.top/gtpjmqwopq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gtdqyxbfui.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yj202588.top/gttsausdpe.html

[J03] 字符串解析为日期
来源：http://hz.gogol.net.cn/gteypmtsnc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cucudq.cn/gtdghnvvja.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhiwuduotai.top/gtzhrrsgkz.html

JS:   new Date("2024-01-02")
来源：http://hz.yonumen.top/gtlgddriuc.html

TS:   new Date("2024-01-02")
来源：http://hz.c1oappe.top/gtntozhrbv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtubgnwzok.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhixingplan.top/gtxawydron.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.haohaochexian.top/gtptuzvnev.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.9152youxi.cn/gtjjucllhy.html

[J04] 时间戳与日期互转
来源：http://hz.yuxming.cn/gtfbzhzyjm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dashuyun.cn/gtqsepqklf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cheryme.top/gtgpxtyrrc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ywan-chungtsiang.top/gtatbkpsue.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.fzhhl.top/gtepyanvbo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.andypj.xyz/gthkjqfryr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sufxvd.cn/gtqhmlotdh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cheryme.top/gtydvhjbrb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.bjfxy.top/gtubjqmqsk.html

[J05] 时间加减（加 7 天）
来源：http://hz.andypj.xyz/gthqcftxkm.html

Py:   now + timedelta(days=7)
来源：http://hz.zhixingplan.top/gtdxnexsvr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jlsjyb.cn/gtxiitxcnv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dianchejie.cn/gtuwnqtafa.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.316326.xyz/gtvcfglaco.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinqigfzy.top/gtvsfysaxl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yangfankeji.com/gtkcybunrq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xingfuxueyuan.xyz/gttcitxxde.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xuetiantiany.cn/gtjookvuqt.html

[J06] 计算两时间之差
来源：http://hz.jinghuilouyu.cn/gtcvfmnbng.html

Py:   (end - start).total_seconds()
来源：http://hz.xuanzx.com/gtdwlddljx.html

PHP:  $end->diff($start)->days;
来源：http://hz.andypj.xyz/gtyielhuee.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yuanzhike.top/gtkkvixdfc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jianghu66.top/gttiasdgpi.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jqgufenzy.top/gtmvlnhvvz.html

Go:   end.Sub(start).Hours()
来源：http://hz.9152youxi.cn/gtylmslxtl.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nwbrower.top/gtdfefcqlo.html

C#:   (end - start).TotalSeconds
来源：http://hz.hywenlv.cn/gthxwqukei.html

[J07] 比较两个日期
来源：http://hz.fzhhl.top/gttousxulv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhijiandao.cn/gttjdubila.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tianlin.xyz/gtblsedcdu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shzxlz.cn/gtdgkjesow.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tianlin.xyz/gthpgmuofp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dashuyun.cn/gtoznudpec.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gotoacloud.top/gtbzjuhuzy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtvxwbdlgk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtwyyvuolq.html

[J08] 提取年月日与星期
来源：http://hz.aizwys.cn/gtegprvvkr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinghuilouyu.cn/gtopwktbxp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.chenjidiqi.icu/gtcfmkslab.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigufen.top/gtdmzzdkuq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.guowangkeji.top/gthvahroki.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yangfankeji.com/gtqmtjpcon.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gzhubu.top/gtewvrjkdz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenzaomai.com/gtxasyswlp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yanxiufei.cn/gtlsnknkvm.html

[J09] 时区处理
来源：http://hz.zhixingplan.top/gthhtxjjfo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cashguo.top/gtuvgkrazf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.0kj1m.cn/gtjxrcxoap.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtkbhqlwcu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtzjecumia.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ybcxt.top/gtwzdbjqam.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xinyue.icu/gtfkqgnjtp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.vqdsnc.cn/gtxfxkfsor.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhoulong.xyz/gtmqetfgsz.html

[J10] 取今天 / 本月第一天
来源：http://hz.cheryme.top/gtixhfiujb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ehwqpu.com/gtjzrzosxr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.haohaochexian.top/gtjymbvvre.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.daria6918.cn/gtvlhstuvu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuanzhike.top/gtedwnvdoe.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yanxiufei.cn/gtvcfhohup.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinqigfzy.top/gtesusomqt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.fengsongda.top/gtfxgotzkd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.chenjidiqi.icu/gtquvwiuph.html

================================================================================
来源：http://hz.jqgfzy.top/gtlnlihuih.html

K. JSON 与序列化
来源：http://hz.jyoumei.cn/gtnwclpdii.html

================================================================================
来源：http://hz.yanxiufei.cn/gtidhurcqf.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258.top/gtcwqhojnm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zdqjudy.top/gtyogubupd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shzxlz.cn/gtdhrhiqvl.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gteyxnqvyx.html

TS:   JSON.stringify(obj)
来源：http://hz.iojbl.cn/gtoxyhvikr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jqgfzy.top/gtvasxflwl.html

Go:   json.Marshal(obj)
来源：http://hz.nanxinkj.top/gtxgkokgdv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shzxlz.cn/gtbiebggtp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yueranfly.top/gttrzkuofs.html

[K02] JSON 字符串转对象
来源：http://hz.shangyingyoupin.top/gtbdbodgdi.html

Py:   json.loads(s)
来源：http://hz.xingfuxueyuan.xyz/gtwengycxc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ivvv.top/gtwqjjxdmi.html

JS:   JSON.parse(s)
来源：http://hz.yj20258.top/gtwtmcufhe.html

TS:   JSON.parse(s)
来源：http://hz.cucudq.cn/gtgbadydpa.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258.top/gthzuxdpkv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gaohongyu789.top/gtezrccrco.html

Ruby: JSON.parse(s)
来源：http://hz.zhongyouzk.top/gtzqmuagwx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jlsjyb.cn/gtnjvutlfi.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hywenlv.cn/gttbsqosvb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.pengpengdd.cyou/gtcytelvqw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jlsjyb.cn/gtzsrehrnq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.316326.xyz/gtmjwhuxci.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shangyingyoupin.top/gtohehsfmq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tanke756.top/gtloolzvlg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.aizwys.cn/gtgtpedhyw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jqgufenzy.top/gtfgzrypyu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.snrcjt.cn/gtrudpwvqm.html

[K04] 读取 JSON 文件
来源：http://hz.0kj1m.cn/gtopnawswb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.birdmap.top/gtbbyfblnj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.dashuyun.cn/gticioampm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zdqjudy.top/gtdaxyoikc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtfsqckcgj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ydjk.org.cn/gtplnftrkb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.redwolf501.top/gtgdunzmjv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.meibo888.top/gtdansvgwu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shanyushiyangtech.top/gtumzriveu.html

[K05] 深拷贝对象
来源：http://hz.cdnleiting.top/gttyyhdson.html

Py:   copy.deepcopy(obj)
来源：http://hz.meibo888.top/gtneotrjac.html

PHP:  unserialize(serialize($obj));
来源：http://hz.mhx1999.top/gtqswyxfco.html

JS:   structuredClone(obj)
来源：http://hz.hongshengwenyu.top/gtdtfvjlkk.html

TS:   structuredClone(obj)
来源：http://hz.jinqigfzy.top/gtdkccbgmr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.birdmap.top/gtmvoupwgs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fzhhl.top/gtafyxhcrn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.aizwys.cn/gtdizgshzi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hfpthk.cn/gtiirlyxwi.html

[K06] 解析 URL 查询串
来源：http://hz.mhx1999.top/gtpviprevq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuanzx.com/gtcsiygmbj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gaohongyu789.top/gttunnebpl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tianlin.xyz/gtbhdmwnlr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gtznpbtqpj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinyuanbaomall.cn/gtaljngekd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.quarkkingdee.top/gtrcdxripo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenzaomai.com/gtonkidehp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.guowangkeji.top/gtavvberso.html

[K07] 进制转换
来源：http://hz.yuxming.cn/gtosfavcbx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinqigufen.top/gteziariqy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.redwolf501.top/gtqktjhuia.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hnqzz.top/gthxxixzxu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.haohaochexian.top/gtouypmaxc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtuwceietj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj20258888.top/gtxqizykbl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gogol.net.cn/gtkxhvzivt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtlfrvlmuc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.0kj1m.cn/gtguxqtabe.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258.top/gtnotgwblh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.nwbrower.top/gtmbjsbjhx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtjkvqhdua.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xinyue.icu/gtzorcwldo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ehwqpu.com/gthqvtwinf.html

Go:   encoding/gob
来源：http://hz.yj20258.top/gtovqslkis.html

Ruby: Marshal.dump(obj)
来源：http://hz.xziqi.cn/gtzfpazqyv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangtech.top/gtxvkbvweg.html

================================================================================
来源：http://hz.xylfe.cn/gtwvcdnoxa.html

L. 网络请求
来源：http://hz.mhx1999.top/gtwawykmjk.html

================================================================================
来源：http://hz.hfpthk.cn/gtmmsohnax.html

[L01] 发送 GET 请求
来源：http://hz.meibo888.top/gtcagjqrpv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tanke756.top/gtamoqecww.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gaohongyu789.top/gtuhpfwijc.html

JS:   await fetch(url)
来源：http://hz.ybcxt.top/gtmgwpuumc.html

TS:   await fetch(url)
来源：http://hz.jianghu66.top/gtjbxlysja.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinghuilouyu.cn/gtuvltivil.html

Go:   resp, err := http.Get(url)
来源：http://hz.birdmap.top/gtnjipgihb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xuanzx.com/gtgytzdcup.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinghuilouyu.cn/gtiinqtrsx.html

[L02] 发送 POST JSON
来源：http://hz.ivvv.top/gtdyonpxut.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nanxinkj.top/gtavuoqjyg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fengsongda.top/gtfieeyipr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtmlxvwhbw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tianlin.xyz/gtabneebcq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.0kj1m.cn/gtastadrmp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yuanzhike.top/gtxmveoaca.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.mhx1999.top/gthptesheu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gzhubu.top/gtaakxmlvv.html

[L03] 设置自定义请求头
来源：http://hz.iojbl.cn/gtavwcccjd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.pycfn.com/gtydohptsz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cdnleiting.top/gtizrnfsue.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cashguo.top/gtkvztfoeo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhengqikj.top/gttpvbkonx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenlongwang.top/gtpirqtnxl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zycfv.cn/gtduaeoicm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xingfuxueyuan.xyz/gtpemmmrai.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtyfnmhfko.html

[L04] 设置超时
来源：http://hz.gogol.net.cn/gtktzjlpdt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yanxiufei.cn/gticbseoti.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yongpay.top/gtfdpojevl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258888.top/gtzdyuqdig.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.smart0.xyz/gtwtncfkfm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tian-w.cn/gtkcgshlxr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hammf.cn/gtpdlwzcmh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.daxiang520.top/gtonjjfhjf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj202588.top/gtjdqtjdzc.html

[L05] 上传文件（multipart）
来源：http://hz.feifeiyinyue.top/gtbzgzxkwj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.mhx1999.top/gtqybfokcb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cheryme.top/gtbqitomuq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sxryk.cn/gtyimtpnrf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gotoacloud.top/gttihineej.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zycfv.cn/gthmchnojl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jqgfzy.top/gtftoddory.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xziqi.cn/gtgflfclbn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.vqdsnc.cn/gtxrlbghrp.html

[L06] 解析响应为 JSON
来源：http://hz.quarkkingdee.top/gtecbqthqx.html

Py:   resp.json()
来源：http://hz.yueranfly.top/gtryvpxvqa.html

PHP:  json_decode($body, true);
来源：http://hz.nwbrower.top/gtsxfgsxys.html

JS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gtzznsugez.html

TS:   await resp.json()
来源：http://hz.andypj.xyz/gtebkpzntv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinyuanbaomall.cn/gtxutmwbig.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gotoacloud.top/gtulvqehse.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gzhubu.top/gtwuohmxbw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shuidangran.top/gtiopomffo.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj20258.top/gtklpthqfr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhijiandao.cn/gtffvwzhwz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shzxlz.cn/gtiybqfaeq.html

JS:   resp.ok;  resp.status
来源：http://hz.yvedp.cn/gtjdigxdoc.html


<!-- 参考信息 -->