代发 wailian999

TS:   s.match(/\d+/g)
来源：http://hz.daxiang520.top/gtmwmxgweq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.wangshuangyany.cn/gteademgwf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ivvv.top/gtxhgatvtu.html

Ruby: s.scan(/\d+/)
来源：http://hz.cucudq.cn/gtokzzvacd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.mhx1999.top/gtezimkwjh.html

[I03] 提取捕获分组
来源：http://hz.ydjk.org.cn/gtczmecbso.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhongyouzk.top/gtcjhequhx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yueranfly.top/gtolyuojoo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.9152youxi.cn/gtadckqqad.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.svipenyu.cn/gtdlvewclx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pycfn.com/gtwsbpflty.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tianlin.xyz/gtusauzhqu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hfpthk.cn/gtsvxvvgjn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shzxlz.cn/gtfjlkvsei.html

[I04] 正则替换
来源：http://hz.jiagoushi.top/gtulwrxuaj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tanke756.top/gtdqfusxeu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258.top/gttxdhjbsx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhixingplan.top/gtfpaelrpy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigufen.top/gtdeuyaryl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hammf.cn/gtvngdzlgm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hysaishi.cn/gtiqalygnm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jiagoushi.top/gtoeeepjth.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.guannengcc.top/gtzygycqpo.html

[I05] 按正则拆分
来源：http://hz.yangfankeji.com/gtdwytyvxo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zdqjudy.top/gtlqdsncnp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhoulong.xyz/gtjrukhdbs.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtwtcjgjjg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtknvtqqbc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ybcxt.top/gtkkhozraf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.daria6918.cn/gtkxzrumbn.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtbsxlzqnc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhongyouzk.top/gtlshqaenm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gogol.net.cn/gtsieuixqo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xinyue.icu/gtjbwdnouc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yueranfly.top/gttgsashli.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigufen.top/gtcehfzcmv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhongyouzk.top/gtbnjgminw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.daxiang520.top/gtwvcvieda.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hnxiangtu.top/gtlmxoqbmv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.aibaodan.cn/gtcfmvgytl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.0kj1m.cn/gtzylzlarn.html

[I07] 忽略大小写与多行模式
来源：http://hz.shangyingyoupin.top/gtcdrfcogh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.kuanghao11.cn/gtlqutggyr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yonumen.top/gtlsvamsvb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.chenzaomai.com/gtxtblygpl.html

TS:   /error/gim
来源：http://hz.ehwqpu.com/gtbsfwvdmr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yongpay.top/gterddfvmj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.9152youxi.cn/gteyzfdpgq.html

Ruby: s.scan(/error/i)
来源：http://hz.tian-w.cn/gtzlvuodig.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.pengpengdd.cyou/gtbtcdwewu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shzxlz.cn/gtrydscbwa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hfpthk.cn/gtvgtumvex.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daxiang520.top/gtahuiybud.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gtrfwgtadd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.mhx1999.top/gtapfnmmhs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xuanzx.com/gthauqyiiw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yvedp.cn/gtthhtemgu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ivvv.top/gtmmpsavpd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhoulong.xyz/gtqrzxmtnk.html

================================================================================
来源：http://hz.0kj1m.cn/gtndsgwbgx.html

J. 日期与时间
来源：http://hz.bjfxy.top/gtkqfmqxix.html

================================================================================
来源：http://hz.jiagoushi.top/gtsyzejcoo.html

[J01] 获取当前时间
来源：http://hz.bjfxy.top/gtkfiloiid.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.wangdashe.top/gtmfomdsuc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hysaishi.cn/gtzyiipuqw.html

JS:   new Date();  Date.now()
来源：http://hz.xziqi.cn/gtovhlimij.html

TS:   new Date();  Date.now()
来源：http://hz.fengsongda.top/gtucqqgpgj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xinyue.icu/gtebtidbde.html

Go:   time.Now()
来源：http://hz.yuxming.cn/gtnnktpwqy.html

Ruby: Time.now
来源：http://hz.ppjwa.cn/gtvlesbgyn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.0kj1m.cn/gtgqyklbcc.html

[J02] 格式化输出
来源：http://hz.aizwys.cn/gtcqksgfeg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gtvgkmwgnr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gthlzhaaeg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sysykeji.top/gtgoqvqtjc.html

TS:   d.toISOString()
来源：http://hz.zdqjudy.top/gtgbuqpkpj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinqigfzy.top/gtdsdmqntp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tanke756.top/gtjzaauceu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.pycfn.com/gtfncqszhc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xylfe.cn/gtqvagidsf.html

[J03] 字符串解析为日期
来源：http://hz.snrcjt.cn/gttgswpdzb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ppjwa.cn/gttzqvupxb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.aibaodan.cn/gthtfnncnw.html

JS:   new Date("2024-01-02")
来源：http://hz.9152youxi.cn/gtorrsibut.html

TS:   new Date("2024-01-02")
来源：http://hz.gogol.net.cn/gtmzjtaspw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj202588.top/gttsmkmxyu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.52xcode.cn/gtmnshuxiz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gthfudemrx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.birdmap.top/gtkmkmcepz.html

[J04] 时间戳与日期互转
来源：http://hz.mhx1999.top/gtqodezcfk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shuidangran.top/gtackxoctt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yvedp.cn/gtjtlifdoe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jyoumei.cn/gtkhqxtezb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shuidangran.top/gtqvpdybdw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ybcxt.top/gtlzfazinx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj20258.top/gtfopxhgyw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinyuanbaomall.cn/gtvjhmlubu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sysykeji.top/gtugqybkpy.html

[J05] 时间加减（加 7 天）
来源：http://hz.yonumen.top/gtymarjifz.html

Py:   now + timedelta(days=7)
来源：http://hz.haohaochexian.top/gtczptbsrr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.snrcjt.cn/gtemcgobed.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhijiandao.cn/gtltenltxs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgufenzy.top/gtvbmykvuo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gogol.net.cn/gtvqylegek.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenzaomai.com/gtsslkqgnd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuxming.cn/gtwbxfgipa.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tanke756.top/gtgvfvluii.html

[J06] 计算两时间之差
来源：http://hz.hfpthk.cn/gtfhufzbhk.html

Py:   (end - start).total_seconds()
来源：http://hz.bjfxy.top/gtvmoyhtvq.html

PHP:  $end->diff($start)->days;
来源：http://hz.xuetiantiany.cn/gtexcqztks.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.meibo888.top/gtofdvokkm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ywan-chungtsiang.top/gtcxbshbvy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.fzhhl.top/gtzhuzgiki.html

Go:   end.Sub(start).Hours()
来源：http://hz.sysykeji.top/gtuemtibqs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhiwuduotai.top/gtbgjledus.html

C#:   (end - start).TotalSeconds
来源：http://hz.havefunace.top/gtqkmneqxt.html

[J07] 比较两个日期
来源：http://hz.zdqjudy.top/gtdqxpydfz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtbsnjfyss.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangdashe.top/gtrowrlgvu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.daxiang520.top/gtlwywthgv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.bjfxy.top/gtcbuemhrr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cheryme.top/gtyixzxjil.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.0kj1m.cn/gttmgobxpb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtysmjqiho.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtnczpoabf.html

[J08] 提取年月日与星期
来源：http://hz.kuanghao11.cn/gtqahrgbgp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sysykeji.top/gtgwuqeklk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.guowangkeji.top/gtvdaugowy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yangfankeji.com/gtvponpfcr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigfzy.top/gtqrteckor.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cheryme.top/gtezluxqwe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.feifeiyinyue.top/gtvgzludyo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.guannengcc.top/gtlkabwzhg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yuxming.cn/gtfjigczog.html

[J09] 时区处理
来源：http://hz.jinqigfzy.top/gttbluhfxx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.wangshuangyany.cn/gtounvqyhr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ehwqpu.com/gtmyqmpior.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtnfgwtmnj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cashguo.top/gtuzadiwvh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhengqikj.top/gtxricelfg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shanyushiyangtech.top/gtsrvvyqcl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hywenlv.cn/gtrbfxlwqj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.smart0.xyz/gtshqcewfj.html

[J10] 取今天 / 本月第一天
来源：http://hz.wangdashe.top/gtpqzqqsby.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cashguo.top/gtetgvhhks.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tian-w.cn/gtkbcrnemf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenzaomai.com/gtlzauhccr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yonumen.top/gtlbhsczov.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.feifeiyinyue.top/gtomrkepoj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shanyushiyangkeji.top/gtzgwfdlii.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tianlin.xyz/gtzmocsnkh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinyuanbaomall.cn/gttgxgmssf.html

================================================================================
来源：http://hz.daxiang520.top/gtpjbwisui.html

K. JSON 与序列化
来源：http://hz.jqgufenzy.top/gtfgkrwbdz.html

================================================================================
来源：http://hz.yuanzhike.top/gtchabpsdl.html

[K01] 对象转 JSON 字符串
来源：http://hz.hongshengwenyu.top/gtjqoyqxda.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yueranfly.top/gtifhxopjd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shzxlz.cn/gtptcrdooo.html

JS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gtwejpoynh.html

TS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gtexbeqsyv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yonumen.top/gtomieisjf.html

Go:   json.Marshal(obj)
来源：http://hz.jlsjyb.cn/gtgurvptiw.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhongyouzk.top/gtamunaprm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinyuanbaomall.cn/gtcshgzelx.html

[K02] JSON 字符串转对象
来源：http://hz.yueranfly.top/gtpugjisbx.html

Py:   json.loads(s)
来源：http://hz.chenzaomai.com/gtjzxuxunx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.quarkkingdee.top/gturnugbtq.html

JS:   JSON.parse(s)
来源：http://hz.cucudq.cn/gtfvxemgoc.html

TS:   JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtbdqriblw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ppjwa.cn/gtfqxzyple.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtihhrnquf.html

Ruby: JSON.parse(s)
来源：http://hz.hywenlv.cn/gtkwphpekv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hammf.cn/gtojlqlxlc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cqqwz.cn/gtszrybuao.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gtrzatomyj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ehwqpu.com/gtquudazoy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.pengpengdd.cyou/gteuntpsrt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.snrcjt.cn/gtorbtqqbl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zdqjudy.top/gtbqnijjgh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hammf.cn/gtkoxzybeq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gogol.net.cn/gtjeacjkcn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.nanxuanxn.top/gtlqunydxz.html

[K04] 读取 JSON 文件
来源：http://hz.nanxuanxn.top/gthshqxyzc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hnxiangtu.top/gtwoubmltk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.feifeiyinyue.top/gtoliikfcd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guannengcc.top/gtizkxpjhc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhixingplan.top/gtrnoexykt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pengpengdd.cyou/gtdkkhndgr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.smart0.xyz/gtirujlyfa.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhaomingkeji.xyz/gtewytsunb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guannengcc.top/gtrmwulmgh.html

[K05] 深拷贝对象
来源：http://hz.sxryk.cn/gtufiknhzw.html

Py:   copy.deepcopy(obj)
来源：http://hz.fzhhl.top/gtpymqovyx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ehwqpu.com/gtylfeteek.html

JS:   structuredClone(obj)
来源：http://hz.jinqigfzy.top/gtkyltbbtd.html

TS:   structuredClone(obj)
来源：http://hz.sweek.top/gtlizckhlv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jyoumei.cn/gtvlpjsmzl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.snrcjt.cn/gtungfihkv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ywan-chungtsiang.top/gtrmmifuvf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pengpengdd.cyou/gtdyjpdwfl.html

[K06] 解析 URL 查询串
来源：http://hz.xinyue.icu/gtjtahctfj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj202588.top/gtuorfhhhu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jiagoushi.top/gtupyvwejz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtobgvqnom.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gtbeyxtkwu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.gogol.net.cn/gtndixmwya.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tanke756.top/gtosxvojjg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xuanzx.com/gtlvbgoaoe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.wangdashe.top/gtqyziznxx.html

[K07] 进制转换
来源：http://hz.ywan-chungtsiang.top/gtmcgmnzam.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hnqzz.top/gtulmcjznn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gogol.net.cn/gtpymdixzm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtdadzdyrp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtjonszgkl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hysaishi.cn/gtgzevvrjh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.haohaochexian.top/gtmmtwtziq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xziqi.cn/gtwnavnvxg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinqigufen.top/gtjwdemsqh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.wangshuangyany.cn/gtjeanfxah.html

Py:   pickle.dumps(obj)
来源：http://hz.jinqigfzy.top/gtsipvztae.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ydzc1.top/gtnodtbhxc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenzaomai.com/gtipcdiocr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.316326.xyz/gtnlulrlwp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ppjwa.cn/gtnhocskcu.html

Go:   encoding/gob
来源：http://hz.tian-w.cn/gtbjlpafkz.html

Ruby: Marshal.dump(obj)
来源：http://hz.shzxlz.cn/gturrvpjle.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gogol.net.cn/gtmgvgypqs.html

================================================================================
来源：http://hz.xylfe.cn/gtafzhxigl.html

L. 网络请求
来源：http://hz.zhengqikj.top/gtgbmjgrlr.html

================================================================================
来源：http://hz.zhengqikj.top/gtccdyooax.html

[L01] 发送 GET 请求
来源：http://hz.jinyuanbaomall.cn/gtferimggm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zycfv.cn/gtahgaseex.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xylfe.cn/gthbguqhqo.html

JS:   await fetch(url)
来源：http://hz.cheryme.top/gtiqeavhnp.html

TS:   await fetch(url)
来源：http://hz.nwbrower.top/gtqkmgijzx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xziqi.cn/gtvscfered.html

Go:   resp, err := http.Get(url)
来源：http://hz.feifeiyinyue.top/gtjhpfmdxy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cashguo.top/gtbxppelvj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xziqi.cn/gtmlpfbaio.html

[L02] 发送 POST JSON
来源：http://hz.kuanghao11.cn/gtwxlacfdl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.haohaochexian.top/gttbnldecc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.andypj.xyz/gtlscffbgp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dianchejie.cn/gtjcixortb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gtuwpoffgz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sxryk.cn/gtsxmrfjox.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xylfe.cn/gtdraczelc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cashguo.top/gtukbblpjk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydjk.org.cn/gtzjngnwqv.html

[L03] 设置自定义请求头
来源：http://hz.daria6918.cn/gtlmeouoap.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tian-w.cn/gtaffbfhna.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sysykeji.top/gtszwqattk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shangyingyoupin.top/gtjbwchozj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yueranfly.top/gtjchmdyvn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhixingplan.top/gtwhaeqslc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxinkj.top/gtussknabe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ywan-chungtsiang.top/gtpfqwpdwv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.chenzaomai.com/gtfqcadczm.html

[L04] 设置超时
来源：http://hz.yj20258888.top/gtzhahnhng.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ybcxt.top/gthxapaasu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yuxming.cn/gtscjpaqsk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cucudq.cn/gtevlejfzs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sysykeji.top/gtygqumacg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.316326.xyz/gtnioiodpi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sweek.top/gtoiikybwd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.wangdashe.top/gtjkxcmrwv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.fzhhl.top/gtftbxutji.html

[L05] 上传文件（multipart）
来源：http://hz.sxryk.cn/gtnrjkjhbp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.316326.xyz/gtzdmiwhob.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.havefunace.top/gtunqfndgb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hywenlv.cn/gtffrshlgl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.mhx1999.top/gtehnsqrkq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhiwuduotai.top/gtopyekomp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hnqzz.top/gtjwoexcbk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.fzhhl.top/gtdxsbzjkw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gzhubu.top/gtquktxnil.html

[L06] 解析响应为 JSON
来源：http://hz.cheryme.top/gtfkaewfug.html

Py:   resp.json()
来源：http://hz.zhiwuduotai.top/gtlahstdgz.html

PHP:  json_decode($body, true);
来源：http://hz.xylfe.cn/gthrizmbfu.html

JS:   await resp.json()
来源：http://hz.birdmap.top/gtbzelmwnj.html

TS:   await resp.json()
来源：http://hz.jinyuanbaomall.cn/gtppobxifn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.wangshuangyany.cn/gtkqttzffu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhaomingkeji.xyz/gtkzcflxlm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shanyushiyangkeji.top/gtckaqbkap.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinqigfzy.top/gtmjdtevjo.html

[L07] 处理 HTTP 状态码
来源：http://hz.9152youxi.cn/gthpdwqwsc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj202588.top/gtiulenglo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yueranfly.top/gtomhwfjor.html

JS:   resp.ok;  resp.status
来源：http://hz.ybcxt.top/gtznividzu.html

TS:   resp.ok;  resp.status
来源：http://hz.xziqi.cn/gtidxvpwsa.html

Java: resp.statusCode()
来源：http://hz.ybcxt.top/gtqjydemqo.html

Go:   resp.StatusCode
来源：http://hz.hfpthk.cn/gthdojzopz.html

Ruby: resp.code.to_i
来源：http://hz.yangfankeji.com/gtwepesfld.html

C#:   (int)resp.StatusCode
来源：http://hz.52xcode.cn/gtnaslytbi.html

[L08] 并发请求多个地址
来源：http://hz.yj20258.top/gtkkmmgowm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gogol.net.cn/gtlmgtvsdk.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhijiandao.cn/gtaqmndvvc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gogol.net.cn/gtbfefpprz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinyuanbaomall.cn/gtdjqbwklq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.vqdsnc.cn/gtlcnjieue.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yangfankeji.com/gtwvkzvyqi.html


<!-- 参考信息 -->